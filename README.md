# Microsoft Entra ID Security Lab

A hands-on Microsoft Entra ID security laboratory focused on Identity and Access Management (IAM), Role-Based Access Control (RBAC), Multifactor Authentication (MFA), Conditional Access, application identity, identity monitoring, detection engineering, and Microsoft Sentinel integration.

## Project Objectives

This lab is designed to demonstrate practical implementation and security investigation using Microsoft Entra ID.

The project covers:

- Identity and Access Management (IAM)
- Users and Security Groups
- Role-Based Access Control (RBAC)
- Multifactor Authentication (MFA)
- Conditional Access
- Authentication Methods
- Application Registrations
- Enterprise Applications
- Service Principals
- Microsoft Graph
- Identity and Audit Logs
- Identity Protection
- Security Monitoring
- Detection Engineering
- Microsoft Sentinel Integration
- KQL-based Investigation

## Lab Architecture

```text
                    Internet
                       |
                       v
              +------------------+
              | Microsoft Entra  |
              |       ID         |
              +--------+---------+
                       |
        +--------------+--------------+
        |              |              |
        v              v              v
      Users          Groups       Applications
        |              |              |
        +--------------+--------------+
                       |
                       v
              Conditional Access
                       |
                       v
                 Identity Logs
                       |
                       v
              Microsoft Sentinel
                       |
                       v
                SOC Investigation
                       |
                       v
                      KQL
