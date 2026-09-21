# DNS Server

## Hostname

DNS-SRV-01

## Operating System

Ubuntu Server 24.04 LTS

## Role

Internal DNS Resolver and Authoritative DNS Server

## Network

VLAN 40 - SERVERS

## IP Configuration

IP Address:
192.168.40.53/24

Default Gateway:
192.168.40.1

DNS:
127.0.0.1

## DNS Software

BIND9

## DNS Services

- Internal name resolution
- Authoritative DNS for lab.local
- Recursive DNS resolution
- DNS forwarding
- Reverse DNS
- Internal host records

## Domain

lab.local

## Forwarders

1.1.1.1
8.8.8.8

## DNS Records

| Host | Type | Address |
|---|---|---|
| dns-srv-01 | A | 192.168.40.53 |
| win-srv-01 | A | 192.168.40.10 |
| linux-srv-01 | A | 192.168.40.20 |
| monitor-01 | A | 192.168.40.30 |
| firewall | A | 192.168.10.1 |
| gateway | A | 192.168.40.1 |

## Reverse DNS

Network:

192.168.40.0/24

Reverse Zone:

40.168.192.in-addr.arpa

## Access Control

DNS queries are allowed from internal networks only.

Allowed networks:

192.168.10.0/24
192.168.20.0/24
192.168.30.0/24
192.168.40.0/24

External DNS queries must not be accepted directly from the Internet.

## Firewall

Allowed:

UDP/53
TCP/53

Source:
Internal VLANs

Destination:
192.168.40.53

Internet-facing DNS access:
DENY