# Lab 12 – Azure VM Troubleshooting

## Overview

This lab focused on troubleshooting and diagnosing Azure Virtual Machines using both the Azure Portal and Azure CLI.

Instead of deploying new infrastructure, the objective was to investigate the health, operational state, diagnostics, and activity history of an existing Azure Virtual Machine.

The lab demonstrates how Azure administrators can identify VM issues, verify deployment status, inspect resource health, review activity logs, and validate infrastructure using command-line tools.

---

## Objectives

During this lab I learned how to:

- Monitor Azure VM health
- Review Azure Resource Health
- Use Boot Diagnostics
- Analyze Azure Activity Logs
- Use Diagnose and Solve Problems
- Verify VM provisioning status
- Check VM power state
- Retrieve VM information using Azure CLI
- Inspect Public IP resources
- Combine Azure Portal and Azure CLI for troubleshooting

---

## Azure Services Used

- Azure Virtual Machines
- Azure Resource Health
- Azure Boot Diagnostics
- Azure Activity Log
- Azure Diagnose and Solve Problems
- Azure Cloud Shell
- Azure CLI
- Public IP Resources

---

## Screenshots

| Step | Description |
|-------|-------------|
| 01 | Virtual Machine Overview |
| 02 | Resource Health |
| 03 | Boot Diagnostics |
| 04 | Activity Log |
| 05 | Diagnose and Solve Problems |
| 06 | VM Instance View (Stopped) |
| 07 | VM Instance View (Running) |
| 08 | Azure CLI Public IP Resources |

---

## Azure CLI Commands

```bash
az vm get-instance-view \
--resource-group rg-lab-01_group \
--name rg-lab-01 \
--output table

az vm start \
--resource-group rg-lab-01_group \
--name rg-lab-01

az vm show \
--resource-group rg-lab-01_group \
--name rg-lab-01 \
--output table

az network public-ip list \
--resource-group rg-lab-01_group \
--output table
```

---

## Key Takeaways

This lab improved my understanding of Azure troubleshooting workflows.

I learned how administrators investigate the current health of virtual machines, verify deployment success, inspect activity logs, analyze boot diagnostics, and validate infrastructure through Azure CLI.

Although no production issues were intentionally introduced, the lab provided practical experience using the same troubleshooting tools that Azure administrators use in real environments.
