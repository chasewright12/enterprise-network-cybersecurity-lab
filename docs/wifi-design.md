# Wireless Network Design

## Access Point

The wireless access point connects to the Aruba CX 6100 using an 802.1Q trunk.

## SSIDs

| SSID | VLAN | Purpose |
|---|---:|---|
| HOME | 20 | Personal devices |
| IOT | 40 | IoT devices |
| LAB | 50 | Wireless lab |
| MANAGEMENT | 99 | AP management |

The exact native/untagged VLAN behavior depends on the access point vendor and configuration.

## HOME

Used for normal personal wireless clients.

```text
HOME
VLAN 20
10.10.20.0/24