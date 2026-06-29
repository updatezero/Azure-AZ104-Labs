# Lab 03 – Azure Storage

## Overview

This lab focuses on Microsoft Azure Storage services.

The objective is to deploy and explore an Azure Storage Account while understanding Blob Storage, Azure Files, redundancy, security and access management.

---

## Objectives

- Create an Azure Storage Account
- Understand StorageV2
- Explore Blob Storage
- Create Blob Containers
- Upload files to Azure Blob Storage
- Enable Blob Versioning
- Explore Azure Files
- Create an Azure File Share
- Generate and test a Shared Access Signature (SAS)
- Explore Storage Account Access Keys
- Understand LRS redundancy

---

## Technologies

- Microsoft Azure
- Azure Storage Account
- Azure Blob Storage
- Azure Files
- Shared Access Signature (SAS)
- Azure Access Keys
- SMB
- StorageV2

---

## Azure Resources

- Resource Group
- Storage Account
- Blob Container
- Blob
- Azure File Share

---

## Storage Architecture

```text
                Azure Storage Account
                     artstorageaz104
                           │
        ┌──────────────────┴──────────────────┐
        │                                     │
   Blob Storage                         Azure Files
        │                                     │
  Container: documents              File Share: companyfiles
        │
    hello.txt
```

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| 01_Storage_Account_Overview.png | Storage Account overview |
| 02_Blob_Containers.png | Blob Containers |
| 03_Documents_Container_HelloBlob.png | Uploaded Blob |
| 04_Blob_Versioning.png | Blob Versioning |
| 05_Data_Protection_Settings.png | Data Protection configuration |
| 06_Azure_File_Share_Overview.png | Azure File Share |
| 07_FileShare_Connect.png | SMB connection script |
| 08_Shared_Access_Signature.png | Shared Access Signature |
| 09_Access_Keys.png | Storage Account Access Keys |

---

## Skills Practiced

- Azure Storage
- Azure Blob Storage
- Azure Files
- Storage Account Management
- Blob Versioning
- Soft Delete
- Shared Access Signature (SAS)
- Storage Account Access Keys
- SMB File Shares
- Azure Security
- Azure Portal Navigation

---

## Key Learnings

- Azure Storage Accounts provide multiple storage services within a single resource.
- Blob Containers organise blobs similarly to folders.
- Blob Versioning protects against accidental overwrites.
- Azure Files provides SMB-based file shares for multiple users.
- SAS Tokens provide temporary and limited access without exposing Access Keys.
- Access Keys provide full administrative access and should be protected carefully.
- LRS stores three copies of data within a single Azure datacenter.

---

## Status

**Completed** ✅

✔ Storage Account deployed

✔ Blob Container created

✔ Blob uploaded

✔ Blob Versioning tested

✔ Azure File Share created

✔ SAS Token generated and tested

✔ Access Keys explored

✔ Lab documented

---

## Next Lab

**Lab 04 – Azure RBAC**
