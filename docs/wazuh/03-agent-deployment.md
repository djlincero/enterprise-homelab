# Wazuh Agent Deployment

## Objective

Deploy and register Wazuh agents across Windows and Linux systems within the Enterprise Homelab.

---

# Managed Systems

| Agent ID | Hostname     | Operating System    | IP Address   |
| -------- | ------------ | ------------------- | ------------ |
| 001      | win11-client | Windows 11 Pro      | 10.30.30.10  |
| 002      | DC02         | Windows Server 2022 | 10.20.20.11  |
| 003      | fileserver   | Windows Server 2022 | 10.20.20.20  |
| 004      | DC01         | Windows Server 2022 | 10.20.20.10  |
| 005      | ca-server    | Windows Server 2022 | 10.20.20.30  |
| 006      | debian       | Debian 13           | 10.10.10.101 |

---

# Windows Deployment

Each Windows server was configured with:

* Wazuh Agent
* Wazuh Service
* Secure enrollment
* Automatic startup

Configuration included:

* Manager IP
* Agent registration
* Service validation

---

# Linux Deployment

The Debian workstation was configured using:

* Wazuh Agent
* Manager configuration
* Agent registration
* Service enablement

---

# Agent Registration

Agents were registered successfully using the Wazuh Manager.

Verification:

```bash
sudo /var/ossec/bin/manage_agents -l
```

---

# Active Agents

Communication was verified using:

```bash
sudo /var/ossec/bin/agent_control -lc
```

Output confirmed:

* All agents Active
* Connected to node01
* Healthy communication

---

# Dashboard Verification

The Wazuh Dashboard confirms:

* Six active agents
* Windows systems reporting
* Linux system reporting
* Agent versions
* Operating systems
* IP addresses

---

# Screenshots

Include:

* Active Agents Dashboard
* Agent Details
* manage_agents output
* agent_control output

---

# Result

All production systems in the homelab successfully report security events to the centralized Wazuh Manager.

This provides complete visibility across:

* Active Directory
* Windows Servers
* Windows Workstations
* Linux Systems

The environment is now ready for advanced security monitoring and threat detection.
