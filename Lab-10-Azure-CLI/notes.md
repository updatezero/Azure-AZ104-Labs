# Azure CLI Notes

## What is Azure CLI?

Azure CLI (Command-Line Interface) is Microsoft's cross-platform command-line tool for managing Azure resources.

Instead of using the Azure Portal, administrators can automate and manage Azure directly from the terminal.

Azure CLI is available on:

- Windows
- macOS
- Linux
- Azure Cloud Shell

---

# Why use Azure CLI?

Advantages:

- Faster administration
- Automation
- Scripting
- Repeatable deployments
- Infrastructure as Code support
- Works locally and in Azure Cloud Shell

---

# Azure Cloud Shell

Azure Cloud Shell is a browser-based terminal provided by Microsoft.

Benefits:

- No installation required
- Already authenticated
- Azure CLI pre-installed
- PowerShell also available
- Accessible from anywhere

---

# Commands used

Show active Azure account

```bash
az account show
```

Displays:

- Subscription
- Tenant
- User
- State

---

List Resource Groups

```bash
az group list --output table
```

---

List Virtual Machines

```bash
az vm list --output table
```

---

List Virtual Networks

```bash
az network vnet list -g rg-lab-01_group --output table
```

---

List Storage Accounts

```bash
az storage account list -g rg-lab-01_group --output table
```

---

List Load Balancers

```bash
az network lb list -g rg-lab-01_group --output table
```

---

List Azure Bastion

```bash
az network bastion list -g rg-lab-01_group --output table
```

---

Show Azure CLI version

```bash
az version
```

---

# Output Formats

Azure CLI supports multiple output formats.

Default:

JSON

Common formats:

```bash
-o table
```

```bash
-o json
```

```bash
-o yaml
```

```bash
-o tsv
```

---

# Azure CLI Structure

Most commands follow this syntax:

```bash
az <service> <resource> <action>
```

Example:

```bash
az vm list
```

Meaning:

- az → Azure CLI
- vm → Virtual Machine
- list → Action

---

# Azure CLI vs Azure Portal

Azure Portal

- Graphical interface
- Beginner friendly
- Easy to navigate

Azure CLI

- Faster
- Better for automation
- Ideal for scripting
- Frequently used by Azure administrators

---

# What I learned

During this lab I learned:

- How Azure Cloud Shell works
- How Azure CLI authenticates automatically
- Azure CLI command structure
- How to query Azure resources
- How to filter resources using Resource Groups
- Different Azure CLI output formats
- Why Azure CLI is important for automation
- How Azure administrators use CLI in daily operations
- How Azure CLI complements the Azure Portal
- Basic Azure administration from the command line

---

# AZ-104 Knowledge

Important Azure CLI commands:

- az account
- az group
- az vm
- az network
- az storage
- az version

Azure CLI is one of the core administration tools required for the AZ-104 certification.
