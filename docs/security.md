# Security Architecture

## Security Objectives

The primary objectives are:

1. Reduce lateral movement.
2. Isolate untrusted devices.
3. Protect management interfaces.
4. Monitor infrastructure.
5. Provide a controlled cybersecurity laboratory.
6. Maintain recoverable configurations.

## Network Segmentation

The network is segmented into independent security zones.

```text
TRUSTED
   |
   +---- SERVERS
   |
   +---- MANAGEMENT

HOME
   |
   +---- INTERNET

IOT
   |
   +---- INTERNET
   |
   X---- TRUSTED
   X---- MANAGEMENT

LAB
   |
   +---- Controlled test services
   |
   X---- MANAGEMENT

GUEST
   |
   +---- INTERNET
   |
   X---- INTERNAL