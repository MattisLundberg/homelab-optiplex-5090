# Networking

## Network interfaces

| Interface | Type | Purpose |
|---|---|---|
| wlp0s20f3 | Wi-Fi | Primary connection |
| enp0s31f6 | Ethernet | Future connection |
| tailscale0 | VPN | Remote access |

## IP addresses

- Local IP: DHCP assigned
- Tailscale IP: DHCP-like allocation by Tailscale

## Netplan

Ethernet interface is configured as optional
to prevent unnecessary boot delays.
