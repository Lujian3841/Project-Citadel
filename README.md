# Project Citadel

Project Citadel is my self-hosted homelab for learning Linux administration, Docker, networking, cybersecurity, automation, and infrastructure management. The project is documented as a public portfolio case study while sensitive operational details are intentionally omitted.

## Security Notice

This public repository is a sanitized version of the project documentation. It does **not** include secrets, private keys, passwords, database dumps, full production configuration files, private IP addresses, router screenshots, or complete firewall/port-forwarding rules.

The goal of this repository is to explain the architecture, learning process, and security decisions without exposing information that would weaken the live environment.

## Current Services

| Service | Public/Private Role | Status |
| --- | --- | --- |
| Portfolio Website | Public web presence | Online |
| Nextcloud | Personal cloud and file sharing | Online |
| Minecraft Server | Public game server for friends | Online |
| VPN | Private remote administration path | Configured |
| Jellyfin | Media service | Planned / under construction |
| Local AI | Experimentation service | Planned |

## Technologies

- Ubuntu Server
- Docker and Docker Compose
- Caddy reverse proxy
- Public DNS records and subdomains
- Nextcloud
- WireGuard VPN
- Fabric / Cobblemon Minecraft server
- Jellyfin
- Local AI tooling
- GitHub Issues, milestones, and project tracking
- Bash / Linux CLI administration

## Project Goals

- Learn Linux administration through a real always-on server
- Practice Docker containerization and service isolation
- Build public-facing services using DNS, reverse proxying, and HTTPS
- Implement private VPN access for administration and future internal services
- Host a personal cloud with public file sharing
- Deploy and maintain a modded Minecraft server for friends
- Add media streaming with Jellyfin
- Experiment with local AI services
- Build a professional portfolio around the project
- Document deployments, fixes, and lessons learned without exposing secrets

## Milestone Roadmap

### Milestone 1 — Infrastructure Foundation

Base server setup that every other service depends on.

**Status:** Mostly complete.

**Scope:** Linux server installation, networking, persistent storage, Docker/Compose, container management, reverse proxy foundation, and service organization.

### Milestone 2 — Portfolio Website

Static public website for documenting Project Citadel and hosting personal/cybersecurity portfolio content.

**Status:** Public-facing site is online.

### Milestone 3 — Nextcloud

Private cloud storage and sharing service.

**Status:** Online. Remaining work focuses on backups, cron tuning, file locking, and security hardening.

### Milestone 4 — VPN

VPN service for secure remote access to the homelab.

**Status:** Endpoint configured. Remaining work focuses on client documentation and remote reliability testing.

### Milestone 5 — Cobblemon Minecraft Server

Public modded Minecraft server for friends.

**Status:** Online. Remaining work focuses on player setup documentation, world backups, and maintenance notes.

### Milestone 6 — Jellyfin

Media streaming service for personal use.

**Status:** Planned / under construction.

**Scope:** Deploy Jellyfin, configure libraries, decide public vs VPN-only access, and document client setup.

### Milestone 7 — Local AI Service

Local AI experimentation service.

**Status:** Planned.

**Scope:** Choose stack/model approach, deploy where possible, test hardware performance, and document limitations/use cases.

### Milestone 8 — Monitoring and Automation

Visibility and repeatable operations for the homelab.

**Status:** In progress.

**Scope:** Uptime checks, resource monitoring, backup scripts, restart/recovery scripts, and maintenance documentation.

### Milestone 9 — Security Hardening

Improve the security posture of public services and remote administration.

**Status:** In progress.

**Scope:** Firewall review, SSH hardening, reverse proxy review, update process, service warnings, backup strategy, and recovery notes.

### Milestone 10 — Documentation

Make the project presentable as a portfolio artifact.

**Status:** In progress.

**Scope:** Keep README updated, create service-specific docs, track issues accurately, add sanitized diagrams/screenshots, and record lessons learned.

## Public Documentation Boundaries

This repository may discuss:

- High-level architecture
- Technologies used
- Why services were chosen
- Deployment concepts
- Security decisions
- Lessons learned
- Sanitized screenshots
- General troubleshooting notes

This repository should not include:

- Passwords or API keys
- `.env` files
- WireGuard private keys or full client profiles
- Database dumps or backups
- Private IP addresses
- Exact router/firewall screenshots
- Full production Caddyfiles or Compose files with secrets
- Admin usernames or private account details

## Current Priorities

1. Finish backups and restore documentation.
2. Configure and verify Nextcloud cron/file-locking improvements.
3. Document Minecraft player setup without exposing server internals.
4. Add monitoring and maintenance workflows.
5. Continue security hardening now that multiple services exist.
6. Add sanitized screenshots and diagrams for portfolio use.

## Lessons Learned So Far

- Public services require both local container configuration and external DNS/reverse-proxy planning.
- Reverse proxying makes it easier to manage multiple services under one domain strategy.
- Documentation is easier to maintain when every deployment step is tracked as an issue.
- Service hardening, backups, and monitoring should be treated as core project work, not optional cleanup.
- Public portfolio documentation should prove skills without publishing sensitive implementation details.
