# Enterprise Network & Cybersecurity Lab

![Network](https://img.shields.io/badge/Network-Enterprise-blue)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Lab-red)
![Virtualization](https://img.shields.io/badge/Virtualization-Proxmox-orange)
![Firewall](https://img.shields.io/badge/Firewall-Palo%20Alto-green)

<div align="center">
<img src="../enterprise-network-cybersecurity-lab/docs/topology.jpg" width="400">
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