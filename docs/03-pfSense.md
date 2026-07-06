# pfSense Firewall

## Overview

The pfSense virtual machine acts as the perimeter firewall and router for the Enterprise Homelab.

It provides network segmentation, routing, firewall protection, DNS forwarding, DHCP services (where applicable), and secure communication between all virtual networks.

---

# Objectives

The firewall was deployed to simulate a real enterprise edge device responsible for:

* Network segmentation
* Traffic filtering
* Static routing
* Gateway management
* DNS forwarding
* Internet connectivity

---

# Architecture

```text
                Internet
                     │
              Home Router
                     │
              Proxmox Host
                     │
                pfSense VM
                     │
 ┌─────────────┬──────────────┬──────────────┐
 │             │              │
Servers      Clients      Management
```

---

# Interfaces

| Interface | Purpose                       |
| --------- | ----------------------------- |
| WAN       | Internet connectivity         |
| LAN       | Internal enterprise network   |
| VLANs     | Segmented enterprise networks |

---

# Network Services

The firewall currently provides:

* IPv4 Routing
* Default Gateway
* Static Routes
* DNS Forwarding
* Firewall Policies
* VLAN Routing

---

# Firewall Responsibilities

The firewall protects:

* Active Directory
* Windows Servers
* Linux Servers
* Management Network
* Client Network

Only authorized traffic is allowed between network segments.

---

# Routing

The firewall performs routing between all internal enterprise networks.

Routing responsibilities include:

* Internal communication
* Internet access
* Inter-VLAN communication
* Static routes

---

# Security

Current security features include:

* Stateful Packet Inspection
* Firewall Rules
* Network Segmentation
* Gateway Monitoring

Future improvements:

* IDS/IPS
* VPN
* GeoIP Blocking
* High Availability

---

# Skills Demonstrated

This deployment demonstrates practical experience with:

* Enterprise Firewall Administration
* Routing
* Network Segmentation
* VLAN Configuration
* Traffic Control
* Network Security

---

# Current Status

| Component      | Status        |
| -------------- | ------------- |
| WAN            | ✅ Operational |
| LAN            | ✅ Operational |
| Routing        | ✅ Operational |
| Firewall Rules | ✅ Operational |
| DNS Forwarding | ✅ Operational |
| VLANs          | ✅ Operational |
| VPN            | 🚧 Planned    |
| IDS/IPS        | 🚧 Planned    |
