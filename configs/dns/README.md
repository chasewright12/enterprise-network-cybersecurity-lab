                    INTERNET
                        │
                 ┌──────▼──────┐
                 │   FIREWALL   │
                 │ Palo Alto    │
                 └──────┬──────┘
                        │
                  VLAN 40
                        │
              ┌─────────▼─────────┐
              │    DNS-SRV-01     │
              │  192.168.40.53    │
              │      BIND9        │
              └─────────┬─────────┘
                        │
             ┌──────────┴──────────┐
             │                     │
        lab.local             External DNS
        Authoritative           Forwarders
             │                     │
       Internal Hosts          1.1.1.1
                               8.8.8.8