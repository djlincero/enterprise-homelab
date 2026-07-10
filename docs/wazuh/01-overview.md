# Wazuh SIEM Deployment

## Project Overview

This project documents the deployment of a centralized Wazuh Security Information and Event Management (SIEM) platform within my Enterprise Homelab.

The objective is to build a realistic enterprise security environment capable of monitoring Windows and Linux systems, collecting security events, detecting suspicious activity, and providing centralized visibility across the infrastructure.

The SIEM serves as the security monitoring platform for the entire homelab and will later be integrated with Active Directory auditing, Sysmon, vulnerability detection, and attack simulations.

---

# Objectives

* Deploy an enterprise-grade SIEM solution.
* Centralize log collection from Windows and Linux systems.
* Monitor security events in real time.
* Prepare the environment for threat detection.
* Build a portfolio demonstrating enterprise security administration.

---

# Infrastructure

The Wazuh platform is integrated into the Enterprise Homelab built on Proxmox Virtual Environment.

## Virtualization

* Proxmox VE

## Firewall

* pfSense

## Active Directory

* Windows Server 2022 Domain Controller (DC01)
* Windows Server 2022 Domain Controller (DC02)

## Additional Servers

* Certificate Authority
* File Server

## Clients

* Windows 11
* Debian Linux

## Security Platform

* Wazuh Manager
* Wazuh Indexer
* Wazuh Dashboard

---

# Network Architecture

The homelab uses VLAN segmentation managed by pfSense.

| VLAN    | Purpose          |
| ------- | ---------------- |
| VLAN 10 | Management       |
| VLAN 20 | Servers          |
| VLAN 30 | Workstations     |
| VLAN 40 | DMZ              |
| VLAN 50 | Security (Wazuh) |

The Wazuh server resides in the dedicated Security VLAN to isolate monitoring services from production workloads.

---

# Connected Agents

The following systems are monitored by Wazuh:

* Windows 11 Client
* Domain Controller 01
* Domain Controller 02
* Certificate Authority Server
* File Server
* Debian Linux

All agents report successfully to the Wazuh Manager.

---

# Technologies

* Wazuh 4.14
* OpenSearch
* OpenSearch Dashboards
* Ubuntu Server
* Windows Server 2022
* Windows 11
* Debian 13
* pfSense
* Proxmox VE

---

# Current Status

✅ Wazuh Manager deployed

✅ OpenSearch Indexer operational

✅ Wazuh Dashboard operational

✅ Six agents enrolled

✅ Agents communicating successfully

✅ Centralized monitoring enabled

---

# Next Steps

The next phases of this project include:

* Dashboard customization
* Sysmon deployment
* Active Directory auditing
* Custom detection rules
* Vulnerability Detection
* MITRE ATT&CK mapping
* Attack simulation
* Incident response scenarios
