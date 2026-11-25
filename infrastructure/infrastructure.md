# Hardware Specifications

## System Overview

| Component | Specification |
|---|---|
| Manufacturer | Dell Inc. |
| Model | OptiPlex 5090 Micro |
| Form Factor | Micro |
| Product Family | Dell OptiPlex |
| Architecture | x86_64 |
| SMBIOS Version | 3.4 |

## CPU

| Component | Specification |
|---|---|
| Processor | Intel Core i5-10500T |
| Architecture | Comet Lake |
| Cores | 6 |
| Threads | 12 |
| Base Frequency | 2.30 GHz |
| Max Turbo Frequency | 3.80 GHz |
| L1 Cache | 384 KiB |
| L2 Cache | 1.5 MiB |
| L3 Cache | 12 MiB |
| Virtualization | Intel VT-x |

## Memory

| Component | Specification |
|---|---|
| Installed RAM | 32 GB |
| Available RAM (last check) | ~29 GB |
| Swap | 8 GB |

## Storage

| Device | Capacity | Purpose |
|---|---|---|
| nvme0n1 | 238.5 GB | Ubuntu installation |
| sda | 238.5 GB | Not yet identified |

### Partition Layout

| Partition | Size | Mount Point |
|---|---|---|
| nvme0n1p1 | 1 GB | /boot/efi |
| nvme0n1p2 | 237.4 GB | / |

## Networking

| Interface | Type | Purpose | Status |
|---|---|---|---|
| wlp0s20f3 | Wi-Fi | Primary network connection | Active |
| enp0s31f6 | Ethernet | Future wired connection | Unused |
| tailscale0 | VPN | Remote access | Active |

## Virtualization

- Intel VT-x supported.
- Hardware-assisted virtualization available.
- Suitable for KVM/QEMU virtualization.
- Potentially suitable for Proxmox VE.

## Intended Purpose

Dedicated homelab server for:

- Linux administration.
- Docker and containerization.
- Virtualization and virtual machines.
- Networking experiments.
- Self-hosted applications.
- Infrastructure and DevOps learning.
