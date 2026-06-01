# Real-Time Monitoring Dashboard using Prometheus & Grafana

## Overview

This project demonstrates a real-time infrastructure monitoring solution using AWS EC2, Prometheus, Node Exporter, and Grafana.

The dashboard provides visibility into:

* CPU Utilization
* Memory Usage
* Disk Usage
* Network Traffic
* System Load
* Server Health

---

## Architecture

```text
AWS EC2
   |
Node Exporter
   |
Prometheus
   |
Grafana Dashboard
```

---

## Technologies Used

* AWS EC2
* Ubuntu Linux
* Prometheus
* Grafana
* Node Exporter
* Git & GitHub

---

## Project Structure

```text
linux-monitoring-dashboard/
│
├── screenshots/
│   ├── dashboard.png
│   ├── prometheus.png
│   └── alerts.png
│
├── configs/
│   ├── prometheus.yml
│   └── node_exporter.service
│
└── README.md
```

---

## Installation Steps

### Install Node Exporter

```bash
sudo systemctl start node_exporter
```

### Install Prometheus

```bash
./prometheus --config.file=prometheus.yml
```

### Install Grafana

```bash
sudo systemctl start grafana-server
```

---

## Configure Prometheus Data Source

Grafana → Connections → Data Sources → Add Data Source

Select:

```text
Prometheus
```

URL:

```text
http://localhost:9090
```

Save & Test

---

## Import Dashboard

Dashboard ID:

```text
1860
```

Node Exporter Full Dashboard

---

## Alert Configuration

Example Alert:

```text
CPU Usage > 80%
Duration: 5 Minutes
```

Notification Channels:

* Email
* Slack
* Webhook

---

## Screenshots

### Dashboard

![Dashboard](screenshots/dashboard.png)

### Prometheus

![Prometheus](screenshots/prometheus.png)

### Alerts

![Alerts](screenshots/alerts.png)

---

## Skills Demonstrated

* Linux Administration
* Monitoring & Observability
* AWS Cloud
* Prometheus Monitoring
* Grafana Dashboarding
* DevOps Practices
* GitHub Documentation

---

## Resume Highlights

Built a real-time monitoring dashboard using Prometheus, Grafana, and Node Exporter on AWS EC2. Configured infrastructure monitoring, dashboard visualization, and automated alerting for CPU, memory, disk, and network metrics.

---

## Author

Sumit Kaulkar

