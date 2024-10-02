Uploading Payload: ⠋Process & "C:\\Users\\n1605156\\Downloads\\sdipta_local\\.hyperexecute\\azcopy.exe" copy "yaml\\win\\mask-5b51ecf7-d6dc-4f35-87dc-d74471ad4cba.yaml" "https://hestoragebjhvnle3phxju.blob.core.windows.net/misc/raw-yaml/org-1194560/5b51ecf7-d6dc-4f35-87dc-d74471ad4cba.yaml?rscd=attachment%3B+filename%3Draw-yaml%2Forg-1194560%2F5b51ecf7-d6dc-4f35-87dc-d74471ad4cba.yaml&se=2024-10-02T12%3A35%3A46Z&sig=CnqfH6VA2L70xLRHYNudLMWtwsyyxr5WvR7dX7Ya0Js%3D&ske=2024-10-03T16%3A22%3A22Z&skoid=afe30b9f-c426-48ec-b8ad-66f6f4317a77&sks=b&skt=2024-10-01T16%3A22%3A22Z&sktid=08a83339-90e7-49bf-9075-957ccd561bf1&skv=2023-11-03&sp=rcwl&spr=https&sr=b&st=2024-10-02T10%3A30%3A46Z&sv=2021-12-02" --log-level=NONE failed------------> with error: exit status 1Stdout: Stderr: Output sTDERR---->>
Output---->> &{  %!s(int=1) exit status 1}
------- error ERR::JOB::UPL     Unable to upload job payload -> github.com/Azure/azure-storage-blob-go/azblob.newStorageError, /Users/shubhamr/go/pkg/mod/github.com/!azure/azure-storage-blob-go@v0.13.0/azblob/zc_storage_error.go:42
===== RESPONSE ERROR (ServiceCode=ContainerNotFound) =====
Description=The specified container does not exist.
RequestId:be66ccbf-801e-0070-39b6-140a34000000
Time:2024-10-02T10:36:06.3665224Z, Details:
   Code: ContainerNotFound
   PUT https://hestoragebjhvnle3phxju.blob.core.windows.net/misc/raw-yaml/org-1194560/5b51ecf7-d6dc-4f35-87dc-d74471ad4cba.yaml?rscd=attachment%3B+filename%3Draw-yaml%2Forg-1194560%2F5b51ecf7-d6dc-4f35-87dc-d74471ad4cba.yaml&se=2024-10-02t12%3A35%3A46z&sig=REDACTED&ske=2024-10-03t16%3A22%3A22z&skoid=afe30b9f-c426-48ec-b8ad-66f6f4317a77&sks=b&skt=2024-10-01t16%3A22%3A22z&sktid=08a83339-90e7-49bf-9075-957ccd561bf1&skv=2023-11-03&sp=rcwl&spr=https&sr=b&st=2024-10-02t10%3A30%3A46z&sv=2021-12-02&timeout=1801
   Content-Length: [1012]
   User-Agent: [Azure-Storage/0.13 (go1.23.1; Windows_NT)]
   X-Ms-Blob-Cache-Control: []
   X-Ms-Blob-Content-Disposition: []
   X-Ms-Blob-Content-Encoding: []
   X-Ms-Blob-Content-Language: []
   X-Ms-Blob-Content-Type: []
   X-Ms-Blob-Type: [BlockBlob]
   X-Ms-Client-Request-Id: [b7681fcc-20e5-4333-7378-71290f16a87d]
   X-Ms-Version: [2019-12-12]
   --------------------------------------------------------------------------------
   RESPONSE Status: 404 The specified container does not exist.
   Content-Length: [225]
   Content-Type: [application/xml]
   Date: [Wed, 02 Oct 2024 10:36:05 GMT]
   Server: [Windows-Azure-Blob/1.0 Microsoft-HTTPAPI/2.0]
   X-Ms-Client-Request-Id: [b7681fcc-20e5-4333-7378-71290f16a87d]
   X-Ms-Error-Code: [ContainerNotFound]
   X-Ms-Request-Id: [be66ccbf-801e-0070-39b6-140a34000000]
   X-Ms-Version: [2019-12-12]
