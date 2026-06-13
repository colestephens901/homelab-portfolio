# Docker Services

This page documents the Docker-based services used in my personal homelab. Docker Compose is used to deploy and manage self-hosted applications for media, photo management, password management, budgeting, monitoring, local AI testing, and other infrastructure services.

Sensitive details such as internal IP addresses, domain names, credentials, API tokens, exact volume paths, and private configuration values are intentionally excluded.

## Purpose

The goal of this part of the homelab is to gain hands-on experience with application hosting and service management concepts, including:

* Docker Compose deployments
* Container networking
* Persistent storage
* Environment variables
* Reverse proxy configuration
* Service troubleshooting
* Application updates
* Permissions management
* Self-hosted infrastructure documentation

## Docker Compose Overview

Docker Compose is used to define and manage multi-container applications. This makes it easier to deploy services consistently, keep configurations organized, and troubleshoot individual services.

Skills practiced include:

* Writing and editing Compose files
* Managing container images
* Configuring environment variables
* Mapping volumes
* Managing container networks
* Restarting and updating services
* Reviewing logs for troubleshooting

## Example Services

The Docker environment includes several self-hosted applications used for practical learning and personal infrastructure.

Example services include:

* Immich for photo management
* Jellyfin for media streaming
* Passbolt for password management
* Actual Budget for budgeting
* Open WebUI and Ollama for local AI testing
* Monitoring and utility services
* Reverse proxy and access management tools

## Persistent Storage

Persistent storage is important because many containers need to keep configuration data, uploaded files, databases, or media libraries after container restarts and updates.

Storage-related skills practiced include:

* Mapping container volumes
* Separating application configuration from application images
* Using NAS-backed storage for selected services
* Troubleshooting file permissions
* Understanding user and group IDs
* Managing application data paths

## Networking

Docker networking is used to allow containers to communicate with each other and with other parts of the homelab.

Networking-related skills practiced include:

* Container network configuration
* Port mapping
* Internal service communication
* Troubleshooting service reachability
* Connecting Docker services to reverse proxy access
* Understanding how container ports differ from host ports

## Reverse Proxy Access

Some services are accessed through a reverse proxy using Nginx Proxy Manager and DNS configuration.

Reverse proxy-related skills practiced include:

* Routing friendly service names to internal applications
* Managing SSL certificates
* Configuring proxy hosts
* Troubleshooting HTTP and HTTPS access issues
* Separating internal-only services from services with controlled external access

## Updates and Maintenance

Docker services require regular maintenance to stay reliable and secure.

Maintenance tasks include:

* Reviewing container logs
* Updating images
* Restarting services after configuration changes
* Verifying service health
* Checking storage paths and permissions
* Backing up important configuration data
* Documenting changes and troubleshooting steps

## Troubleshooting Experience

Working with Docker services has helped me practice troubleshooting issues such as:

* Containers failing to start
* Incorrect environment variables
* Port conflicts
* Broken volume mappings
* File permission problems
* Services unable to access NAS-backed storage
* Reverse proxy misconfiguration
* DNS-related access issues
* Authentication and login problems
* Application updates causing configuration changes

## Skills Demonstrated

This project demonstrates hands-on experience with:

* Docker
* Docker Compose
* Linux server administration
* Container networking
* Persistent storage
* Environment variables
* Application hosting
* Reverse proxy configuration
* SSL certificate management
* Log review and troubleshooting
* Self-hosted service maintenance
* Infrastructure documentation

## What I Learned

Building and maintaining Docker-based services helped me better understand how modern applications are deployed, configured, updated, and troubleshot.

This project gave me practical experience with the same types of issues commonly seen in IT support and junior systems administration roles, including service availability, networking, storage access, configuration management, permissions, and log-based troubleshooting.
