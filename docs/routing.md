# Routing Architecture

## Overview

Inter-VLAN routing is performed by the Palo Alto NGFW.

The Aruba CX 6100 transports VLAN traffic but does not act as the default gateway for the main security zones.

## Default Gateways

Each VLAN has a gateway on the Palo Alto firewall:

```text
VLAN 10 -> 10.10.10.1
VLAN 20 -> 10.10.20.1
VLAN 30 -> 10.10.30.1
VLAN 40 -> 10.10.40.1
VLAN 50 -> 10.10.50.1
VLAN 60 -> 10.10.60.1
VLAN 70 -> 10.10.70.1
VLAN 99 -> 10.10.99.1