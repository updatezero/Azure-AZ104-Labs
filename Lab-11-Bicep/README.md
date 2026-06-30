# Lab 11 – Azure Bicep

## Overview

In this lab I explored Azure Bicep and Azure Resource Manager (ARM) templates. The objective was to understand Infrastructure as Code (IaC), learn the relationship between ARM templates and Bicep, and use Azure CLI to install and verify the Bicep CLI.

Unlike previous labs where resources were deployed manually through the Azure Portal, this lab introduced template-based deployments that allow Azure infrastructure to be described as code.

---

## Objectives

During this lab I completed the following tasks:

- Explored Azure Custom Deployment
- Opened the ARM Template editor
- Created a basic ARM deployment template
- Added a Storage Account resource to the template
- Reviewed automatically generated ARM JSON
- Learned how Azure Resource Manager templates work
- Installed the Azure Bicep CLI
- Verified the installed Bicep version
- Listed all available Bicep versions
- Compared ARM Templates with Azure Bicep

---

## Technologies Used

- Microsoft Azure
- Azure Resource Manager (ARM)
- Azure Bicep
- Azure CLI
- Azure Cloud Shell
- JSON
- Infrastructure as Code (IaC)

---

## Azure CLI Commands

### Check whether Bicep is installed

```bash
az bicep version
```

### Install Bicep

```bash
az bicep install
```

### Verify installation

```bash
az bicep version
```

### Show available versions

```bash
az bicep list-versions
```

---

## Screenshots

This lab contains screenshots demonstrating:

- Azure Custom Deployment
- ARM Template Editor
- Generated Storage Account template
- Initial Bicep version check
- Successful Bicep installation
- Installed Bicep version
- Available Bicep releases

---

## Skills Practiced

During this lab I practiced:

- Infrastructure as Code
- Azure Resource Manager
- ARM Templates
- Azure Bicep
- Azure Cloud Shell
- Azure CLI
- Template-based deployments
- Azure resource definitions
- Storage Account templates
- Azure deployment automation

---

## Result

Successfully created and explored an ARM template, added Azure resources through the template editor, installed Azure Bicep using Azure CLI, verified the installation and learned how Bicep simplifies Infrastructure as Code deployments within Azure.
