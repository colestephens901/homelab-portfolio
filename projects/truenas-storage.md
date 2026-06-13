# TrueNAS Storage

This page documents the storage portion of my personal homelab. TrueNAS is used to provide NAS-backed storage for application data, media, backups, and shared storage across the environment.

Sensitive details such as internal IP addresses, hostnames, usernames, dataset paths, credentials, and exact share names are intentionally excluded.

## Purpose

The goal of this part of the homelab is to gain hands-on experience with storage administration concepts, including:

* NAS management
* ZFS storage concepts
* Dataset organization
* NFS shares
* Storage permissions
* Application storage mounts
* Backup storage planning
* Storage troubleshooting

## Storage Overview

TrueNAS provides centralized storage for different services in the homelab. This allows application data, media files, and backup storage to be separated from individual virtual machines and containers.

Centralized storage helps make services easier to manage, back up, migrate, and troubleshoot.

## ZFS

The storage environment uses ZFS for managing storage pools and datasets.

Skills practiced include:

* Understanding storage pools
* Organizing datasets by purpose
* Planning storage layout
* Managing storage usage
* Understanding redundancy concepts
* Separating application data from general file storage

## Dataset Organization

Datasets are organized based on the type of data or service using them.

Example dataset categories include:

* Application configuration data
* Media storage
* Photo storage
* Backup storage
* Shared service data

This organization helps keep data separated, easier to manage, and easier to troubleshoot.

## NFS Shares

NFS shares are used to provide storage access to Linux systems, Docker hosts, and other infrastructure services.

Skills practiced include:

* Creating NFS shares
* Mounting NFS shares from Linux systems
* Connecting application storage to NAS-backed paths
* Verifying share access
* Troubleshooting mount issues
* Managing access between servers and storage

## Permissions

Storage permissions are an important part of the environment because many self-hosted services depend on correct access to mounted data.

Troubleshooting permissions has helped me better understand:

* Linux file ownership
* User and group IDs
* Docker container permissions
* Read/write access issues
* NFS permission behavior
* Application access to mounted storage

## Application Storage

Several self-hosted services use NAS-backed storage for media, photos, application data, or backups.

Example use cases include:

* Media storage for Jellyfin
* Photo storage for Immich
* Application data for Docker services
* Backup storage for infrastructure workloads
* Shared storage between virtualized systems

## Backup Storage

TrueNAS also supports backup workflows by providing storage for backups and recovery planning.

Backup-related skills practiced include:

* Separating backup storage from primary service storage
* Planning backup destinations
* Supporting Proxmox Backup Server storage
* Understanding restore planning
* Protecting important infrastructure data

## Troubleshooting Experience

Working with TrueNAS has helped me practice troubleshooting issues such as:

* NFS shares not mounting correctly
* Services unable to read or write to mounted storage
* Incorrect file ownership or permissions
* Docker containers unable to access NAS-backed paths
* Storage paths not matching application expectations
* Backup storage access issues
* Media or photo services not detecting files correctly

## Skills Demonstrated

This project demonstrates hands-on experience with:

* TrueNAS
* NAS administration
* ZFS
* NFS
* Dataset organization
* Linux storage mounts
* Docker storage mapping
* File permissions
* Backup storage planning
* Storage troubleshooting
* Infrastructure documentation

## What I Learned

Building and maintaining NAS-backed storage helped me understand how important storage planning is for reliable infrastructure.

This project gave me practical experience connecting Linux systems, Docker services, virtualized workloads, media applications, photo management tools, and backup systems to centralized storage.
