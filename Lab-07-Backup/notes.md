# Lab 07 Notes

## Azure Recovery Services

Azure Recovery Services provides centralized backup and disaster recovery services for Azure resources.

Main purposes:

- Protect virtual machines
- Restore deleted or corrupted workloads
- Disaster Recovery
- Business Continuity
- Centralized backup management

---

# Recovery Services Vault

The Recovery Services Vault acts as the central management component.

It stores:

- Backup configuration
- Recovery points
- Backup policies
- Monitoring information
- Alerts
- Site Recovery configuration

---

# Backup Dashboard

The dashboard provides an overview of:

- Protected Items
- Backup Health
- Backup Storage
- Backup Jobs
- Warnings
- Critical Events

This gives administrators a quick health overview of backup operations.

---

# Backup Items

Backup Items represent resources currently protected by Azure Backup.

Examples:

- Azure Virtual Machines
- Azure Files
- SQL Databases
- SAP HANA
- Azure Backup Agent

Each protected workload appears as a Backup Item.

---

# Backup Policies

Backup Policies define how Azure performs backups.

A policy specifies:

- Backup Frequency
- Backup Time
- Retention Period
- Recovery Point Schedule

Multiple policies can exist simultaneously for different workloads.

---

# Backup Jobs

Backup Jobs show every executed backup operation.

Possible states:

- Completed
- Running
- Failed
- Cancelled
- In Progress

Administrators use Backup Jobs for troubleshooting.

---

# Backup Alerts

Alerts notify administrators about backup issues.

Examples:

- Failed Backup
- Missed Backup
- Warning
- Critical Event

Alerts allow quick response before data protection is compromised.

---

# Metrics

Azure Metrics provide operational monitoring.

Examples:

- Performance
- Throughput
- Resource Health
- Usage

Metrics can be visualized in Azure Monitor.

---

# Diagnostic Settings

Diagnostic Settings forward logs and metrics to:

- Log Analytics Workspace
- Azure Storage
- Event Hub

This enables long-term monitoring and auditing.

---

# Advisor Recommendations

Azure Advisor continuously analyzes Azure resources.

Recommendations include:

- Security Improvements
- Backup Best Practices
- High Availability
- Operational Excellence
- Cost Optimization

Following Advisor recommendations improves overall Azure reliability.

---

# Difference: Backup vs Site Recovery

Backup

- Protects data
- Allows file or VM restoration
- Focused on recovery after data loss

Site Recovery

- Protects entire workloads
- Replicates virtual machines
- Supports disaster recovery
- Used for failover between regions

---

# Key Takeaways

During this lab I learned:

- How Azure Backup is organized
- Why Recovery Services Vaults are required
- How backup policies control protection
- How backup monitoring works
- How Azure tracks backup jobs
- How alerts detect failures
- How metrics support monitoring
- How diagnostics integrate with Azure Monitor
- How Azure Advisor improves operational health
- Difference between Backup and Disaster Recovery

This lab provided a solid understanding of Azure Backup architecture and Recovery Services.
