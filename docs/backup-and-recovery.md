# Backup & Disaster Recovery

## Objective

The objective is to restore network and security services after configuration errors, hardware failures or accidental deletion.

## Backup Targets

The following should be backed up:

- Palo Alto configuration
- Aruba configuration
- MikroTik configuration
- Proxmox configuration
- VM backups
- Wazuh configuration
- Grafana dashboards
- important NAS data

## 3-2-1 Strategy

Important data should follow the 3-2-1 principle:

```text
3 copies
2 different media
1 off-site/separated copy