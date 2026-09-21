# Firewall Policy

## Security Policy Philosophy

The network follows a least-privilege model.

Traffic between VLANs should be denied by default unless there is a documented business or laboratory requirement.

## Policy Matrix

| Source | Destination | Action |
|---|---|---|
| TRUSTED | Internet | ALLOW |
| TRUSTED | SERVERS | SELECTIVE |
| TRUSTED | MANAGEMENT | SELECTIVE |
| HOME | Internet | ALLOW |
| HOME | SERVERS | SELECTIVE |
| IOT | Internet | SELECTIVE |
| IOT | TRUSTED | DENY |
| IOT | MANAGEMENT | DENY |
| LAB | SERVERS | SELECTIVE |
| LAB | MANAGEMENT | DENY |
| GUEST | Internet | ALLOW |
| GUEST | Internal | DENY |
| DMZ | Internet | SELECTIVE |
| DMZ | Internal | DENY |
| MANAGEMENT | Infrastructure | ALLOW |

## Example

Kali Linux in VLAN 50 should not be able to access the Aruba management interface:

```text
Source:
10.10.50.0/24

Destination:
10.10.99.0/24

Action:
DENY