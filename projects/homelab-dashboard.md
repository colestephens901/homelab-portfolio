# Homelab Dashboard

## Overview

This project documents the centralized dashboard used to organize and monitor my self-hosted homelab environment. The dashboard provides a single landing page for internal services, monitoring tools, infrastructure links, and frequently used administration resources.

The dashboard is built around a self-hosted Glance deployment and is designed to make the lab easier to manage at a glance.

## Purpose

The dashboard was created to solve a practical problem in the lab: as the number of self-hosted services grew, it became harder to keep track of what was running, where services were located, and which tools were used for monitoring, administration, and troubleshooting.

Instead of relying on browser bookmarks or manually remembering service URLs, the dashboard provides a clean central interface for daily use.

## Technologies Used

* Glance
* Docker
* Docker Compose
* Nginx Proxy Manager
* Internal DNS
* Reverse proxy routing
* Linux container hosting
* Service monitoring tools

## Dashboard Features

The dashboard includes organized sections for:

* Core infrastructure services
* Virtualization and storage management
* Monitoring and uptime tools
* Media services
* Home automation services
* Remote access tools
* Utility applications
* Documentation and project links

## Services Represented

The dashboard links to and organizes services such as:

* Proxmox VE
* TrueNAS
* Proxmox Backup Server
* OPNsense
* Home Assistant
* Jellyfin
* Immich
* Vaultwarden
* Uptime Kuma
* Beszel
* SearXNG
* Gotify
* Syncthing
* RustDesk
* Nginx Proxy Manager

## Infrastructure Role

The dashboard is hosted as part of the Docker-based services environment and is reverse proxied through Nginx Proxy Manager. It acts as the main entry point for managing the homelab and provides quick visibility into the systems and services that support the environment.

## Rack Display Usage

The dashboard is also used as the primary display for a dedicated server rack monitor. This allows infrastructure status and service links to be visible without needing to open a separate workstation or laptop.

## Skills Demonstrated

This project demonstrates:

* Self-hosted dashboard deployment
* Docker Compose service management
* Reverse proxy configuration
* Internal service organization
* Infrastructure documentation
* Homelab operations planning
* Practical monitoring workflow design

## Security Notes

Sensitive information such as internal IP addresses, domain names, credentials, API keys, and management URLs are intentionally excluded from this public documentation.
