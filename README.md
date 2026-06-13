# Personal Infrastructure Homelab

This repository documents my personal homelab environment, built to develop hands-on experience with IT support, networking, systems administration, virtualization, Linux, storage, backups, and self-hosted services.

The goal of this project is to demonstrate practical infrastructure skills that apply to IT Support, Junior Systems Administrator, Network Technician, and infrastructure-focused roles.

## Overview

My homelab includes a segmented network, virtualized server environment, NAS-backed storage, Docker-based services, VPN access, reverse proxying, DNS management, and backup workflows.

Core technologies include:

* Proxmox VE
* TrueNAS
* OPNsense
* Debian and Ubuntu Linux
* Docker Compose
* Cloudflare DNS
* Nginx Proxy Manager
* Tailscale
* ZFS
* NFS
* Proxmox Backup Server

## Project Goals

* Build practical experience with real infrastructure tools
* Learn virtualization, Linux, networking, and storage administration
* Practice troubleshooting service, networking, permissions, and access issues
* Document infrastructure clearly and professionally
* Build a public technical portfolio for IT career growth

## Infrastructure Areas

### Virtualization

The environment uses Proxmox VE to run virtual machines and Linux containers for networking, storage, application hosting, and infrastructure services.

Skills demonstrated:

* VM and container management
* Resource allocation
* Linux server deployment
* Service separation
* Backup planning

### Networking

The network is managed using OPNsense with segmented VLANs for different device groups and access levels.

Skills demonstrated:

* Firewall rules
* VLAN segmentation
* DHCP and DNS management
* VPN access
* Internal routing
* Client and service isolation

### Storage

Storage is handled through TrueNAS using ZFS and NFS shares for application data, media, and backup storage.

Skills demonstrated:

* NAS administration
* ZFS storage concepts
* NFS share configuration
* Dataset permissions
* Application storage mounts

### Docker Services

Several self-hosted services are deployed using Docker Compose.

Example services include:

* Immich for photo management
* Jellyfin for media streaming
* Passbolt for password management
* Open WebUI and Ollama for local AI testing
* Monitoring and utility services

Skills demonstrated:

* Docker Compose
* Container networking
* Volume mapping
* Environment variables
* Service troubleshooting
* Reverse proxy configuration

### Reverse Proxy and DNS

Cloudflare DNS and Nginx Proxy Manager are used for DNS management, SSL certificates, reverse proxying, and controlled service access.

Skills demonstrated:

* DNS records
* SSL certificate management
* Reverse proxy configuration
* Internal vs. external access planning
* Service access control

### Backups

Backup workflows are built around Proxmox Backup Server and NAS-backed storage.

Skills demonstrated:

* VM and container backups
* Backup storage planning
* Restore planning
* Infrastructure resiliency

## Planned Documentation

* Network diagram
* VLAN overview
* Proxmox layout
* TrueNAS storage overview
* Docker Compose service stack
* Backup strategy
* Troubleshooting notes
* Security considerations

## Security Notes

This public documentation intentionally avoids exposing sensitive information such as public IP addresses, private keys, API tokens, credentials, exact firewall rules, internal hostnames, and administrative dashboards.
