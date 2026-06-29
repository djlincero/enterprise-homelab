# Enterprise Infrastructure Homelab

> A production-inspired enterprise infrastructure built with Proxmox, pfSense, Windows Server, Linux, Active Directory, Ansible, and Wazuh.

---

## Project Overview

This project simulates a small-to-medium enterprise environment to develop hands-on experience with systems administration, networking, cybersecurity, automation, and infrastructure documentation.

The lab is designed around real-world enterprise practices, including network segmentation, centralized identity management, infrastructure automation, and security monitoring.

---

## Technologies

### Virtualization

* Proxmox VE

### Networking

* pfSense
* VLANs
* DNS
* DHCP

### Windows Infrastructure

* Active Directory Domain Services
* Group Policy
* Enterprise Certificate Authority
* File Server

### Linux

* Debian 13
* OpenSSH

### Automation

* Ansible
* WinRM
* SSH

### Security

* Wazuh SIEM

---

## Current Infrastructure

| Server     | Purpose                          |
| ---------- | -------------------------------- |
| pfSense    | Firewall & Routing               |
| DC01       | Primary Domain Controller        |
| DC02       | Secondary Domain Controller      |
| FS01       | File Server                      |
| CA01       | Enterprise Certificate Authority |
| Debian     | Ansible Controller               |
| Windows 11 | Domain Workstation               |
| Wazuh      | Security Monitoring              |

---

## Project Structure

```text
enterprise-homelab/
├── ansible/
├── diagrams/
├── docs/
├── screenshots/
├── scripts/
└── website/
```

---

## Features

* Enterprise network segmentation
* Active Directory domain
* Centralized DNS and DHCP
* Enterprise PKI
* Infrastructure automation with Ansible
* Linux and Windows administration
* Security monitoring with Wazuh
* Professional documentation

---

## Project Status

Current Phase:

**Infrastructure Automation & Documentation**

Completed:

* Proxmox deployment
* pfSense configuration
* Active Directory
* Windows administration
* Linux administration
* WinRM configuration
* SSH configuration
* Ansible automation
* Git version control

Next Steps:

* Architecture diagrams
* Portfolio website
* Advanced Ansible roles
* Monitoring enhancements
* Backup automation

---

## Author

Zemlah

Enterprise Infrastructure Homelab Project
