# Wazuh Installation

## Objective

Deploy a complete Wazuh SIEM platform capable of collecting logs from Windows and Linux endpoints and providing centralized monitoring.

---

# Server Information

| Component        | Value                   |
| ---------------- | ----------------------- |
| Operating System | Ubuntu Server 24.04 LTS |
| Hostname         | wazuh-siem              |
| IP Address       | 10.50.50.10             |
| VLAN             | Security (VLAN 50)      |

---

# Installed Components

The deployment includes:

* Wazuh Manager
* Wazuh Indexer
* Wazuh Dashboard
* OpenSearch
* OpenSearch Dashboards

---

# Installation Process

The installation was completed using the official Wazuh installation assistant.

The deployment automatically configured:

* TLS certificates
* OpenSearch
* Dashboard
* Wazuh Manager
* API
* Internal communication

---

# Service Verification

After installation the following services were verified:

| Service         | Status  |
| --------------- | ------- |
| Wazuh Manager   | Running |
| Wazuh Indexer   | Running |
| Wazuh Dashboard | Running |
| Wazuh API       | Running |

Example verification:

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

---

# Indexer Authentication

The default administrator password was replaced with a strong custom password using the Wazuh password management tool.

Connectivity was verified using:

```bash
curl -k -u admin:<password> https://127.0.0.1:9200
```

Successful authentication confirmed that the OpenSearch Indexer was operational.

---

# Screenshots

The following screenshots demonstrate the deployment:

* Login page
* Dashboard overview
* Running services
* Agent status
* Indexer connectivity

---

# Result

The SIEM platform is fully operational and ready to receive logs from Windows and Linux agents.
