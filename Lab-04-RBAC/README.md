# Lab 04 – Azure Role-Based Access Control (RBAC)

## Overview

This lab focuses on Azure Role-Based Access Control (RBAC), one of the core identity and governance features of Microsoft Azure.

The objective is to understand how Azure permissions are assigned, inherited and managed using built-in roles while following the Principle of Least Privilege.

---

## Objectives

* Explore Azure Access Control (IAM)
* Understand Azure RBAC
* Review built-in Azure roles
* Assign the Virtual Machine Contributor role
* Understand permission inheritance
* Compare Subscription and Resource Group scopes
* Learn the Principle of Least Privilege
* Explore Azure role assignments

---

## Technologies

* Microsoft Azure
* Azure RBAC
* Azure IAM
* Azure Subscription
* Azure Resource Group
* Built-in Roles
* Azure Governance

---

## Azure Resources

* Azure Subscription
* Resource Group
* Azure RBAC
* Access Control (IAM)
* Role Assignments

---

## RBAC Architecture

```text
Management Group
        │
        ▼
Subscription
        │
        ▼
Resource Group
        │
        ▼
Azure Resources
(VMs, Storage, Networking...)
```

Permissions assigned at higher levels are automatically inherited by lower scopes.

---

## Screenshots

| Screenshot                                  | Description                                 |
| ------------------------------------------- | ------------------------------------------- |
| 01_IAM_Overview.png                         | Access Control (IAM) overview               |
| 02_View_My_Access.png                       | Current user permissions                    |
| 03_Role_Assignments.png                     | Existing Azure role assignments             |
| 04_Virtual_Machine_Contributor_Assigned.png | Virtual Machine Contributor role assignment |
| 05_Subscription_Owner_Role.png              | Owner role assigned at Subscription scope   |

---

## Skills Practiced

* Azure Role-Based Access Control (RBAC)
* Azure Identity and Access Management (IAM)
* Azure Governance
* Role Assignments
* Built-in Azure Roles
* Subscription Scope
* Resource Group Scope
* Permission Inheritance
* Principle of Least Privilege
* Azure Security Best Practices

---

## Key Learnings

* Azure RBAC controls authorization for Azure resources.
* Azure IAM provides centralized access management.
* Built-in roles simplify permission management.
* Permissions can be assigned at different scopes.
* Higher-level permissions are inherited automatically.
* Owner has full administrative permissions including RBAC management.
* Contributor can manage resources but cannot assign roles.
* Reader provides read-only access.
* Virtual Machine Contributor is limited to managing virtual machines.
* Least Privilege reduces security risks and follows Microsoft's recommended security model.

---

## Common AZ-104 Exam Topics

* Azure RBAC
* IAM
* Owner vs Contributor vs Reader
* Built-in vs Custom Roles
* Role Assignments
* Scope Hierarchy
* Permission Inheritance
* Least Privilege
* Azure Governance

---

## Status

**Completed** ✅

✔ Access Control (IAM) explored

✔ Current permissions reviewed

✔ Role assignments analysed

✔ Virtual Machine Contributor assigned

✔ Permission inheritance verified

✔ Subscription scope compared with Resource Group scope

✔ Lab documented

---

## Next Lab

**Lab 05 – Azure Virtual Machine Management**
