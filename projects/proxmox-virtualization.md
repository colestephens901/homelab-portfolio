# Proxmox Virtualization

This page documents the virtualization portion of my personal homelab. Proxmox VE is used to host virtual machines and Linux containers for infrastructure services, application hosting, storage-related services, monitoring, and testing.

Sensitive details such as internal IP addresses, hostnames, public IP information, credentials, and exact management URLs are intentionally excluded.

## Purpose

The goal of this part of the homelab is to gain hands-on experience with real infrastructure concepts, including:

* Virtual machine management
* Linux container management
* Server resource allocation
* Network bridge configuration
* VLAN-aware networking
* Backup planning
* Service separation
* Infrastructure troubleshooting

## Environment Overview

The Proxmox environment is used to run multiple workloads across virtual machines and containers. Each workload is separated based on purpose so services can be managed, backed up, and troubleshot independently.

Example workload categories include:

* Firewall and networking services
* Docker application hosting
* Storage and backup services
* Monitoring tools
* Linux testing environments
* Self-hosted applications

## Virtual Machines and Containers

Proxmox allows me to run both full virtual machines and lightweight Linux containers.

### Virtual Machines

Virtual machines are used when I need stronger isolation, dedicated operating system environments, or services that benefit from a full VM setup.

Examples include:

* Linux server environments
* Application hosting systems
* Backup-related services
* Testing environments

### Linux Containers

Linux containers are used for lightweight services where a full virtual machine is not necessary.

Benefits include:

* Lower resource usage
* Faster deployment
* Easier service separation
* Simple backup and restore workflows

## Networking

Proxmox networking is connected into the larger homelab network. The environment supports segmented networking and infrastructure access through VLAN-aware configuration.

Skills practiced include:

* Linux bridge configuration
* VLAN-aware networking
* Static IP planning
* Service network separation
* Troubleshooting VM and container connectivity
* Verifying access between trusted networks and hosted services

## Storage

Storage for virtual machines, containers, and application data is planned around reliability and separation of responsibilities.

The environment uses NAS-backed storage for selected workloads and backup storage, while local storage may be used for operating system disks or test systems.

Skills practiced include:

* VM disk management
* Container storage management
* NAS-backed storage planning
* NFS mount troubleshooting
* Permissions troubleshooting
* Separating application data from system disks

## Backups

Backups are an important part of the Proxmox environment. Proxmox Backup Server is used to support backup workflows for virtual machines and containers.

Backup goals include:

* Protect important services from accidental data loss
* Practice backup scheduling
* Understand restore workflows
* Separate backups from primary service storage
* Build better infrastructure recovery habits

## Troubleshooting Experience

Working with Proxmox has helped me practice troubleshooting issues such as:

* VM and container network connectivity problems
* VLAN and bridge configuration issues
* Storage mount and permissions issues
* Resource allocation problems
* Service startup failures
* Backup and restore planning
* Linux configuration problems

## Skills Demonstrated

This project demonstrates hands-on experience with:

* Proxmox VE
* Virtual machines
* Linux containers
* Linux server administration
* Network bridge configuration
* VLAN-aware infrastructure
* Storage planning
* Backup workflows
* Troubleshooting
* Infrastructure documentation

## What I Learned

Building and maintaining this Proxmox environment helped me better understand how virtualization is used to separate services, manage resources, test configurations, and support reliable infrastructure.

It also gave me practical experience with the type of troubleshooting used in IT support and junior systems administration roles, especially when working with Linux systems, networking, storage, and hosted services.
