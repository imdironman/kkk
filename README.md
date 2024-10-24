const { exec } = require('child_process');

function listPlaywrightTests(file) {
  return new Promise((resolve, reject) => {
    const command =`npx playwright test --list ${file}`;
    exec(command, (error, stdout, stderr) => {
      if (error) {
        console.log('-------------->>')
        reject(error);
        return;
      }
      if (stderr) {
        
        console.error('stderr:', stderr);
        reject(stderr);
        return;
      }

      // Split the output into lines and trim the first and last lines
      let lines = stdout.trim().split('\n');
      if (lines.length > 2) {
        lines = lines.slice(1, -2);
      } else {
        reject('Insufficient lines to process.');
        return;
      }

      // Regex pattern to extract the part after the last '›'
      const pattern = /[^›]+$/;
      const testTitles = lines.map(line => {
        const match = line.match(pattern);
        return match ? match[0].trim() : null;
      }).filter(Boolean); // Filter out null values

      if (!testTitles.length) {
        console.error('No test titles found.');
        reject('No test titles found.');
        return;
      }

      resolve(testTitles.slice(0, -1));
    });
  });
}

const file = process.argv[2]?process.argv[2]:"";

listPlaywrightTests(file)
  .then(testTitles => {
    console.log('------------------------')
    // You can do something with the test titles here
    testTitles.forEach(element => {
      console.log(element);
    });
  })
  .catch(error => {
    console.error('Error:', error);
  });
