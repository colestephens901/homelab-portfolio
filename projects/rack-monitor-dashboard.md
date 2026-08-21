# Rack Monitor Dashboard

## Overview

This project documents the setup of a dedicated server rack dashboard display used to monitor and access homelab services at a glance. The goal was to repurpose existing hardware into a lightweight kiosk-style display for infrastructure visibility.

The display is designed to show the homelab dashboard continuously without requiring a full desktop workstation.

## Purpose

The rack monitor was created to provide a simple, always-visible view of the homelab environment. It helps make service status, monitoring links, and infrastructure tools easier to access while working near the rack.

This project also helps improve the physical presentation of the rack by turning an unused monitor into a functional dashboard display.

## Hardware Used

* Raspberry Pi 3
* Existing small monitor
* HDMI display connection
* Server rack or nearby monitor placement
* Existing network access to internal homelab services

## Software Used

* Debian Linux
* Xorg
* Openbox
* Chromium
* unclutter
* Glance dashboard
* Tailscale
* Pi-hole
* Linux systemd services

## Kiosk Configuration

The Raspberry Pi was configured as a lightweight Linux kiosk system. The setup uses a minimal graphical environment instead of a full desktop environment in order to reduce resource usage.

The kiosk environment includes:

* Xorg display server
* Openbox window manager
* Chromium launched in kiosk mode
* Cursor hiding with unclutter
* Disabled screen blanking
* Automatic dashboard launch on boot

## Dashboard Role

The rack monitor displays the homelab Glance dashboard, which acts as a centralized landing page for infrastructure tools, monitoring services, and commonly used self-hosted applications.

This allows quick access to:

* Service dashboards
* Monitoring tools
* Infrastructure management links
* Backup and storage tools
* Home automation systems
* Utility applications

## Performance Validation

The Raspberry Pi was tested to confirm it could handle the kiosk workload while continuing to perform its existing lightweight infrastructure roles.

Validation included:

* Checking memory usage while Chromium was running
* Monitoring CPU load
* Confirming display output and supported resolutions
* Checking thermal behavior
* Verifying stable operation under continuous dashboard display usage

## Skills Demonstrated

This project demonstrates:

* Linux system administration
* Lightweight kiosk configuration
* Raspberry Pi repurposing
* Display and resolution troubleshooting
* Service autostart configuration
* Resource monitoring
* Practical infrastructure visibility planning

## Security Notes

The dashboard is intended for internal homelab use. Sensitive information such as internal IP addresses, hostnames, credentials, API keys, and private management URLs are intentionally excluded from this public documentation.
