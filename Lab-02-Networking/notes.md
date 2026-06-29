# Lab 02 Notes

## Objective

Understand the networking architecture of Microsoft Azure by analysing an existing Virtual Network, Subnet, Network Interface and Network Security Group.

---

## Virtual Network (VNet)

A Virtual Network (VNet) is a private network in Microsoft Azure.

All Azure virtual machines must be connected to a Virtual Network.

Current VNet:

* Name: rg-lab-01-vnet
* Address Space: 10.0.0.0/16

---

## Address Space

The Virtual Network uses the following address space:

10.0.0.0/16

The /16 CIDR notation means that the first 16 bits identify the network.

This provides 65,536 IPv4 addresses inside the Virtual Network.

---

## Subnet

Current subnet:

* Name: default
* Address Range: 10.0.0.0/24

A subnet divides a large Virtual Network into smaller logical networks.

The current subnet contains 256 IPv4 addresses.

Azure reserves several addresses for internal services.

---

## Private and Public IP

Private IP:

10.0.0.4

Public IP:

20.228.163.134

The Private IP is used for communication inside the Virtual Network.

The Public IP allows external access from the Internet.

Without a Public IP, direct SSH access from the Internet would not be possible.

---

## Network Interface (NIC)

The Virtual Machine communicates through a Network Interface.

The Network Interface owns:

* Private IP Address
* Public IP Address (optional)
* Network Security Group (optional)
* IP Configurations
* Load Balancer association

The Virtual Machine uses the Network Interface to access the network.

---

## Network Security Group (NSG)

Current NSG:

rg-lab-01-nsg

Inbound SSH access is allowed on TCP Port 22.

Azure evaluates NSG rules by priority.

Lower priority numbers are processed before higher numbers.

The first matching rule is applied.

---

## Effective Security Rules

The Network Interface uses one Network Security Group.

No additional subnet-level NSG is configured.

Therefore, the effective security rules are identical to the rules configured in the attached Network Security Group.

---

## Key Learnings

* Understand Virtual Networks
* Understand Address Spaces
* Understand CIDR notation
* Understand Subnets
* Understand Public vs Private IP addresses
* Understand Network Interfaces
* Understand Network Security Groups
* Understand NSG priorities
* Understand the First Match Wins principle
