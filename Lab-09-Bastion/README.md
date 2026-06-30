# Lab 09 - Azure Bastion

## Objective

The goal of this lab was to deploy and configure an Azure Bastion Host to securely connect to Azure Virtual Machines without exposing RDP (3389) or SSH (22) ports to the Internet.

Azure Bastion provides browser-based remote access through the Azure Portal and significantly improves the security posture of virtual machine management.

---

## Technologies Used

- Microsoft Azure
- Azure Bastion
- Virtual Network (VNet)
- AzureBastionSubnet
- Public IP Address
- Resource Groups
- Azure Portal

---

## Lab Steps

### 1. Open Azure Bastion

Navigate to:

Azure Portal → Bastions

**Screenshot**

`01-overview.png`

---

### 2. Create Azure Bastion

Configured the following settings:

- Resource Group
- Bastion Name
- Region
- Basic Tier
- Existing Virtual Network
- AzureBastionSubnet
- New Public IP

**Screenshot**

`02-create-basics.png`

---

### 3. Advanced Configuration

Reviewed Advanced settings.

No additional configuration was required for this lab.

**Screenshot**

`03-advanced.png`

---

### 4. Tags

Skipped optional tags.

**Screenshot**

`04-tags.png`

---

### 5. Review + Create

Validated the deployment configuration before creating the Bastion resource.

**Screenshot**

`05-review.png`

---

### 6. Deployment

Azure started provisioning the Bastion Host.

Provisioning required several minutes because multiple Azure networking resources were configured automatically.

**Screenshot**

`06-deployment.png`

---

### 7. Deployment Completed

Azure successfully deployed the Bastion Host.

**Screenshot**

`07-success.png`

---

### 8. Bastion Overview

Verified the Bastion resource after deployment.

**Screenshot**

`08-bastion-overview.png`

---

# What I Learned

During this lab I learned:

- What Azure Bastion is.
- Why Azure Bastion is more secure than exposing RDP or SSH ports.
- How browser-based remote administration works.
- Why Azure Bastion removes the need for Public IP addresses on Virtual Machines.
- How Azure creates a secure tunnel between the Azure Portal and the VM.
- Why AzureBastionSubnet is required.
- Why AzureBastionSubnet must use the exact reserved name.
- Why Azure Bastion requires at least a /26 subnet.
- The purpose of the Bastion Public IP.
- The difference between Basic and Standard Bastion tiers.
- How Azure validates networking before deployment.
- Why Bastion deployments take several minutes.
- Common deployment errors and how to resolve them.

---

# Security Benefits

Azure Bastion improves security by:

- Eliminating exposed RDP ports (3389)
- Eliminating exposed SSH ports (22)
- Protecting against port scanning
- Reducing brute-force attack surface
- Centralising remote administration
- Encrypting management traffic
- Providing secure browser-based access

---

# Key Takeaways

- Azure Bastion provides secure remote administration.
- Virtual Machines no longer require Public IP addresses.
- AzureBastionSubnet is mandatory.
- AzureBastionSubnet must be at least /26.
- Bastion communicates through the Azure Portal.
- Bastion is a Platform as a Service (PaaS) offering.
- Azure handles the infrastructure automatically.

---

# Result

Successfully deployed and validated an Azure Bastion Host that provides secure browser-based management access to Azure Virtual Machines.
