# VLAN Design

## VLAN Overview

| VLAN | Name | Subnet | Purpose |
|---:|---|---|---|
| 10 | TRUSTED | 10.10.10.0/24 | Trusted endpoints |
| 20 | HOME | 10.10.20.0/24 | Personal Wi-Fi |
| 30 | SERVERS | 10.10.30.0/24 | Servers and NAS |
| 40 | IOT | 10.10.40.0/24 | IoT devices |
| 50 | LAB | 10.10.50.0/24 | Cybersecurity lab |
| 60 | GUEST | 10.10.60.0/24 | Guest network |
| 70 | DMZ | 10.10.70.0/24 | Public services |
| 99 | MANAGEMENT | 10.10.99.0/24 | Infrastructure management |

## VLAN 10 - TRUSTED

Used for trusted computers and administrative workstations.

Examples:

- Main PC
- Administration workstation
- Development workstation

Access:

```text
TRUSTED -> Internet      ALLOW
TRUSTED -> SERVERS       SELECTIVE
TRUSTED -> MANAGEMENT    SELECTIVE
TRUSTED -> LAB           SELECTIVE