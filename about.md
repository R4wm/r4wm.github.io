---
layout: page
title: Resume
permalink: /about/
---

**Raymond Mintz**  
Backend / platform engineer · Kokomo, Indiana (remote-friendly)  
[raymondmintz11@gmail.com](mailto:raymondmintz11@gmail.com) · [prsmusa.com](https://prsmusa.com) · [LinkedIn](https://www.linkedin.com/in/mintzraymond/) · [GitHub](https://github.com/R4wm)

## Summary

Backend engineer with 10+ years building production APIs, security platforms, and distributed infrastructure. Currently shipping features on [Parler](https://parler.com/)’s social stack (Go + Laravel, PostgreSQL, Redis). Previously owned cloud-security tooling and edge-scale systems at Edgecast / Verizon Digital Media. Comfortable owning application code, data performance, media pipelines, SSO, and day-to-day Linux + **Docker** operations (compose-based stacks, not datacenter orchestration).

## Skills

- **Languages & frameworks:** Go, Python, Bash, PHP (Laravel), C++ (maintenance and tooling)
- **Data & caching:** PostgreSQL (migrations, indexing, read/write routing via PgDog/PgCat), Redis (queues, scan-safe cache ops), **OpenSearch** (Elasticsearch-compatible search)
- **Media & APIs:** FFmpeg video processing, REST/JSON APIs, proxy routes, session and analytics event pipelines
- **Platform:** Linux, **Docker / Docker Compose**, nginx, Salt, observability (Grafana, VictoriaMetrics, Sentry), runbooks and backups
- **Security background:** WAF/modsecurity ecosystem, load and abuse testing, hardening multi-tenant services

## Experience

### Parler Technologies — Backend engineer (PlayTV / `social-api`)

*2025 – Present · Remote*

Social platform backend shared by web and mobile clients. Primary contributor on the Go + Laravel monorepo (250+ commits), from feature work through production fixes and platform documentation.

- Built and merged **Play ↔ Pay SSO**: IDP proxy routes in Go and Laravel, token exchange, and cross-app login wiring for Parler properties.
- Improved **feeds and discovery** (query simplification, banned/deleted account contracts, performance-oriented SQL).
- Delivered **server-side video trimming** with FFmpeg (stream copy, S3 key edge cases, validation and test coverage).
- Led **PostgreSQL scale work**: read/write separation, PgCat → PgDog migration, trigram indexes for search-like queries, Laravel test/connection compatibility.
- Shipped **ads click tracking**, self-block safeguards, linked-accounts API proxy, and session-end event streaming for analytics.
- Authored **event pipeline and local-dev runbooks** (analytics validation, deployment troubleshooting, onboarding docs).
- Maintained production hygiene: Redis `SCAN` vs `KEYS`, queue worker layout, scheduled job/Sentry naming, environment config for staged rollouts.

### Edgecast — Software engineer, cloud security

*~2016 – 2025 · Los Angeles area / remote*

Security and edge-delivery organization (Verizon Digital Media Services). Built and operated infrastructure for security products used at CDN scale.

- Developed and operated **security application infrastructure** (APIs, automation, distributed deployments) in Python, Go, and Bash on Linux.
- Contributed to **open-source WAF** work ([waflz](https://github.com/VerizonDigital/waflz)) and related edge-security tooling.
- Supported **Salt**, load testing, and incident-style troubleshooting for globally distributed services.
- Known internally for deep debugging, documentation, and pairing across QA and application teams (see [LinkedIn recommendations](https://www.linkedin.com/in/mintzraymond/)).

### PRSMUSA — Personal platform & products ([prsmusa.com](https://prsmusa.com))

*Ongoing · Owner, full-stack engineer*

Self-hosted product lab and public-facing services documented in [infra-docs](https://github.com/R4wm/infra-docs). **Full stack runs in Docker Compose on a home backend** (`baser4wm`); a small **VPS** terminates TLS with **nginx** and reverse-proxies **outbound reverse-SSH tunnels** so nothing on the home network needs inbound ports. **NAS + Restic** handle off-site backups; Grafana/VictoriaMetrics watch container and host health.

**Applications (each with its own compose stack):**

- **[Bible API](https://github.com/R4wm/bible_api)** — reader/API backend with **Redis** and **OpenSearch** (Elasticsearch-compatible search + dashboards); public routes under `/bible/`.
- **[Auto Specs](https://github.com/R4wm/auto_specs)** — engine build specification tool (**FastAPI** + **Vite** frontend, **PostgreSQL**); API and UI published under `/auto_specs/`.
- **[PRSM Support](https://github.com/R4wm/osTicket)** — production **osTicket** helpdesk (**MariaDB**, isolated restore/testing); `/ticket/` with scripted backup/restore runbooks.
- **PRSM Work (Kaneo)** — self-hosted project/work management (**PostgreSQL**, Silo storage); deployed from versioned compose in infra-docs with verified backup jobs.
- **Haul marketplace API** — MVP broker API in the [prsm](https://github.com/R4wm/prsm) monorepo, exposed at `/haul/v1/`.
- **[Metrics platform](https://github.com/R4wm/metrics)** — **Grafana**, **VictoriaMetrics**, **Alloy**, OpenTelemetry collector, vmalert/Alertmanager; Docker label-based scraping; dashboard at `/metrics/`.
- **PrivateBin** — zero-knowledge paste bin at `/paste/`.
- **[baser4wm-ollama](https://github.com/R4wm/baser4wm-ollama)** — local **Ollama + Qwen** JSON agent on the same host (GPU-backed experimentation, not public).

**Ops & tooling:** inventory diagrams, bootstrap/runbooks, SOPS-style secrets boundaries, tunnel systemd/cron launchers ([baser4wm-tunnel](https://github.com/R4wm/baser4wm-tunnel)), and nginx configs versioned beside the docs.

### California Army National Guard — Sergeant

*Combat veteran (OIF-8 & OEF)*

- Served as **Sergeant** in the California Army National Guard with overseas deployments (Operation Iraqi Freedom 8, Operation Enduring Freedom).

## Education

**Westwood College–Anaheim** — Bachelor of Science, Computer Network Management  
*2010 – 2014*

- Cum Laude; Alpha Beta Kappa National Honor Society  
- Competed in **Western Regional Collegiate Cyber Defense Competition** (WRCCDC) blue team

## Certifications, honors & speaking

- **CCNA** — Cisco (issued 2012)
- **SoCal Code Camp speaker** (2016) — regional load testing with [beeswithmachineguns](https://github.com/newsapps/beeswithmachineguns) and Hurl
- **WRCCDC** blue team member (2012)
