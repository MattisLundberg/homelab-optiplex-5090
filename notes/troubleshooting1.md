# Troubleshooting: Slow boot

## Problem

Ubuntu took approximately 3 minutes to boot.

systemd-analyze blame showed:

systemd-networkd-wait-online.service
2min 36ms

## Cause

The Ethernet interface was configured as required,
but no Ethernet cable was connected.

The server was using Wi-Fi instead.

## Solution

Modified the Netplan configuration.

Added:

optional: true

to the Ethernet interface.

## Verification

Rebooted the server and checked:

systemd-analyze blame

The unnecessary delay was gone.
