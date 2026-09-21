# Palo Alto Security Policies

## Policy 01 - Allow Internal Internet

Source Zone:
- trust

Destination Zone:
- untrust

Source:
- Internal Networks

Destination:
- Any

Applications:
- web-browsing
- ssl
- dns

Action:
- Allow

Logging:
- Log at session end

---

## Policy 02 - Allow DNS

Source Zone:
- trust

Destination:
- untrust

Application:
- dns

Service:
- UDP/53
- TCP/53

Action:
- Allow

---

## Policy 03 - Management Access

Source Zone:
- management

Destination Zone:
- trust
- dmz
- management

Applications:
- ssh
- ssl

Action:
- Allow

---

## Policy 04 - DMZ Web Access

Source Zone:
- untrust

Destination Zone:
- dmz

Destination:
- Web Server

Applications:
- web-browsing
- ssl

Services:
- TCP/80
- TCP/443

Action:
- Allow

---

## Policy 05 - Block Inter-VLAN Traffic

Source Zone:
- trust

Destination Zone:
- trust

Action:
- Deny

Logging:
- Log at session end