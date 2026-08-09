# Microsoft Entra ID Security Lab Architecture

## Overview

This document describes the architecture of the Microsoft Entra ID Security Lab.

The lab is designed to simulate a small organization's identity environment and demonstrate identity administration, authentication security, access control, application identity, security monitoring, and SOC investigation.

## High-Level Architecture

```text

                         Microsoft Entra ID
                              │
             ┌────────────────┼────────────────┐
             │                │                │
           Users            Groups          Devices
             │                │
             │                ├── Assigned Groups
             │                │
             │                └── Dynamic Groups
             │                         │
             │                  LAB-SECURITY-DYNAMIC
             │
             └───────────────┐
                             │
                    Administrative Unit
                             │
                      LAB-Security-AU
                             │
                     Scoped RBAC / PIM























                         Internet
                            |
                            v
                  +-------------------+
                  | Microsoft Entra ID|
                  +---------+---------+
                            |
          +-----------------+-----------------+
          |                 |                 |
          v                 v                 v
       Users             Groups         Applications
          |                 |                 |
          +-----------------+-----------------+
                            |
                            v
                  +-------------------+
                  | Conditional Access|
                  +---------+---------+
                            |
                            v
                    Identity Logs
                            |
                            v
                  +-------------------+
                  | Microsoft Sentinel|
                  +---------+---------+
                            |
                            v
                    SOC Investigation
                            |
                            v
                           KQL
