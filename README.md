# Raspberry Pi 5 Docker Homelab

A personal Linux infrastructure homelab built on a Raspberry Pi 5, focused on containerization, remote administration, network monitoring, and troubleshooting.

## Project Overview

This project documents my experience deploying and managing self-hosted services using Docker on Raspberry Pi OS. My goal is to develop practical Linux systems administration, networking, and infrastructure engineering skills.

## Hardware and Software

- Raspberry Pi 5 (4GB RAM)
- Raspberry Pi OS (64-bit)
- HighPi Pro 5S case
- Docker
- Uptime Kuma
- SSH
- Void Linux ThinkPad T480 (administration workstation)

## Architecture

```text
Void Linux ThinkPad
       |
       | SSH
       v
 Raspberry Pi 5
       |
       v
     Docker
       |
       v
   Uptime Kuma
       |
       v
 Router monitoring
```

## Implemented Features

### Remote Administration
- Configured headless Raspberry Pi OS
- Enabled SSH for remote administration
- Accessed the Raspberry Pi from a Linux workstation

### Containerization
- Installed Docker
- Deployed Uptime Kuma as a container
- Configured container port mapping
- Verified access to the monitoring dashboard

### Network Monitoring
- Configured Uptime Kuma to monitor router availability
- Verified connectivity and monitored uptime
## Screenshots

### Uptime Kuma monitoring dashboard

The dashboard displays the availability and uptime of my home router

![Uptime Kuma Dashboard](Screenshots/uptimekuma.png)

## Troubleshooting

During deployment, I investigated browser connection failures, container status, and incorrect port configurations. I corrected the Docker port mapping and successfully accessed Uptime Kuma through its web interface.

## Roadmap

- [x] Configure Raspberry Pi OS
- [x] Enable SSH access
- [x] Install Docker
- [x] Deploy Uptime Kuma
- [x] Monitor router availability
- [ ] Add Tailscale for remote access
- [ ] Deploy Pi-hole for DNS filtering
- [ ] Add more self-hosted services
- [ ] Document backups and recovery

## Lessons Learned

This project improved my understanding of Linux administration, Docker networking, service deployment, and systematic troubleshooting.

## Security

This repository contains documentation and example configurations only. Passwords, private keys, tokens, and other sensitive configuration values are excluded.

