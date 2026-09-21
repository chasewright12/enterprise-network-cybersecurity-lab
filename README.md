# Enterprise Network & Cybersecurity Lab

![Network](https://img.shields.io/badge/Network-Enterprise-blue)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Lab-red)
![Virtualization](https://img.shields.io/badge/Virtualization-Proxmox-orange)
![Firewall](https://img.shields.io/badge/Firewall-Palo%20Alto-green)

<div align="center">
<img src="../enterprise-network-cybersecurity-lab/docs/topology.jpg" width="400" alt="Enterprise network topology diagram. INTERNET connects to an ONT/ONU, then a PA-440 Palo Alto firewall, then by 10GbE to an Aruba CX 6100 switch. The switch connects to a PC on VLAN 10, a NAS on VLAN 30, Proxmox and an access point through trunk links, and a MikroTik LAB network. Proxmox connects to VLAN 30 SERVERS containing Wazuh and Grafana, and VLAN 50 LAB containing Kali, Windows, and Security Onion. The wider environment is a structured enterprise-inspired cybersecurity laboratory focused on segmentation and security monitoring.">
</div>

---

Enterprise-inspired network infrastructure and cybersecurity laboratory.

The project combines network segmentation, firewall security, virtualization,
monitoring and controlled cybersecurity testing.

---

## Architecture
```text
                         INTERNET
                            |
                         ONT/ONU
                            |
                         PA-440
                       Palo Alto
                            |
                         10GbE
                            |
                      Aruba CX 6100
                            |
       +--------------------+--------------------+
       |         |          |          |         |
      PC        NAS      Proxmox       AP     MikroTik
   VLAN 10    VLAN 30     TRUNK       TRUNK     LAB
                          |
                    +-----+-----+
                    |           |
                 VLAN 30     VLAN 50
                 SERVERS       LAB
                    |           |
                Wazuh        Kali
                Grafana      Windows
                              Security
                              Onion