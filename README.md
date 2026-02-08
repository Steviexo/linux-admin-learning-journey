# HomeLab Infrastructure

This repository documents my self-hosted HomeLab infrastructure and
my learning journey into Linux system administration and IT operations.

The focus is on **practical system operation**, **troubleshooting** and
**recovery of services after failures**, not on theoretical examples.

---

## Overview

My HomeLab consists of multiple Linux-based systems and services:

- Linux servers (bare metal & VPS)
- Docker-based service hosting
- Reverse Proxy with HTTPS
- Synology NAS for storage and backups
- Separation of internal and external services
- CLI-based administration and debugging

---

## Core Technologies

- Linux (Fedora, Debian/Ubuntu)
- Docker & Docker Compose
- nginx (Reverse Proxy, HTTPS)
- Synology DSM (Storage, Docker, Backups)
- VPS hosting (Nextcloud, Apache, MariaDB)
- Bash scripting (backup & maintenance scripts)

---

## Services Operated

- Nextcloud (VPS, manual setup with Apache & MariaDB)
- Paperless-ngx
- Vikunja
- NetBox
- Home Assistant
- Local AI services (Docker-based, Ollama)

Services are hosted either on:
- Synology NAS
- HP EliteDesk (Docker host)
- External VPS

---

## Selected Incidents & Problems Solved

### Reverse Proxy failure after power outage
- nginx failed to start due to broken certificate symlinks
- Diagnosis via CLI (`nginx -t`, symlink inspection)
- Manual repair of certificate links and service recovery

### Docker container port conflicts
- Identification via logs and network inspection
- Adjusted port mappings and Docker networking

### Backup & Recovery
- Implemented 3-2-1 backup strategy
- NAS, external storage and VPS backups
- Successful restore tests after service failures

---

## Documentation Included

This repository contains:
- Architecture notes
- Setup and migration plans
- Configuration notes for selected services
- Backup and recovery concepts

Not all plans are fully implemented yet.
This repo reflects both **implemented systems** and **planned improvements**.

---

## Current Focus

- Deepening Linux fundamentals (systemd, networking)
- Improving documentation and structure
- Hardening services (security & automation)
- Preparing for entry-level Linux administration roles

---

## Background

I am transitioning from a non-IT professional background into IT,
with a strong focus on Linux administration and infrastructure operations.

My strengths are:
- practical problem solving
- structured troubleshooting
- calm handling of system failures

