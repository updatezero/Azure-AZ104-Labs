# Final Project Notes

## Objective

Build a complete Azure infrastructure by combining multiple AZ-104 concepts into one practical deployment.

---

## What I Learned

### Azure Resource Groups

- Organizing Azure resources into a single logical container
- Managing related resources together

---

### Virtual Networks

- Creating custom VNets
- Planning IP address ranges
- Designing subnet structures

Address Space

10.10.0.0/16

Subnets

- Frontend: 10.10.1.0/24
- Backend: 10.10.2.0/24
- AzureBastionSubnet: 10.10.3.0/26

---

### Network Security Groups (NSG)

Learned how NSGs control inbound and outbound traffic.

Configured:

- SSH (22)
- HTTP (80)

Understanding rule priorities was important when allowing traffic.

---

### Azure Virtual Machine

Created an Ubuntu Server 24.04 LTS virtual machine.

Configured:

- Public IP
- SSH Authentication
- Standard D2s v3
- Ubuntu 24.04 LTS

---

### SSH

Connected securely from macOS Terminal using an SSH private key.

Useful commands:

```bash
chmod 400 vm-frontend-01_key.pem

ssh -i vm-frontend-01_key.pem azureuser@<Public-IP>
```

---

### Linux Administration

Basic Linux commands used:

```bash
hostname

hostname -I

ip a

pwd

ls

sudo apt update

sudo apt install nginx -y

sudo systemctl status nginx
```

---

### Nginx

Installed and configured Nginx.

Verified:

- Service running
- Website reachable via browser
- HTTP Port 80 configured in Azure NSG

---

## Problems Encountered

### SSH timeout

Cause

Port 22 was not reachable.

Solution

Verified NSG configuration and connected using the correct SSH key.

---

### Permission denied (publickey)

Cause

Incorrect private key or wrong file path.

Solution

Used the generated Azure SSH key and correct file location.

---

### Nginx not reachable

Cause

HTTP Port 80 was blocked.

Solution

Created an inbound NSG rule allowing TCP Port 80.

---

## Key Takeaways

- Azure networking is essential before deploying workloads.
- NSGs control traffic to Azure resources.
- SSH keys provide secure authentication.
- Linux administration is important when managing Azure VMs.
- A running VM alone is not enough; services must also be configured correctly.
- Testing connectivity is a critical part of troubleshooting.

---

## Overall Result

Successfully deployed:

- Resource Group
- Virtual Network
- Frontend Subnet
- Backend Subnet
- Azure Bastion Subnet
- Network Security Group
- Ubuntu Virtual Machine
- SSH Connection
- Nginx Web Server
- HTTP Access

Final Result:

A fully functional Linux web server running in Microsoft Azure and accessible through the public internet.
