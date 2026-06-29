# Lab 03 – Azure Storage

## Objective

Deploy and explore an Azure Storage Account and understand the different storage services available in Microsoft Azure.

---

## Business Scenario

Contoso Ltd. requires a secure and scalable cloud storage solution for company documents, application data and future backups. As the Azure Administrator, the task is to deploy an Azure Storage Account, explore its services and understand how Azure protects stored data.

---

## Azure Resources

- Resource Group
- Storage Account
- Blob Container
- Blob
- Azure File Share
- Shared Access Signature (SAS)
- Access Keys

---

## Storage Configuration

| Setting | Value |
|----------|-------|
| Storage Account | artstorageaz104 |
| Region | East US |
| Performance | Standard |
| Redundancy | Locally Redundant Storage (LRS) |
| Account Kind | StorageV2 (General Purpose v2) |

---

## Blob Storage

### Container

Container created:

```text
documents
```

### Uploaded Blob

```text
hello.txt
```

The blob was uploaded successfully and later modified to test Blob Versioning.

---

## Blob Versioning

Blob Versioning was enabled.

After modifying and uploading the file again, Azure automatically created an older version of the blob.

This allows previous versions to be restored if a file is accidentally overwritten.

---

## Azure Files

Created File Share:

```text
companyfiles
```

Azure Files provides SMB-based file shares that can be mounted as a network drive on Windows, macOS and Linux.

Unlike Blob Storage, Azure Files behaves like a traditional file server.

---

## Shared Access Signature (SAS)

Generated a SAS Token with:

- Read permission
- HTTPS only
- Limited expiration time

A SAS URL allows temporary access to a blob without exposing the Storage Account Key.

---

## Access Keys

Azure automatically creates two Storage Account Keys.

Having two keys allows administrators to rotate credentials without interrupting running applications.

Access Keys provide full access to the Storage Account and should therefore be protected carefully.

---

## Key Learnings

- Created an Azure Storage Account
- Understood the purpose of StorageV2
- Learned the difference between Blob Storage and Azure Files
- Created a Blob Container
- Uploaded files to Azure Blob Storage
- Tested Blob Versioning
- Created an Azure File Share
- Learned how SMB File Shares work
- Generated and tested a Shared Access Signature (SAS)
- Explored Azure Access Keys
- Compared Access Keys with SAS Tokens
- Understood LRS redundancy
- Learned the difference between Hot, Cool and Cold storage tiers

---

## Screenshots

- 01_Storage_Account_Overview.png
- 02_Blob_Containers.png
- 03_Documents_Container_HelloBlob.png
- 04_Blob_Versioning.png
- 05_Data_Protection_Settings.png
- 06_Azure_File_Share_Overview.png
- 07_FileShare_Connect.png
- 08_Shared_Access_Signature.png
- 09_Access_Keys.png

---

## Lab Status

✅ Completed
