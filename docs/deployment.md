# Deployment Guide

## Phase 1 — Physical Infrastructure

Install:

- ONT/ONU
- Palo Alto
- Aruba CX
- NAS
- Proxmox server
- Access Point
- MikroTik

Verify physical connectivity before configuring VLANs.

## Phase 2 — Palo Alto

Configure:

1. Management
2. WAN
3. LAN trunk
4. VLAN interfaces
5. Security zones
6. DHCP
7. NAT
8. Security policies
9. Logging

## Phase 3 — Aruba

Configure:

1. Management
2. VLAN database
3. Palo Alto trunk
4. Access ports
5. Proxmox trunk
6. AP trunk
7. MikroTik connection

## Phase 4 — Wireless

Create:

```text
HOME -> VLAN 20
IOT -> VLAN 40
LAB -> VLAN 50