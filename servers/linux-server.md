# Linux Server

## Hostname

LINUX-SRV-01

## Operating System

Ubuntu Server 24.04 LTS

## Network

VLAN 40 - SERVERS

## IP Configuration

IP Address:
192.168.40.20/24

Gateway:
192.168.40.1

DNS:
192.168.40.10

## Services

- SSH
- Docker
- Nginx
- Monitoring Agent

## SSH

SSH access is restricted to the Management VLAN.

Management network:

192.168.10.0/24

## Firewall

UFW enabled.

Allowed:

SSH:
TCP/22

HTTP:
TCP/80

HTTPS:
TCP/443

All other inbound traffic:
DENY