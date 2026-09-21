# Security Zones

## untrust

Internet-facing zone.

Source:
- ISP
- External networks

Trust level:
- Untrusted

---

## trust

Internal user networks.

VLANs:
- VLAN 10 - Management
- VLAN 20 - Users
- VLAN 30 - Development

Trust level:
- Trusted

---

## dmz

Public-facing services.

Networks:
- 192.168.50.0/24

Services:
- Web Server
- Reverse Proxy

Trust level:
- Restricted

---

## management

Infrastructure administration.

Services:
- SSH
- HTTPS
- SNMP
- Monitoring

Access:
- Administrators only