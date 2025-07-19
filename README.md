# Monitoring Stack: Prometheus, Grafana, Alertmanager

## Overview

This project provides a complete monitoring stack using **Prometheus**, **Grafana**, **Alertmanager**, and **Node Exporter** — all orchestrated with Docker Compose.  
The stack is designed to collect, store, visualize, and alert on metrics from your infrastructure and applications.

## Architecture

- **Prometheus**: Collects and stores metrics from various targets.
- **Node Exporter**: Provides hardware and OS metrics from the host.
- **Alertmanager**: Handles alerts sent by Prometheus and notifies via configured channels.
- **Grafana**: Visualizes metrics and dashboards for real-time monitoring.

![Architecture](https://raw.githubusercontent.com/grafana/grafana/master/public/img/grafana_icon.svg)

## Features

- Out-of-the-box Docker Compose setup
- Pre-configured service discovery for Node Exporter
- Example Grafana dashboards
- Sample alert rules for Prometheus/Alertmanager
- Easy extension for your custom exporters

## How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/MikeTR312/monitoring-stack-prometheus-grafana.git
   cd monitoring-stack-prometheus-grafana

2.	Start the stack:	docker-compose up -d

3.  Access the services:
	•	Prometheus: http://localhost:9090
	•	Grafana: http://localhost:3000 (default login: admin / admin)
	•	Alertmanager: http://localhost:9093

Example Dashboards
	•	System metrics (CPU, RAM, Disk)
	•	Docker container monitoring
	•	Custom application metrics

 Customization
	•	Edit prometheus/prometheus.yml to add your targets/exporters.
	•	Configure alert rules in alertmanager/alertmanager.yml.
	•	Add new Grafana dashboards for your services.
