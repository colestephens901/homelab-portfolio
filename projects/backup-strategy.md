# Backup Strategy

This page documents the backup strategy used in my personal homelab. The goal of this backup setup is to protect important virtual machines, containers, configuration data, and application storage while building practical experience with backup planning and recovery workflows.

Sensitive details such as internal IP addresses, hostnames, usernames, storage paths, credentials, and exact backup targets are intentionally excluded.

## Purpose

The goal of this part of the homelab is to gain hands-on experience with backup and recovery concepts, including:

* VM and container backups
* Backup scheduling
* NAS-backed backup storage
* Restore planning
* Storage separation
* Service recovery
* Disaster recovery fundamentals
* Infrastructure resiliency

## Backup Overview

The homelab uses Proxmox Backup Server and NAS-backed storage to support backup workflows for virtual machines and containers.

The backup strategy is designed around a few core ideas:

* Keep backups separate from primary workloads
* Back up important infrastructure services regularly
* Protect configuration data and application state
* Practice restore planning before failures happen
* Document backup processes clearly
* Avoid relying on a single system or storage location for important data

## Proxmox Backup Server

Proxmox Backup Server is used to manage backups for virtual machines and containers in the Proxmox environment.

Skills practiced include:

* Creating backup jobs
* Scheduling backups
* Managing backup storage
* Reviewing backup status
* Understanding retention policies
* Planning restore workflows
* Separating backup storage from active workloads

## NAS-Backed Backup Storage

TrueNAS provides storage used by backup-related workflows. This helps separate backups from the main virtualization host and provides centralized storage for recovery planning.

Skills practiced include:

* Backup storage planning
* NFS-backed storage concepts
* Storage permissions
* Dataset organization
* Backup destination management
* Troubleshooting access between backup systems and storage

## What Gets Backed Up

Important backup targets include:

* Virtual machines
* Linux containers
* Infrastructure services
* Application configuration data
* Selected Docker service data
* Important system configurations

Some large media libraries or replaceable data may be handled differently depending on size, importance, and recovery needs.

## Backup Planning

Backup planning includes deciding what data matters most, how often it should be backed up, and how quickly it would need to be restored after a failure.

Important questions include:

* Which services are critical?
* Which systems would be difficult to rebuild?
* Which data is replaceable?
* Which data would be difficult or impossible to replace?
* How long should backups be retained?
* Where should backups be stored?
* How would services be restored after a hardware or configuration failure?

## Restore Planning

Backups are only useful if they can be restored. Part of this project is understanding how restore workflows work and how services would be recovered after a failure.

Restore-related skills practiced include:

* Understanding VM and container restore options
* Planning recovery order for important services
* Verifying backup availability
* Separating application data from operating system disks
* Documenting recovery steps
* Thinking through failure scenarios before they happen

## Troubleshooting Experience

Working with backups has helped me practice troubleshooting issues such as:

* Failed backup jobs
* Storage destination access problems
* Permission issues
* Backup storage capacity concerns
* Network connectivity between systems
* Misconfigured backup schedules
* Restore planning gaps
* Services with data stored in unexpected locations

## Skills Demonstrated

This project demonstrates hands-on experience with:

* Proxmox Backup Server
* Backup scheduling
* VM backups
* Container backups
* NAS-backed storage
* TrueNAS
* NFS
* Storage permissions
* Recovery planning
* Infrastructure resiliency
* Documentation
* Troubleshooting

## What I Learned

Building a backup strategy helped me understand that reliable infrastructure is not just about keeping services running. It also requires planning for failure, protecting important data, testing recovery workflows, and documenting how systems should be restored.

This project gave me practical experience with backup and recovery concepts that apply directly to IT support, systems administration, and infrastructure roles.
