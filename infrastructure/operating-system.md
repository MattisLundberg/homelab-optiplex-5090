# Operating System

## General Information

| Property | Value |
|---|---|
| Operating System | Ubuntu Server |
| Version | 26.04.1 LTS |
| Codename | Resolute Raccoon |
| Architecture | x86_64 |
| Hostname | optiplex-5090 |
| Kernel | To be documented |
| Init System | systemd |

## System Configuration

### Remote Access

- OpenSSH Server installed.
- SSH enabled at boot.
- Tailscale installed.
- Tailscale enabled at boot.
- Server and laptop connected to the same Tailnet.
- MagicDNS used for hostname-based access.

### Networking

- Network manager: systemd-networkd.
- Primary connection: Wi-Fi.
- Ethernet interface: enp0s31f6.
- Wi-Fi interface: wlp0s20f3.
- Tailscale interface: tailscale0.
- Ethernet configured as optional in Netplan to prevent unnecessary boot delays.

### Power Management

- Sleep and hibernation disabled.
- BIOS AC Recovery: To be verified.
- Intended to run continuously as a headless server.

### Boot Configuration

- SSH automatically starts at boot.
- Tailscale automatically starts at boot.
- Ethernet does not block system startup.
- Server can be administered without a monitor, keyboard or mouse.

## Installed Software

| Software | Purpose |
|---|---|
| OpenSSH Server | Remote administration |
| Tailscale | Secure remote networking |
| Netplan | Network configuration |
| systemd | Service and system management |

## Network Access

### SSH

Connect to the server using:

    ssh mattis@optiplex-5090

SSH runs on the default port 22.

### Tailscale

Tailscale provides secure remote connectivity without requiring router port forwarding.

Useful commands:

    tailscale status
    tailscale ip -4
    tailscale ping optiplex-5090

## Maintenance

### Useful Commands

Check OS version:

    cat /etc/os-release

Check kernel version:

    uname -r

Check system uptime:

    uptime

Check boot performance:

    systemd-analyze

Check disk usage:

    df -h

Check running services:

    systemctl --type=service --state=running

Check Tailscale:

    tailscale status

Check SSH:

    sudo systemctl status ssh

## Future Plans

- Install Docker and Docker Compose.
- Set up container management.
- Experiment with self-hosted applications.
- Configure network-wide DNS.
- Experiment with virtualization.
- Set up system monitoring.
- Establish automated backups.
- Eventually transition to a wired Ethernet connection.
