# Lab 02 – Azure Networking

## Overview

This lab explores the core networking components of Microsoft Azure.

The objective is to understand how Azure Virtual Networks, Subnets, Network Interfaces and Network Security Groups work together to provide secure communication between Azure resources and external clients.

---

## Objectives

* Explore an Azure Virtual Network (VNet)
* Understand Address Spaces and CIDR notation
* Analyse Azure Subnets
* Understand Private and Public IP addresses
* Learn the purpose of a Network Interface (NIC)
* Explore Network Security Groups (NSGs)
* Understand NSG priorities and rule evaluation
* Understand Effective Security Rules
* Learn how SSH traffic reaches an Azure Virtual Machine

---

## Technologies

* Microsoft Azure
* Azure Virtual Network (VNet)
* Azure Subnet
* Azure Network Interface (NIC)
* Azure Network Security Group (NSG)
* IPv4 Networking
* CIDR Notation
* SSH

---

## Azure Resources

* Resource Group
* Virtual Network
* Subnet
* Network Interface
* Network Security Group
* Public IP Address
* Linux Virtual Machine

---

## Skills Practiced

* Azure Virtual Networks
* Azure Subnets
* IPv4 Addressing
* CIDR Notation
* Azure Network Interfaces
* Public and Private IP Addressing
* Azure Network Security Groups
* NSG Rule Priorities
* Effective Security Rules
* Azure Networking Architecture
* Azure Portal Navigation

---

## Network Architecture

```text
                    Internet
                        │
                        ▼
              Public IP Address
              20.228.163.134
                        │
                        ▼
           Network Interface (NIC)
                rg-lab-01491
                        │
                        ▼
       Network Security Group (NSG)
          Allow SSH (TCP Port 22)
                        │
                        ▼
             Subnet (default)
               10.0.0.0/24
                        │
                        ▼
      Virtual Network (VNet)
              10.0.0.0/16
                        │
                        ▼
            Ubuntu Linux VM
        rg-lab-01 (10.0.0.4)
```

---

## Screenshots

| Screenshot                          | Description                  |
| ----------------------------------- | ---------------------------- |
| 01-vnet-overview.png                | Virtual Network overview     |
| 02-address-space.png                | Address Space configuration  |
| 03-subnets.png                      | Available subnets            |
| 04-default-subnet-details.png       | Default subnet configuration |
| 05-network-settings-overview.png    | VM network configuration     |
| 06-network-security-group-rules.png | NSG inbound security rules   |
| 07-effective-security-rules.png     | Effective security rules     |

---

## Status

🟢 Completed

* Virtual Network analysed
* Address Space analysed
* CIDR notation understood
* Subnet configuration analysed
* Public and Private IP addresses explained
* Network Interface architecture understood
* Network Security Group rules analysed
* Effective Security Rules reviewed
* Azure networking architecture documented


---

## Next Lab

**Lab 03 – Azure Storage**



