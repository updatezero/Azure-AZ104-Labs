# Final Project – Azure Virtual Machine Deployment & Network Configuration

## Overview

This final project demonstrates the deployment of a secure Linux virtual machine in Microsoft Azure using core AZ-104 administration concepts.

The environment includes a custom virtual network, multiple subnets, a Network Security Group (NSG), SSH connectivity, and a running Nginx web server accessible over HTTP.

---

## Objectives

- Deploy an Ubuntu Linux virtual machine
- Create and configure a Resource Group
- Configure a Virtual Network with multiple subnets
- Secure the environment using a Network Security Group (NSG)
- Connect securely using SSH
- Install and verify an Nginx web server
- Validate external HTTP access

---

## Azure Services Used

- Azure Resource Group
- Azure Virtual Network (VNet)
- Subnets
- Azure Network Security Group (NSG)
- Azure Virtual Machine (Ubuntu 24.04 LTS)
- Public IP Address
- SSH
- Nginx Web Server

---

## Network Architecture

Internet
│
Public IP
│
Network Security Group
│
Frontend Subnet
│
Ubuntu Virtual Machine
│
Nginx Web Server

Additional infrastructure:

- Backend Subnet
- AzureBastionSubnet

---

## Configuration Summary

| Component | Configuration |
|----------|---------------|
| Operating System | Ubuntu Server 24.04 LTS |
| VM Size | Standard D2s v3 |
| Virtual Network | vnet-final-project |
| Frontend Subnet | 10.10.1.0/24 |
| Backend Subnet | 10.10.2.0/24 |
| Azure Bastion Subnet | 10.10.3.0/26 |
| NSG | nsg-final-project |
| SSH Port | 22 |
| HTTP Port | 80 |
| Web Server | Nginx |

---

## Deployment Steps

1. Created a Resource Group
2. Created a Virtual Network
3. Configured Frontend, Backend and Azure Bastion subnets
4. Created a Network Security Group
5. Associated the NSG with the Frontend subnet
6. Deployed an Ubuntu virtual machine
7. Connected to the VM using SSH
8. Installed the Nginx web server
9. Opened HTTP (Port 80) in the NSG
10. Verified successful access to the web server

---

## Verification

Successful verification included:

- SSH connection established
- Nginx service running
- HTTP access verified through the browser
- Azure networking configured correctly

---

## Screenshots

- Resource Group
- Virtual Network & Subnets
- Network Security Group
- VM Deployment
- VM Overview
- VM Networking
- SSH Connection
- SSH Session
- Nginx Web Server

---

## Skills Demonstrated

- Azure Virtual Machine deployment
- Virtual Network configuration
- IP addressing and subnetting
- Network Security Group configuration
- SSH administration
- Linux server management
- Nginx installation
- Azure networking fundamentals
- Basic cloud infrastructure deployment

---

## Lessons Learned

During this project I gained practical experience deploying and securing Azure infrastructure.

Key takeaways include:

- Designing Azure virtual networks
- Understanding subnet segmentation
- Applying Network Security Groups
- Managing Linux virtual machines
- Connecting securely via SSH
- Installing and validating web server services
- Publishing a web application over HTTP
- Troubleshooting connectivity between Azure networking and virtual machines

---

## Technologies

- Microsoft Azure
- Ubuntu Server 24.04 LTS
- Azure Virtual Network
- Azure Network Security Groups
- SSH
- Nginx
