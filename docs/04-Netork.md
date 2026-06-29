# Enterprise Network Design

## Overview

The Enterprise Homelab is divided into multiple network segments using VLANs and routed through a pfSense firewall.

The objective is to simulate the network architecture commonly found within enterprise environments.

---

# Network Segments

| Network    | Purpose                       |
| ---------- | ----------------------------- |
| Management | Infrastructure Management     |
| Servers    | Windows Server Infrastructure |
| Clients    | User Workstations             |
| Security   | Monitoring and Logging        |

---

# Core Services

Routing

* pfSense

Domain Services

* DC01
* DC02

Certificate Services

* CA01

Storage

* FS01

Automation

* Debian (Ansible)

Monitoring

* Wazuh

Clients

* Windows 11

---

# Design Goals

* Network segmentation
* Centralized authentication
* Secure administration
* Infrastructure automation
* Security monitoring
* Future scalability
