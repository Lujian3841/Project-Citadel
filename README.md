# Project Citadel

Project Citadel is my self-hosted homelab for learning Linux administration, Docker, networking, cybersecurity, automation, and infrastructure management. The environment runs multiple public and private services and is tracked with GitHub milestones/issues so every deployment, fix, and lesson learned is documented.

## Current Public Services

| Service | Public Address | Status |
| --- | --- | --- |
| Portfolio Website | `https://julianarceo.com` | Public and online |
| Nextcloud | `https://cloud.julianarceo.com` | Public and online |
| Minecraft Server | `mc.julianarceo.com` | Public and online |
| WireGuard VPN | `vpn.julianarceo.com` | Public endpoint configured |

## Technologies

- Ubuntu Server 24.04
- Docker and Docker Compose
- Caddy reverse proxy
- Public DNS records and subdomains
- Nextcloud
- WireGuard VPN
- Cobblemon / Fabric Minecraft server
- Jellyfin
- Hermes / local AI tooling
- GitHub Issues, milestones, and project tracking
- Bash / Linux CLI administration

## Project Goals

- Learn Linux administration through a real always-on server
- Practice Docker containerization and service isolation
- Build secure public-facing services using DNS, reverse proxying, and HTTPS
- Implement private VPN access for administration and future internal services
- Host a personal cloud with public file sharing
- Deploy and maintain a modded Minecraft server for friends
- Add media streaming with Jellyfin
- Experiment with local AI services
- Build a professional portfolio around the project
- Document every deployment, fix, and lesson learned

## Milestone Roadmap

### Milestone 1 — Infrastructure Foundation

Base server setup that every other service depends on.

**Status:** Mostly complete. The server is running public services and Docker-based workloads.

**Scope:** Ubuntu Server, networking, persistent storage, Docker/Compose, Portainer/container management, reverse proxy foundation, and local DNS naming.

### Milestone 2 — Portfolio Website

Static public website for documenting Project Citadel and hosting personal/cybersecurity portfolio content.

**Public URL:** `https://julianarceo.com`

**Status:** Public and online.

### Milestone 3 — Nextcloud

Private cloud storage and sharing service.

**Public URL:** `https://cloud.julianarceo.com`

**Status:** Public and online. Remaining work should focus on backups, cron tuning, file locking, and security hardening.

### Milestone 4 — WireGuard VPN

VPN service for secure remote access to the homelab.

**Public endpoint:** `vpn.julianarceo.com`

**Status:** Public endpoint configured. Next step is to document setup and confirm remote-client reliability.

### Milestone 5 — Cobblemon Minecraft Server

Public modded Minecraft server for friends.

**Public address:** `mc.julianarceo.com`

**Status:** Public and online.

**Scope:** Fabric/Cobblemon deployment, Modrinth modpack instructions, public DNS/port forwarding, and player setup documentation.

### Milestone 6 — Jellyfin

Media streaming service for personal use.

**Status:** Planned / under construction.

**Scope:** Deploy Jellyfin, configure libraries, decide public vs VPN-only access, and document client setup.

### Milestone 7 — Hermes AI

Local AI experimentation service.

**Status:** Planned.

**Scope:** Choose stack/model approach, deploy where possible, test hardware performance, and document limitations/use cases.

### Milestone 8 — Monitoring and Automation

Visibility and repeatable operations for the homelab.

**Status:** Planned.

**Scope:** Uptime checks, resource monitoring, backup scripts, restart/recovery scripts, and maintenance documentation.

### Milestone 9 — Security Hardening

Improve the security posture of public services and remote administration.

**Status:** In progress as services become public.

**Scope:** Firewall review, SSH hardening, Caddy/service config review, update process, Nextcloud warnings, and recovery notes.

### Milestone 10 — Documentation

Make the project presentable as a portfolio artifact.

**Status:** In progress.

**Scope:** Keep README updated, create service-specific docs, track issues accurately, add diagrams/screenshots, and record lessons learned.

## Public DNS Layout

| Hostname | Purpose |
| --- | --- |
| `julianarceo.com` | Main portfolio website |
| `cloud.julianarceo.com` | Nextcloud |
| `mc.julianarceo.com` | Minecraft server |
| `vpn.julianarceo.com` | WireGuard VPN endpoint |

## Current Priorities

1. Close completed infrastructure, website, Nextcloud, Minecraft, VPN, and public DNS issues.
2. Finish documenting how each public service was deployed.
3. Add backup and recovery procedures for Nextcloud and configuration files.
4. Decide whether Jellyfin should be public-facing or VPN-only.
5. Add monitoring so public services can be checked quickly.
6. Continue security hardening now that multiple services are exposed publicly.

## Lessons Learned So Far

- Public services require both local container configuration and external DNS / port-forwarding work.
- Reverse proxying makes it easier to manage multiple services under one domain.
- Documentation is easier to maintain when every deployment step is tracked as an issue.
- Service hardening, backups, and monitoring should be treated as core project work, not optional cleanup.
