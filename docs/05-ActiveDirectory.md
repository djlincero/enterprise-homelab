# Active Directory Infrastructure

## Overview

Microsoft Active Directory Domain Services (AD DS) provides centralized identity management for the Enterprise Homelab.

The domain environment allows users, computers, and servers to authenticate using a centralized directory service while enabling administrators to manage resources through policies and permissions.

---

# Domain Information

| Property         | Value               |
| ---------------- | ------------------- |
| Domain Name      | myhomelab.local     |
| Forest           | Single Forest       |
| Domain           | Single Domain       |
| Functional Level | Windows Server 2022 |

---

# Domain Controllers

The environment contains two Domain Controllers.

| Server | Purpose                     |
| ------ | --------------------------- |
| DC01   | Primary Domain Controller   |
| DC02   | Secondary Domain Controller |

Responsibilities include:

* Authentication
* Authorization
* DNS
* Active Directory Replication
* Group Policy

---

# Organizational Units

The Active Directory structure is organized into logical Organizational Units (OUs).

Example:

```text
myhomelab.local

├── Servers
│
├── Workstations
│
├── Users
│
├── Groups
│
└── Service Accounts
```

---

# Authentication

Authentication is centralized using Active Directory.

Supported systems include:

* Windows Server
* Windows 11
* Administrative Accounts
* Service Accounts

---

# DNS Integration

Active Directory integrates with Microsoft DNS.

Responsibilities include:

* Name Resolution
* Dynamic DNS Updates
* SRV Records
* Domain Controller Discovery

---

# DHCP Integration

DHCP distributes IP addresses to domain clients while registering DNS records automatically.

---

# Group Policy

Group Policy provides centralized management for:

* Password Policies
* Security Settings
* Windows Configuration
* Administrative Templates

Future improvements include additional security baselines and workstation hardening.

---

# Enterprise Services

Active Directory supports:

* File Server Authentication
* Certificate Authority
* Windows Administration
* Remote Management
* Future Wazuh Integration

---

# Skills Demonstrated

This deployment demonstrates experience with:

* Active Directory Administration
* Domain Controller Deployment
* DNS Administration
* DHCP Administration
* Organizational Unit Design
* Authentication Management
* Group Policy

---

# Current Status

| Component          | Status        |
| ------------------ | ------------- |
| Active Directory   | ✅ Operational |
| DNS                | ✅ Operational |
| DHCP               | ✅ Operational |
| Authentication     | ✅ Operational |
| Domain Controllers | ✅ Operational |
| Group Policy       | 🚧 Expanding  |
| Replication        | ✅ Operational |

---

# Future Improvements

* Additional Group Policies
* Fine-Grained Password Policies
* LAPS
* Windows Admin Center
* Privileged Access Workstations
* Active Directory Certificate Services Enhancements
