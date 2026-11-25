# Homelab Changelog

This file documents significant changes, additions and modifications to the homelab infrastructure.

## 2026-11-25 – Initial Setup

### Hardware
- Set up Dell OptiPlex 5090 Micro as the primary homelab server.
- Intel Core i5-10500T CPU (6 cores / 12 threads).
- 32 GB RAM.
- Approximately 240 GB NVMe storage.

### Operating System
- Installed Ubuntu Server 26.04.1 LTS.
- Changed system hostname to optiplex-5090.
- Configured the machine for headless operation.

### Networking
- Configured Wi-Fi as the primary network connection.
- Identified Ethernet interface as enp0s31f6.
- Configured Ethernet as optional in Netplan to prevent unnecessary boot delays.
- Installed Tailscale for secure remote connectivity.
- Connected server and Ubuntu laptop to the same Tailnet.

### Remote Access
- Installed OpenSSH Server.
- Enabled SSH at boot.
- Enabled Tailscale at boot.
- Verified remote SSH access through Tailscale.
- Verified connectivity after reboot.

### System Administration
- Configured SSH and Tailscale to start automatically.
- Disabled sleep and hibernation.
- Investigated BIOS automatic power recovery settings.
- Resolved slow boot caused by network-online waiting for an unavailable Ethernet connection.

### Documentation
- Created initial homelab documentation structure.
- Documented hardware specifications.
- Documented operating system configuration.
