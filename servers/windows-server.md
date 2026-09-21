# Windows Server

## Hostname

WIN-SRV-01

## Operating System

Windows Server 2022

## Role

Infrastructure Server

## Network

VLAN 40 - SERVERS

## IP Configuration

IP Address:
192.168.40.10

Subnet Mask:
255.255.255.0

Default Gateway:
192.168.40.1

DNS:
192.168.40.10

## Services

- Active Directory Domain Services
- DNS
- DHCP
- Group Policy

## Domain

lab.local

## DNS

Primary DNS:
192.168.40.10

Forwarders:
- 1.1.1.1
- 8.8.8.8

## Security

- Windows Defender Firewall enabled
- RDP restricted to Management VLAN
- Administrative accounts separated from normal user accounts
- Automatic security updates enabled