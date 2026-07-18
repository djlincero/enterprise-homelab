---

# 🤖 Infrastructure Automation

Infrastructure configuration and deployment are automated using **Ansible**, allowing consistent, repeatable provisioning across Linux and Windows systems.

## Automation Features

- Linux baseline configuration
- Windows Server baseline configuration
- Windows Exporter deployment
- Prometheus deployment and configuration
- Wazuh Agent deployment
- Service validation
- Connectivity testing
- Role-based Ansible architecture

### Repository Structure

```text
ansible/
├── inventory/
├── group_vars/
├── host_vars/
├── playbooks/
├── roles/
│   ├── node_exporter/
│   ├── prometheus/
│   ├── windows_exporter/
│   ├── wazuh/
│   └── linux_baseline/
└── site.yml
```

---

# 📊 Monitoring

The monitoring platform provides centralized visibility into both Windows and Linux infrastructure.

## Components

| Component | Purpose |
|----------|---------|
| Prometheus | Metrics collection |
| Node Exporter | Linux metrics |
| Windows Exporter | Windows metrics |
| Grafana | Dashboard visualization *(planned/current deployment)* |

### Metrics Collected

- CPU utilization
- Memory utilization
- Disk usage
- Network traffic
- Operating system metrics
- Windows performance counters
- Linux system metrics

---

# 🛡 Security Monitoring

Security monitoring is implemented using **Wazuh SIEM**.

## Security Features

- Endpoint monitoring
- Event collection
- Log analysis
- Security alerts
- Windows Event Logs
- Linux system logs
- Sysmon integration
- Agent management

---

# 📸 Project Gallery

## Infrastructure

> *(Insert Proxmox screenshot)*

## pfSense

> *(Insert Firewall / VLAN screenshot)*

## Active Directory

> *(Insert AD Users & Computers screenshot)*

## Certificate Authority

> *(Insert CA screenshot)*

## File Server

> *(Insert SMB/File Share screenshot)*

## Wazuh Dashboard

> *(Insert Wazuh Dashboard screenshot)*

## Prometheus

> *(Insert Prometheus Targets screenshot)*

## Grafana

> *(Insert Grafana Dashboard screenshot)*

## Ansible

> *(Insert successful Ansible playbook execution)*

---

# 💼 Skills Demonstrated

This project demonstrates practical experience with:

## Windows Administration

- Active Directory Domain Services
- Group Policy
- DNS
- Certificate Services (AD CS)
- SMB File Services
- Windows Administration

## Linux Administration

- Debian Server
- Systemd
- SSH
- Package Management
- Performance Monitoring

## Networking

- VLAN Design
- Routing
- Firewall Configuration
- DNS
- DHCP
- Network Segmentation

## Infrastructure Automation

- Ansible
- YAML
- Jinja2
- Role-Based Automation
- Infrastructure as Code

## Monitoring

- Prometheus
- Windows Exporter
- Node Exporter
- Metrics Collection
- Dashboard Integration

## Security

- Wazuh SIEM
- Endpoint Monitoring
- Security Event Analysis
- Log Collection

## Documentation

- Architecture documentation
- Deployment documentation
- Troubleshooting guides
- Network documentation
- Infrastructure diagrams

---

# 📖 Lessons Learned

Throughout this project I gained practical experience in:

- Designing enterprise network architectures
- Building a multi-server Active Directory environment
- Implementing enterprise PKI
- Automating infrastructure deployments using Ansible
- Deploying centralized monitoring across Windows and Linux
- Configuring SIEM-based security monitoring
- Troubleshooting enterprise services
- Creating professional technical documentation

---

# 🚀 Future Improvements

Planned enhancements include:

- Grafana dashboard provisioning with Ansible
- HTTPS for internal services
- Automated backups
- Prometheus Alertmanager
- Email alerting
- High Availability (HA) Proxmox cluster
- Additional Linux servers
- Containerized applications
- Kubernetes integration
- CI/CD pipeline automation

---

# 📂 Project Documentation

Detailed documentation is available in the `docs/` directory.

- Infrastructure deployment
- Network configuration
- Active Directory implementation
- Wazuh configuration
- Monitoring configuration
- Troubleshooting guides

---

# 👨‍💻 About the Author

This project was created as part of my professional systems administration portfolio to demonstrate hands-on experience with enterprise infrastructure, automation, monitoring, and security technologies.

**Core Technologies**

- Windows Server
- Active Directory
- Linux
- Proxmox VE
- pfSense
- Ansible
- Prometheus
- Wazuh
- Git & GitHub

---

# 📄 License

This project is licensed under the MIT License.

ZEMLAH!!!
