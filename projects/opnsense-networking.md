# OPNsense Networking

This page documents the networking portion of my personal homelab. OPNsense is used as the primary firewall and router for network segmentation, DHCP, DNS-related routing, firewall rules, VPN access, and controlled access to internal services.

Sensitive details such as public IP addresses, private IP ranges, hostnames, credentials, API tokens, and exact firewall rule exports are intentionally excluded.

## Purpose

The goal of this part of the homelab is to gain hands-on experience with practical networking and firewall concepts, including:

* Firewall rule planning
* VLAN segmentation
* DHCP configuration
* DNS management
* VPN access
* Network isolation
* Internal service routing
* Troubleshooting client and service connectivity

## Network Overview

OPNsense sits at the edge of the network and handles routing between the internet, trusted devices, management systems, untrusted devices, and self-hosted infrastructure.

The network is designed to separate devices based on trust level and purpose.

## VLAN Design

The environment uses VLAN segmentation to separate different types of devices and services.

| VLAN    | Purpose         | Description                                                               |
| ------- | --------------- | ------------------------------------------------------------------------- |
| VLAN 10 | Management      | Used for infrastructure management and administrative access              |
| VLAN 20 | Trusted         | Used for servers, workstations, Proxmox, TrueNAS, and Docker services     |
| VLAN 30 | Untrusted / IoT | Used for wireless clients, smart home devices, and less trusted endpoints |

This design helps reduce unnecessary access between devices and keeps management interfaces separated from general client devices.

## Firewall Rules

Firewall rules are configured to control communication between VLANs and services.

The general approach is:

* Allow trusted devices to access required internal services
* Restrict untrusted or IoT devices from reaching management interfaces
* Allow only necessary traffic between VLANs
* Keep administrative access limited to trusted networks
* Avoid exposing internal management services directly to the public internet

This rule structure helps practice the principle of least privilege while still keeping the network usable.

## DHCP

DHCP is used to automatically provide network configuration to client devices and servers where appropriate.

DHCP-related skills practiced include:

* Creating DHCP scopes
* Managing static reservations
* Organizing devices by network segment
* Troubleshooting clients that fail to receive addresses
* Verifying gateway and DNS configuration

## DNS

DNS is used to make internal services easier to access and manage.

DNS-related skills practiced include:

* Internal DNS records and overrides
* Local service name resolution
* DNS troubleshooting
* Split internal and external service access planning
* Reducing reliance on memorizing IP addresses

## VPN Access

Remote access is handled through VPN access instead of exposing administrative interfaces directly to the internet.

The VPN setup allows private access to internal services while reducing unnecessary public exposure.

Skills practiced include:

* Remote access planning
* VPN routing
* Private service access
* Testing internal services from outside the local network
* Limiting access to trusted users and devices

## Internal Service Access

Several services are hosted internally or behind controlled access methods.

Examples include:

* Management interfaces
* Self-hosted applications
* Docker services
* NAS resources
* Monitoring tools
* Backup services

Access to these services is controlled using a combination of firewall rules, DNS, VPN access, and reverse proxy configuration where appropriate.

## Troubleshooting Experience

Working with OPNsense has helped me practice troubleshooting issues such as:

* Devices unable to reach the internet
* VLANs not passing traffic correctly
* Firewall rules blocking expected access
* DNS records resolving incorrectly
* DHCP reservations or leases not behaving as expected
* VPN routing issues
* Internal services reachable from one network but not another
* Reverse proxy and DNS-related access problems

## Skills Demonstrated

This project demonstrates hands-on experience with:

* OPNsense
* Firewall administration
* VLAN segmentation
* DHCP
* DNS
* VPN access
* Network isolation
* Internal routing
* Access control
* Troubleshooting
* Infrastructure documentation

## What I Learned

Building and maintaining this network helped me better understand how firewalls, VLANs, DHCP, DNS, VPN access, and internal routing work together in a real environment.

It also gave me practical troubleshooting experience that applies directly to IT support, network support, junior systems administration, and infrastructure-focused roles.
