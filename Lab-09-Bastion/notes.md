# Notes - Lab 09: Azure Bastion

## Overview

Azure Bastion is a fully managed Platform-as-a-Service (PaaS) solution that provides secure Remote Desktop Protocol (RDP) and Secure Shell (SSH) connectivity to Azure Virtual Machines directly through the Azure Portal.

Unlike traditional remote access methods, Azure Bastion eliminates the need to expose management ports to the public Internet.

---

# Why Azure Bastion?

Traditionally, administrators connected to Azure Virtual Machines using:

- RDP (TCP 3389)
- SSH (TCP 22)

Both ports are common attack targets.

If these ports are publicly accessible, attackers can perform:

- Brute Force Attacks
- Password Spraying
- Credential Stuffing
- Port Scanning
- Exploitation of vulnerable services

Azure Bastion removes this risk by keeping management traffic entirely within Azure.

---

# Azure Bastion Architecture

Traditional Connection

Administrator

↓

Internet

↓

Public IP

↓

Virtual Machine

↓

RDP / SSH

---

Azure Bastion

Administrator

↓

Azure Portal (HTTPS)

↓

Azure Bastion Host

↓

AzureBastionSubnet

↓

Virtual Machine (Private IP)

No management ports need to be exposed to the Internet.

---

# AzureBastionSubnet

Azure Bastion requires a dedicated subnet.

Requirements:

Subnet Name

AzureBastionSubnet

This name is mandatory.

Azure automatically searches for this subnet during deployment.

If the subnet has another name, deployment fails.

---

# Subnet Size

Azure Bastion requires at least:

/26

Reason:

Azure reserves multiple internal addresses for Bastion infrastructure.

Smaller subnets such as /27 or /28 are not supported.

---

# Public IP Address

Azure Bastion requires its own dedicated Public IP Address.

Important:

The Bastion Public IP is NOT assigned to the Virtual Machine.

Instead, it belongs exclusively to the Bastion Host.

The Virtual Machine can remain private.

---

# Bastion Tiers

## Basic

Suitable for:

- Small environments
- Learning labs
- Simple remote administration

Supports:

- RDP
- SSH
- Browser-based connection

---

## Standard

Adds features such as:

- Native Client Support
- IP Connect
- Shareable Links
- Session Recording (depending on Azure updates)
- More enterprise capabilities

---

# Deployment Process

During deployment Azure automatically:

- Validates the Virtual Network
- Validates AzureBastionSubnet
- Creates Bastion infrastructure
- Creates networking components
- Associates the Public IP
- Deploys Bastion

Deployment typically takes several minutes.

---

# Common Deployment Problems

## AzureBastionSubnet missing

Deployment fails.

Solution:

Create AzureBastionSubnet manually.

---

## Wrong subnet name

Deployment fails.

Must be:

AzureBastionSubnet

---

## Subnet too small

Deployment fails.

Minimum supported size:

/26

---

## Public IP already in use

A Public IP assigned to a Virtual Machine cannot also be assigned to Azure Bastion.

Create a dedicated Public IP.

---

# Security Advantages

Azure Bastion provides:

- Secure browser-based administration
- No exposed RDP port
- No exposed SSH port
- Reduced attack surface
- Centralized management
- Encrypted management traffic
- Zero Trust friendly architecture

---

# Best Practices

Microsoft recommends:

- Remove Public IP addresses from Virtual Machines whenever possible.
- Use Azure Bastion for administration.
- Restrict administrator access using RBAC.
- Protect administrator accounts with Multi-Factor Authentication.
- Enable monitoring using Azure Monitor.
- Review Bastion diagnostic logs regularly.

---

# AZ-104 Exam Knowledge

After completing this lab I understand:

- What Azure Bastion is.
- Why Azure Bastion improves security.
- Difference between Bastion and direct RDP/SSH.
- AzureBastionSubnet requirements.
- Minimum subnet size (/26).
- Why Bastion requires its own Public IP.
- Basic vs Standard Bastion.
- Azure Bastion deployment workflow.
- Common deployment errors.
- Secure VM administration best practices.

---

# Key Learnings

This lab taught me how Azure Bastion secures remote administration by eliminating direct exposure of management ports.

I learned how Azure creates a dedicated AzureBastionSubnet, why a /26 subnet is required, and how Bastion establishes secure browser-based sessions without assigning a Public IP to the Virtual Machine itself.

Additionally, I gained practical experience troubleshooting deployment failures, including missing subnets and networking configuration issues.

Azure Bastion is an important security service for Azure administrators and is frequently referenced in the AZ-104 certification exam.
