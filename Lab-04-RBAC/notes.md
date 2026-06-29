# Lab 04 – Azure Role-Based Access Control (RBAC)

## Objective

Understand and implement Azure Role-Based Access Control (RBAC) to manage permissions using built-in roles and the principle of least privilege.

---

## Business Scenario

Contoso Ltd. has hired a new infrastructure administrator who requires permission to manage virtual machines but should not have full administrative access to the Azure subscription.

As the Azure Administrator, the goal is to assign the appropriate Azure role while understanding scopes, inherited permissions and Azure RBAC best practices.

---

## Azure Resources

* Azure Subscription
* Resource Group
* Azure RBAC
* Access Control (IAM)
* Built-in Roles
* Role Assignments

---

## Lab Activities

During this lab the following tasks were completed:

* Explored Access Control (IAM)
* Reviewed current role assignments
* Verified inherited Owner permissions
* Assigned the Virtual Machine Contributor role
* Assigned the role to an Azure user
* Compared Subscription and Resource Group scopes
* Analysed permission inheritance
* Reviewed Azure built-in roles

---

## RBAC Built-in Roles

### Owner

Permissions:

* Full access to all Azure resources
* Can create, modify and delete resources
* Can assign Azure RBAC roles

Typical use:

* Azure Administrators
* Subscription Owners

---

### Contributor

Permissions:

* Can manage Azure resources
* Cannot assign Azure RBAC permissions

Typical use:

* Infrastructure Administrators
* Cloud Engineers

---

### Reader

Permissions:

* Read-only access
* Cannot modify resources

Typical use:

* Auditors
* Management
* Security Teams

---

### Virtual Machine Contributor

Permissions:

* Create Virtual Machines
* Modify Virtual Machines
* Start and Stop Virtual Machines
* Restart Virtual Machines

Cannot:

* Assign Azure roles
* Manage other Azure resources outside VM management

---

## Azure RBAC Scope Hierarchy

Azure permissions can be assigned at different scopes.

Hierarchy:

```text
Management Group
        │
Subscription
        │
Resource Group
        │
Azure Resource
```

Permissions assigned at higher levels are inherited by lower levels.

---

## Important Concepts

### Scope

Azure RBAC permissions can be assigned to:

* Management Groups
* Subscriptions
* Resource Groups
* Individual Resources

---

### Inheritance

Permissions assigned on a Subscription automatically flow down to:

* Resource Groups
* Virtual Machines
* Storage Accounts
* Virtual Networks

This reduces administration effort.

---

### Least Privilege Principle

Users should only receive the minimum permissions required to perform their job.

This reduces security risks and follows Microsoft's recommended best practices.

---

## AZ-104 Exam Notes

Important RBAC concepts for the AZ-104 exam:

* Built-in Roles
* Custom Roles
* Role Assignments
* Scope
* Permission Inheritance
* Least Privilege
* Azure IAM
* Access Control
* Management Groups
* Azure Governance

---

## Key Learnings

* Azure RBAC controls access to Azure resources.
* Azure IAM is used to manage role assignments.
* Permissions are assigned using built-in or custom roles.
* Higher-level permissions are inherited automatically.
* Virtual Machine Contributor provides VM management without full administrative rights.
* Owner can assign RBAC permissions.
* Least Privilege improves Azure security.
* Choosing the correct scope is an important design decision.

---

## Screenshots

* 01_IAM_Overview.png
* 02_View_My_Access.png
* 03_Role_Assignments.png
* 04_Virtual_Machine_Contributor_Assigned.png
* 05_Subscription_Owner_Role.png

---

## Lab Status

✅ Completed
