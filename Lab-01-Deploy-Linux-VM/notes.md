# Lab 01 Notes

## Environment

* Platform: Microsoft Azure
* Operating System: Ubuntu 24.04 LTS
* Authentication: SSH using an Ed25519 key pair
* User: azureuser

---

# Azure Deployment

The Linux virtual machine was successfully deployed in Microsoft Azure.

The deployment automatically created the following resources:

* Resource Group
* Virtual Machine
* Virtual Network (VNet)
* Subnet
* Network Security Group (NSG)
* Network Interface (NIC)
* Public IP Address
* Managed OS Disk
* SSH Key

SSH access is allowed through TCP port 22 using a Network Security Group rule.

---

# SSH Connection

The virtual machine was accessed securely using SSH.

Connection command:

```bash
ssh -i ~/.ssh/id_ed25519_azure azureuser@<Public-IP>
```

Authentication is performed using an Ed25519 SSH key pair instead of a password.

---

# Linux Commands

## hostname

Displays the hostname of the server.

Example:

```bash
hostname
```

Output:

```
rg-lab-01
```

---

## whoami

Displays the currently logged-in user.

Example:

```bash
whoami
```

Output:

```
azureuser
```

---

## pwd

Displays the current working directory.

Example:

```bash
pwd
```

Output:

```
/home/azureuser
```

---

## ls

Lists visible files and directories.

Example:

```bash
ls
```

---

## ls -la

Displays all files, including hidden files, together with permissions, owner, size and timestamps.

Example:

```bash
ls -la
```

Hidden files begin with a dot (`.`).

Examples:

* .bashrc
* .profile
* .cache
* .ssh

---

## ls -la ~/.ssh

Displays the contents of the user's SSH directory.

Example:

```bash
ls -la ~/.ssh
```

The directory contains the `authorized_keys` file, which stores the public keys that are allowed to connect to the server.

---

# Linux Root Directory

The Linux file system starts at the root directory:

```
/
```

Important directories:

| Directory | Description                             |
| --------- | --------------------------------------- |
| /home     | User home directories                   |
| /etc      | System configuration files              |
| /var      | Log files and variable application data |
| /tmp      | Temporary files                         |
| /usr      | Applications and libraries              |
| /root     | Home directory of the root user         |

---

# Current Progress

* Azure resources deployed
* VM successfully created
* SSH rule configured
* SSH key configured
* Successful SSH connection established
* Basic Linux commands completed
* Linux file system explored
