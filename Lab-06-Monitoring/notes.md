# Lab 06 – Azure Monitoring

## Objective

The objective of this lab was to explore Microsoft Azure Monitor and understand how Azure administrators monitor infrastructure, collect metrics, review logs, analyse changes and investigate resource health.

---

## Business Scenario

Contoso Ltd. has deployed several Azure resources including virtual machines, storage accounts and networking components. The IT department requires centralized monitoring to improve operational visibility, identify performance issues and proactively detect problems before they impact production.

As the Azure Administrator, the goal is to explore Azure Monitor and understand how monitoring, metrics and diagnostics work together.

---

## Azure Services Used

- Azure Monitor
- Activity Log
- Alerts
- Metrics
- Azure Virtual Machines
- Azure Monitor Logs
- Azure Monitor Workbooks
- Service Health
- Change Analysis
- Virtual Machine Insights
- Azure Managed Prometheus

---

## Lab Activities

During this lab I completed the following tasks:

- Opened Azure Monitor
- Explored the Azure Monitor dashboard
- Reviewed Azure Activity Logs
- Explored Azure Alerts
- Selected a monitoring scope
- Configured Metrics for a Virtual Machine
- Analysed CPU utilization using Percentage CPU metrics
- Reviewed Azure Monitor Logs
- Explored Azure Monitor Workbooks
- Reviewed Azure Service Health
- Explored Change Analysis
- Opened Azure VM Insights
- Reviewed Azure Managed Prometheus

---

## Important Concepts

### Azure Monitor

Azure Monitor is Microsoft's centralized monitoring platform used to collect, analyse and visualize telemetry from Azure resources.

---

### Activity Log

The Activity Log records management operations performed on Azure resources.

Examples:

- Resource creation
- Resource deletion
- RBAC changes
- Configuration changes

---

### Metrics

Metrics are numerical performance values collected over time.

Examples include:

- CPU Usage
- Network Traffic
- Disk Operations
- Memory Usage
- IOPS

Metrics can be visualized using charts and dashboards.

---

### Logs

Logs contain detailed operational data collected from Azure resources.

Logs are typically stored inside Log Analytics Workspaces and queried using KQL (Kusto Query Language).

---

### Alerts

Azure Alerts automatically notify administrators when configured conditions are met.

Examples:

- CPU above 90%
- VM unavailable
- Storage capacity exceeds threshold

---

### Workbooks

Azure Workbooks provide customizable dashboards combining metrics, logs and visualizations.

---

### Service Health

Service Health provides information about Azure platform incidents, planned maintenance and health advisories.

---

### Change Analysis

Change Analysis tracks configuration changes performed on Azure resources.

It helps administrators identify the root cause of infrastructure problems.

---

### Virtual Machine Insights

VM Insights provides detailed monitoring information including:

- Performance
- Dependencies
- Health
- Utilization

---

### Managed Prometheus

Azure Managed Prometheus collects and stores metrics from Kubernetes environments using Prometheus without requiring manual infrastructure management.

---

## AZ-104 Exam Notes

Important topics for the AZ-104 exam:

- Azure Monitor
- Activity Log
- Metrics
- Alerts
- Log Analytics
- Diagnostic Settings
- Azure Monitor Agent
- VM Insights
- Service Health
- Resource Health
- Workbooks
- KQL basics

---

## Key Learnings

- Azure Monitor centralizes monitoring across Azure resources.
- Activity Logs record management events.
- Metrics provide real-time performance information.
- Alerts automate monitoring and notifications.
- Workbooks simplify visualization of operational data.
- Service Health monitors Azure platform incidents.
- Change Analysis helps identify configuration changes.
- VM Insights provides advanced monitoring capabilities.
- Managed Prometheus simplifies Kubernetes monitoring.
- Monitoring is essential for maintaining highly available cloud environments.

---

## Screenshots

- 01-monitor-overview.png
- 02-activity-log.png
- 03-alerts.png
- 04-metrics-scope.png
- 05-metrics-selection.png
- 06-cpu-metric-chart.png
- 07-logs-overview.png
- 08-workbooks-overview.png
- 09-service-health.png
- 10-change-analysis.png
- 11-insights-virtual-machines.png
- 12-managed-prometheus.png

---

## Lab Status

✅ Completed
