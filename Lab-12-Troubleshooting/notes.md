# Lab 12 Notes

## Goal

The goal of this lab was to become familiar with Azure troubleshooting tools and understand where administrators investigate problems when virtual machines do not behave as expected.

Unlike deployment labs, this exercise focused on observation, diagnostics, monitoring, and verification.

---

# Resource Health

Resource Health provides information about the current availability of Azure resources.

It helps determine whether an issue is caused by:

- Microsoft Azure
- Customer configuration
- Planned maintenance
- Unexpected outages

This allows administrators to quickly identify if the problem is infrastructure-related or configuration-related.

---

# Boot Diagnostics

Boot Diagnostics captures the virtual machine boot process.

It provides:

- Boot screenshots
- Serial console logs
- Startup information

Boot Diagnostics is especially useful when a VM cannot be reached through SSH or RDP.

---

# Activity Log

The Activity Log records management operations performed on Azure resources.

Examples include:

- Start VM
- Stop VM
- Create Resource
- Delete Resource
- Update Configuration

The Activity Log allows administrators to determine:

- Who performed an action
- When it happened
- Whether the operation succeeded
- Which resource was affected

---

# Diagnose and Solve Problems

Azure provides automated troubleshooting through the Diagnose and Solve Problems feature.

This service analyzes Azure resources and recommends solutions for common issues.

Examples include:

- VM availability
- Networking issues
- Extension failures
- Performance problems
- Deployment issues

---

# VM Instance View

The Azure CLI command

```bash
az vm get-instance-view
```

provides runtime information that is not always immediately visible inside the Azure Portal.

Useful values include:

- Provisioning State
- Power State
- VM Agent status
- Extension status

Examples:

ProvisioningState = Succeeded

PowerState = VM running

PowerState = VM deallocated

---

# VM Information

Using

```bash
az vm show
```

I retrieved configuration details for the virtual machine.

This command is useful for verifying:

- Resource Group
- Location
- VM Name
- Operating System
- VM Size
- Azure Resource ID

---

# Public IP Resources

Using Azure CLI I listed the Public IP resources assigned within the Resource Group.

This allows administrators to verify:

- Public IP allocation
- Associated resources
- Provisioning status
- Public addresses

---

# Skills Practiced

- Azure troubleshooting
- VM diagnostics
- Resource Health analysis
- Activity Log investigation
- Boot Diagnostics
- Azure Portal navigation
- Azure CLI
- Cloud Shell
- Infrastructure validation

---

# What I Learned

During this lab I gained practical experience using Azure troubleshooting tools rather than deploying new resources.

I learned where Azure administrators investigate infrastructure problems and how to verify the operational state of virtual machines using both graphical and command-line interfaces.

Understanding Resource Health, Activity Logs, Boot Diagnostics, and Instance View gave me a better understanding of Azure operations and how administrators diagnose issues in production environments.

This lab also reinforced the importance of Azure CLI for quickly validating infrastructure without relying solely on the Azure Portal.
