# Palo Alto Firewall - Interfaces

## Physical Interfaces

| Interface | Purpose | Zone |
|---|---|---|
| ethernet1/1 | WAN / Internet | untrust |
| ethernet1/2 | LAN Trunk | trust |
| ethernet1/3 | DMZ | dmz |
| ethernet1/4 | Management | management |

## VLAN Interfaces

| Interface | VLAN | IP Address |
|---|---:|---|
| ethernet1/2.10 | 10 | 192.168.10.1/24 |
| ethernet1/2.20 | 20 | 192.168.20.1/24 |
| ethernet1/2.30 | 30 | 192.168.30.1/24 |
| ethernet1/2.40 | 40 | 192.168.40.1/24 |
| ethernet1/2.50 | 50 | 192.168.50.1/24 |