# Enterprise Certificate Authority

## Overview

The Enterprise Homelab includes Microsoft Active Directory Certificate Services (AD CS) to provide a Public Key Infrastructure (PKI) for the domain.

The Certificate Authority issues and manages digital certificates used for authentication, encryption, and secure communication between enterprise systems.

---

# Objectives

The Certificate Authority was deployed to:

* Build an internal Public Key Infrastructure (PKI)
* Issue certificates to domain computers
* Secure Windows services
* Support encrypted communications
* Prepare the environment for future VPN and web services

---

# Server Information

| Server | Role                                  |
| ------ | ------------------------------------- |
| CA01   | Enterprise Root Certificate Authority |

---

# Certificate Services

Current services include:

* Enterprise Root CA
* Certificate Enrollment
* Certificate Management
* Trusted Root Distribution

---

# Integration

The Certificate Authority integrates with:

* Active Directory
* Domain Controllers
* Windows Clients
* File Server
* Future IIS Servers
* Future VPN Services

---

# Enterprise Benefits

Implementing PKI provides:

* Secure authentication
* Digital identity
* Encrypted communications
* Certificate-based trust
* Centralized certificate management

---

# Future Certificate Usage

Planned certificate deployments include:

* HTTPS Web Servers
* WinRM over HTTPS
* VPN Authentication
* Code Signing
* RDP Certificates
* User Certificates

---

# Security

Security considerations include:

* Private key protection
* Certificate expiration management
* Certificate revocation
* Backup of the Certificate Authority database

---

# Skills Demonstrated

This deployment demonstrates practical experience with:

* Microsoft PKI
* Active Directory Certificate Services
* Enterprise Certificate Management
* Windows Security
* Infrastructure Hardening

---

# Current Status

| Component                 | Status        |
| ------------------------- | ------------- |
| Enterprise Root CA        | ✅ Operational |
| AD Integration            | ✅ Operational |
| Certificate Enrollment    | ✅ Operational |
| Trusted Root Distribution | ✅ Operational |
| HTTPS Certificates        | 🚧 Planned    |
| VPN Certificates          | 🚧 Planned    |

---

# Future Improvements

* Automatic Certificate Enrollment
* Web Server Certificates
* Certificate Templates
* Smart Card Authentication Research
* Certificate Lifecycle Automation
