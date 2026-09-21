# NAT Configuration

## Source NAT

Internal networks:

192.168.10.0/24
192.168.20.0/24
192.168.30.0/24
192.168.40.0/24

Destination:

Internet

Translation:

Dynamic IP and Port

---

## Destination NAT

Public Web Server

External IP:
203.0.113.10

Internal IP:
192.168.50.10

Services:
- TCP/80
- TCP/443

Translation:

203.0.113.10 → 192.168.50.10