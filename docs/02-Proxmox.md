# Proxmox Virtual Environment

## Overview

The Enterprise Infrastructure Homelab is hosted on a single Proxmox VE server.

Proxmox provides the virtualization platform used to host all Windows and Linux virtual machines while offering centralized management, snapshots, networking, and storage.

---

# Hypervisor

Platform:

* Proxmox Virtual Environment (PVE)

Primary Functions:

* Virtual Machine Management
* Virtual Networking
* Storage Management
* Snapshots
* ISO Management
* Backup Support

---

# Virtual Machines

Current infrastructure includes:

| VM         | Purpose                            |
| ---------- | ---------------------------------- |
| pfSense    | Firewall and Routing               |
| DC01       | Active Directory Domain Controller |
| DC02       | Secondary Domain Controller        |
| FS01       | File Server                        |
| CA01       | Enterprise Certificate Authority   |
| Debian     | Ansible Controller                 |
| Windows 11 | Domain Workstation                 |
| Wazuh      | Security Monitoring                |

---

# Virtual Networking

The Proxmox host provides virtual networking between all infrastructure components.

Network segmentation is implemented using VLANs configured on pfSense.

---

# Administration

Primary administration is performed through:

* Proxmox Web Interface
* SSH
* Ansible

---

# Future Improvements

Planned enhancements include:

* Automated backups
* Template virtual machines
* Snapshot management
* High Availability research
* Storage optimization
