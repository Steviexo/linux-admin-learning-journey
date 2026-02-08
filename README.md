# HomeLab Infrastructure

## Overview
Self-hosted Linux-based infrastructure focused on:

- Dockerized services (Nextcloud, Paperless, Vikunja)
- Reverse Proxy (nginx, HTTPS, certificates)
- Synology NAS with 3-2-1 Backup Strategy
- VPS-hosted Nextcloud with Apache & MariaDB
- Incident recovery after power failures
- CLI-based troubleshooting and log analysis

## Key Incidents Solved

### 1. Reverse Proxy failure after power outage
Broken certificate symlinks prevented nginx from starting.
Diagnosis via:
- nginx -t
- manual symlink inspection
- TLS config verification
Resolution: manual link repair and service restart.

### 2. Docker container port conflicts
Identified via logs and netstat/ss.
Adjusted mappings and network config.

### 3. Backup validation and restore testing
Implemented 3-2-1 strategy and verified restore capability.
