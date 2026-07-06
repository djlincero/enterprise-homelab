# Proxmox Virtual Environment

## Overview

The enterprise homelab is hosted on a Proxmox Virtual Environment (VE) server that provides virtualization, networking, storage, and centralized management for all virtual machines.

Proxmox serves as the foundation of the infrastructure by hosting the Windows Server environment, Linux automation server, firewall appliance, and client operating systems.

---

# Objectives

The Proxmox environment provides:

* Centralized virtualization
* Enterprise networking
* Snapshot capability
* Resource management
* Rapid deployment of virtual machines
* Isolated testing environment

---

# Virtual Machine Inventory

| VM ID | Name                  | Operating System    | Purpose                     |
| ----: | --------------------- | ------------------- | --------------------------- |
|   100 | pfSense               | pfSense CE          | Firewall & Routing          |
|   101 | Debian Client         | Debian 13           | Linux Test Machine          |
|   102 | DC01                  | Windows Server 2022 | Primary Domain Controller   |
|   103 | DC02                  | Windows Server 2022 | Secondary Domain Controller |
|   104 | Windows 11            | Windows 11 Pro      | Domain Client               |
|   105 | File Server           | Windows Server 2022 | SMB File Services           |
|   106 | Certificate Authority | Windows Server 2022 | PKI Services                |
|   107 | Wazuh                 | Ubuntu Server       | SIEM Platform               |
|   109 | Debian Automation     | Debian 13           | Ansible Controller          |

---

# Infrastructure Components

The Proxmox server hosts the following enterprise services:

* Active Directory
* DNS
* DHCP
* Certificate Authority
* File Services
* Linux Automation
* Security Monitoring
* Client Operating Systems

---

# Networking

The virtual infrastructure is segmented using VLANs managed by pfSense.

Current logical networks include:

* Management Network
* Server Network
* Client Network
* Security Network

Routing between networks is performed by pfSense.

---

# Storage

The Proxmox storage subsystem provides:

* Virtual disks
* ISO image storage
* Snapshots
* Backup support

---

# Backup Strategy

Current backup strategy:

* Manual snapshots before major configuration changes
* VM cloning for testing
* Future automated backup implementation

---

# Administration

Primary administration tasks include:

* VM provisioning
* Resource allocation
* Snapshot management
* Network configuration
* Console access
* Performance monitoring

---

# Skills Demonstrated

This section demonstrates experience with:

* Enterprise Virtualization
* Hypervisor Administration
* Resource Planning
* Virtual Networking
* Infrastructure Design
* System Deployment
* Disaster Recovery Planning

---

# Current Status

| Component          | Status        |
| ------------------ | ------------- |
| Hypervisor         | ✅ Operational |
| Virtual Networking | ✅ Operational |
| VM Management      | ✅ Operational |
| Storage            | ✅ Operational |
| Snapshots          | ✅ Operational |
| Backup Strategy    | 🚧 Improving  |

---

## Future Improvements

* Automated VM backups
* Backup verification
* Resource monitoring
* High Availability research
* Template-based VM deployment
* Infrastructure as Code integration
