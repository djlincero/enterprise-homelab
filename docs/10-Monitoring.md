# Phase 9 - Enterprise Monitoring

## Overview

This phase adds a complete enterprise monitoring solution to the homelab using Prometheus, Node Exporter, and Grafana.

The monitoring stack provides real-time visibility into the infrastructure and demonstrates modern observability practices commonly used in enterprise environments.

---

# Objectives

- Deploy Node Exporter
- Collect system metrics
- Deploy Prometheus
- Configure metric collection
- Deploy Grafana
- Build enterprise dashboards
- Monitor Linux infrastructure

---

# Monitoring Architecture

```
Node Exporter
        │
        │ Metrics
        ▼
Prometheus
        │
        │ Data Source
        ▼
Grafana
        │
        ▼
Enterprise Dashboards
```

---

# Node Exporter

Node Exporter was installed on the Debian monitoring server.

It exposes Linux system metrics through port **9100**.

Collected metrics include:

- CPU usage
- Memory usage
- Disk usage
- Filesystem usage
- Network traffic
- Load average
- System uptime
- Running processes

---

# Prometheus

Prometheus was deployed as the monitoring server.

Configuration file:

```
/etc/prometheus/prometheus.yml
```

Configured scrape targets:

- Prometheus
- Node Exporter

Scrape interval:

```
15 seconds
```

Prometheus Web Interface:

```
http://10.20.20.40:9090
```

---

# Grafana

Grafana was deployed for visualization and dashboard creation.

Web Interface:

```
http://10.20.20.40:3000
```

Datasource configured:

- Prometheus

---

# Dashboard

The **Node Exporter Full** dashboard was imported from Grafana.com.

Displayed metrics include:

- CPU utilization
- Memory utilization
- Filesystem utilization
- Disk I/O
- Network throughput
- Load average
- Uptime
- Running processes

---

# Results

The monitoring platform successfully provides real-time visibility into the Debian monitoring server.

Prometheus continuously collects metrics from Node Exporter while Grafana presents them through interactive dashboards suitable for enterprise infrastructure monitoring.

---

# Screenshots

## Prometheus

- 01-prometheus-home.png
- 02-prometheus-targets.png
- 03-prometheus-runtime.png

## Grafana

- 01-grafana-login.png
- 02-grafana-home.png
- 03-grafana-prometheus-datasource.png
- 04-node-exporter-dashboard.png
- 05-dashboard-cpu-memory.png
- 06-dashboard-filesystem-network.png

---

# Skills Demonstrated

- Linux Administration
- Infrastructure Monitoring
- Prometheus
- Grafana
- Node Exporter
- Metrics Collection
- Dashboard Design
- Enterprise Monitoring
- Observability
- Documentation
