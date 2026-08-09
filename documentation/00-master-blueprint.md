# Microsoft Entra ID Security Lab — Master Blueprint

## Project Overview

This project is a hands-on Microsoft Entra ID security lab designed to build practical skills in Identity and Access Management (IAM), authentication, authorization, Zero Trust, identity governance, security monitoring, detection engineering, and identity-focused security investigation.

The lab is designed from a Security Engineer / SOC perspective rather than as a purely theoretical Microsoft Entra administration exercise.

---

## Lab Objectives

The project aims to demonstrate practical implementation and investigation of:

- Microsoft Entra ID identity management
- Users and security groups
- Dynamic group membership
- Administrative Units
- Role-Based Access Control (RBAC)
- Privileged Identity Management (PIM)
- Authentication and MFA
- Conditional Access
- Identity Protection
- Application identities
- Service principals
- Managed identities
- Device identities
- External identities
- Identity Governance
- Access Reviews
- Entitlement Management
- Lifecycle Workflows
- Sign-in and Audit Logs
- Security monitoring
- Detection engineering
- Microsoft Graph
- PowerShell automation
- Identity security investigations

---

# Project Roadmap

| Phase | Area | Status |
|---|---|---|
| 1 | Identity Foundation | 🟡 In Progress |
| 2 | Authentication | ⬜ Not Started |
| 3 | Conditional Access | ⬜ Not Started |
| 4 | Identity Protection | ⬜ Not Started |
| 5 | RBAC & PIM | ⬜ Not Started |
| 6 | Applications & Workload Identity | ⬜ Not Started |
| 7 | Device Identity | ⬜ Not Started |
| 8 | External Identities | ⬜ Not Started |
| 9 | Identity Governance | ⬜ Not Started |
| 10 | Monitoring & Detection | ⬜ Not Started |
| 11 | Security Investigation | ⬜ Not Started |
| 12 | Microsoft Graph & Automation | ⬜ Not Started |
| 13 | Final Security Engineer Project | ⬜ Not Started |

---

# Phase 1 — Identity Foundation

## 1. Tenant & Directory Fundamentals

**Status:** ✅ Completed

Topics:

- Microsoft Entra tenant
- Directory structure
- Tenant configuration
- Licensing
- Security baseline
- Identity security principles

Documentation:

`01-tenant-setup.md`

---

## 2. Users

**Status:** 🟡 Lab Completed / Documentation In Progress

Topics:

- User creation
- User Principal Name (UPN)
- Object ID
- Member accounts
- Account status
- Department
- Employee ID
- Usage location
- User properties
- Group membership
- Assigned roles
- Assigned licenses
- Sign-in activity
- Password management

Documentation:

`02-users.md`

---

## 3. Security Groups

**Status:** 🟡 Lab Completed / Documentation In Progress

Topics:

- Security groups
- Assigned membership
- Group owners
- Group members
- Group purpose
- Group-based access control
- Group-based licensing
- Group organization

Documentation:

`03-groups.md`

---

## 4. Dynamic Groups

**Status:** 🟡 Lab Completed / Documentation In Progress

Topics:

- Dynamic membership
- Attribute-based membership
- Rule syntax
- Rule validation
- Positive validation
- Negative validation
- Troubleshooting overly broad rules

Example rule:

```text
(user.department -eq "Security")
and
(user.employeeId -startsWith "LAB")
