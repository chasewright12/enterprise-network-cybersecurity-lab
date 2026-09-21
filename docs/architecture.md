# Network Architecture

## Overview

The Enterprise Network & Cybersecurity Lab is a segmented network infrastructure designed to simulate an enterprise environment while providing an isolated cybersecurity testing platform.

The architecture combines:
- Palo Alto NGFW
- Aruba CX 6100 maganed switch
- Proxmox virtualization
- VLAN segmentation
- Wireless network segmentation
- Centralized security monitoring
- Network security monitoring
- Isolated penetration-test environment

## High-Level Architecture
```text
                          INTERNET
                              |
                           ONT/ONU
                              |
                            10GbE
                              |
                    +-------------------+
                    |   PALO ALTO       |
                    |      PA-440       |
                    |       NGFW        |
                    | Inter-VLAN Gateway|
                    +---------+---------+
                              |
                            10GbE
                              |
                    +-------------------+
                    |   ARUBA CX 6100   |
                    |   CORE SWITCH     |
                    +---------+---------+
                              |
        +---------------------+----------------------+
        |            |            |          |       |
       PC           NAS        Proxmox      AP    MikroTik
     VLAN 10      VLAN 30      TRUNK       TRUNK    LAB