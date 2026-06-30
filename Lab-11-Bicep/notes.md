# Notes – Lab 11

## Learning Objectives

This lab introduced Infrastructure as Code (IaC) and Microsoft's recommended language for Azure deployments: Azure Bicep.

Instead of manually deploying Azure resources through the Azure Portal, infrastructure can be described as code and deployed repeatedly, consistently and automatically.

---

# Infrastructure as Code (IaC)

Infrastructure as Code is the practice of managing cloud infrastructure using code instead of manual configuration.

Benefits include:

- Repeatable deployments
- Faster provisioning
- Reduced human errors
- Consistent environments
- Easier automation
- Version control using Git
- Better collaboration between administrators and developers

Examples of Infrastructure as Code tools include:

- Azure Bicep
- ARM Templates
- Terraform
- Ansible
- Pulumi

---

# Azure Resource Manager (ARM)

Azure Resource Manager (ARM) is Azure's deployment and management service.

ARM templates describe Azure resources using JSON.

Characteristics:

- Declarative language
- JSON format
- Supports complete infrastructure deployments
- Native Azure deployment technology
- Supports dependencies between resources

Examples of resources that can be deployed:

- Virtual Machines
- Storage Accounts
- Virtual Networks
- Network Security Groups
- Load Balancers
- Public IP Addresses
- Azure Bastion
- Azure Key Vault

---

# Azure Bicep

Azure Bicep is Microsoft's modern Infrastructure as Code language.

Instead of manually writing large ARM JSON files, Bicep provides a much cleaner syntax.

Bicep automatically compiles into ARM Templates before deployment.

Advantages:

- Easier to read
- Easier to maintain
- Smaller files
- Better readability
- Native Microsoft solution
- Fully supported by Azure
- Built-in validation
- IntelliSense support

---

# ARM Template vs Bicep

| ARM Template | Azure Bicep |
|--------------|-------------|
| JSON syntax | Bicep syntax |
| Verbose | Concise |
| Harder to read | Easier to read |
| More repetitive | Less repetitive |
| Native deployment format | Compiles into ARM JSON |
| Larger files | Smaller files |

---

# Azure CLI Commands Used

## Verify whether Bicep is installed

```bash
az bicep version
```

Purpose:

Checks whether the Azure Bicep CLI is installed and displays the installed version.

---

## Install Azure Bicep

```bash
az bicep install
```

Purpose:

Downloads and installs the latest Azure Bicep CLI into Azure Cloud Shell.

---

## List all available Bicep versions

```bash
az bicep list-versions
```

Purpose:

Displays every available version that Microsoft currently provides.

---

# Azure Cloud Shell

Azure Cloud Shell is a browser-based command-line environment hosted by Microsoft Azure.

Features:

- No local installation required
- Azure CLI pre-installed
- PowerShell available
- Bash available
- Direct authentication with Azure
- Accessible from any browser

---

# Template Editor

The Azure Template Editor allows administrators to create and edit ARM templates directly in the Azure Portal.

During this lab I:

- Opened the template editor
- Added a Storage Account resource
- Reviewed the generated JSON
- Explored template parameters
- Reviewed template variables
- Observed how Azure automatically generates ARM code

---

# Storage Account Template

After adding a Storage Account, Azure automatically generated:

- Parameters
- Variables
- Resource definitions
- API version
- Resource type
- Location
- Storage SKU
- Resource properties

This demonstrated how ARM templates describe Azure resources in JSON.

---

# What I Learned

During this lab I learned:

- What Infrastructure as Code is
- Why Infrastructure as Code is important
- The purpose of Azure Resource Manager
- The structure of ARM Templates
- The relationship between ARM Templates and Azure Bicep
- Why Bicep is Microsoft's recommended IaC language
- How Azure automatically generates ARM templates
- How to install Azure Bicep
- How to verify a Bicep installation
- How to list available Bicep versions
- How Azure Cloud Shell simplifies Azure administration
- How Azure CLI integrates with Azure Bicep

---

# Key Takeaways

- Infrastructure can be managed using code instead of manual deployment.
- ARM Templates are the native deployment format for Azure.
- Azure Bicep is a simplified language that compiles into ARM Templates.
- Azure CLI provides commands to install and manage the Bicep CLI.
- Azure Cloud Shell offers a ready-to-use environment for Azure administration without requiring local installations.
- Infrastructure as Code enables repeatable, consistent and automated Azure deployments.

---

# AZ-104 Skills Covered

- Azure Resource Manager
- Azure Bicep
- Infrastructure as Code
- ARM Templates
- Azure CLI
- Azure Cloud Shell
- JSON Templates
- Resource Deployment
- Storage Account Templates
- Deployment Automation
