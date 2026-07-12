# Enterprise Network Architecture

## Overview

The Enterprise Homelab network was designed to simulate a small to medium-sized enterprise infrastructure. Network segmentation, routing, and centralized security are provided by pfSense running as a virtual firewall inside Proxmox.

The objective is to separate management, servers, and clients while maintaining secure communication between authorized systems.

---

# Network Design

The infrastructure consists of:

* Internet
* Home Router
* Proxmox Host
* pfSense Firewall
* Windows Servers
* Linux Servers
* Windows Clients

---

# Logical Architecture

```text
                    Internet
                         │
                  Home Router
                         │
                  Proxmox Server
                         │
                    pfSense VM
                         │
        ┌────────────────┼─────────────────┐
        │                │                 │
   Server Network   Client Network   Management
```

---

# Core Components

## Proxmox VE

Responsible for:

* Virtualization
* Virtual Networking
* Storage
* Resource Allocation

---

## pfSense

Responsible for:

* Routing
* Firewall
* DNS Forwarding
* Static Routes
* Gateway Management

---

## Windows Infrastructure

Provides:

* Active Directory
* DNS
* DHCP
* Certificate Authority
* File Services

---

## Linux Infrastructure

Provides:

* Automation
* SSH
* Ansible Controller

---

# Network Services

| Service          | Purpose               |
| ---------------- | --------------------- |
| DNS              | Name Resolution       |
| DHCP             | IP Address Assignment |
| Active Directory | Authentication        |
| WinRM            | Windows Automation    |
| SSH              | Linux Administration  |

---

# Security Model

Security is based on the following principles:

* Least Privilege
* Network Segmentation
* Firewall Policies
* Secure Remote Administration
* Centralized Authentication

---

# Current Environment

| Component        | Status        |
| ---------------- | ------------- |
| Internet Access  | ✅ Operational |
| Routing          | ✅ Operational |
| DNS              | ✅ Operational |
| DHCP             | ✅ Operational |
| Active Directory | ✅ Operational |
| WinRM            | ✅ Operational |
| SSH              | ✅ Operational |
| Ansible          | ✅ Operational |

---

# Future Improvements

* VPN Remote Access
* IDS/IPS
* Network Monitoring
* NetFlow
* High Availability Firewall
* Automated Configuration Backup
