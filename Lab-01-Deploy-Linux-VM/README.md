# Lab 01 – Deploy a Linux Virtual Machine

## Overview

This lab focuses on deploying and exploring a Linux virtual machine in Microsoft Azure.

The objective is to understand the Azure infrastructure created during deployment, establish a secure SSH connection and perform basic Linux administration tasks. This lab serves as the foundation for the remaining AZ-104 project.

---

## Objectives

* Deploy an Ubuntu Linux VM in Microsoft Azure
* Understand the Azure resources created during deployment
* Configure secure SSH authentication
* Connect to the VM from macOS
* Explore the Linux file system
* Execute basic Linux commands

---

## Technologies

* Microsoft Azure
* Ubuntu 24.04 LTS
* Azure Virtual Machine
* Azure Virtual Network (VNet)
* Network Security Group (NSG)
* SSH (Ed25519)
* macOS Terminal
* Git & GitHub

---

## Azure Resources

The deployment includes the following Azure resources:

* Resource Group
* Virtual Machine
* Virtual Network
* Subnet
* Network Security Group
* Network Interface
* Public IP Address
* Managed Disk
* SSH Key Authentication

---

## Screenshots

| Screenshot                     | Description                          |
| ------------------------------ | ------------------------------------ |
| 01-resource-group-overview.png | Resource Group overview              |
| 02-vm-overview.png             | Virtual Machine overview             |
| 03-vm-networking.png           | Networking configuration             |
| 04-nsg-ssh-rule.png            | SSH inbound rule (Port 22)           |
| 05-ssh-login.png               | Successful SSH connection from macOS |

---

## Files

```text
Lab-01-Deploy-Linux-VM/
├── README.md
├── notes.md
└── screenshots/
    ├── 01-resource-group-overview.png
    ├── 02-vm-overview.png
    ├── 03-vm-networking.png
    ├── 04-nsg-ssh-rule.png
    └── 05-ssh-login.png
```

---

## Skills Practiced

* Azure Virtual Machines
* Azure Networking
* SSH Authentication
* Linux Administration
* Terminal Commands
* Azure Resource Management
* Git Version Control

---

## Status

**Completed**

✔ Ubuntu VM deployed

✔ Azure resources created

✔ SSH authentication configured

✔ Successful SSH connection

✔ Basic Linux commands executed

✔ Project documented

---

## Next Lab

**Lab 02 – Azure Networking**
