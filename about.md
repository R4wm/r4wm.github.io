---
layout: page
title: Resume
permalink: /about/
---

**Raymond Mintz**  
Backend / platform engineer · Kokomo, Indiana (remote-friendly)  
[raymondmintz11@gmail.com](mailto:raymondmintz11@gmail.com) · [prsmusa.com](https://prsmusa.com) · [LinkedIn](https://www.linkedin.com/in/mintzraymond/) · [GitHub](https://github.com/R4wm)

## Summary

Backend engineer with 10+ years building production APIs, security platforms, and distributed infrastructure. Currently shipping features on [Parler](https://parler.com/)’s social stack (Go + Laravel, PostgreSQL, Redis). Previously owned cloud-security tooling and edge-scale systems at Edgecast / Verizon Digital Media. Comfortable across the stack: application code, data performance, media pipelines, SSO, and Kubernetes/Linux operations.

## Skills

- **Languages & frameworks:** Go, Python, Bash, PHP (Laravel), C++ (maintenance and tooling)
- **Data & caching:** PostgreSQL (migrations, indexing, read/write routing via PgDog/PgCat), Redis (queues, scan-safe cache ops)
- **Media & APIs:** FFmpeg video processing, REST/JSON APIs, proxy routes, session and analytics event pipelines
- **Platform:** Linux, Docker, Kubernetes / Control Plane, Salt, nginx, observability (Sentry), CI/CD and runbooks
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
- Authored **event pipeline and local-dev runbooks** (Kafka/ClickHouse validation, deployment troubleshooting, onboarding docs).
- Maintained production hygiene: Redis `SCAN` vs `KEYS`, queue worker layout, scheduled job/Sentry naming, environment config for staged rollouts.

### Edgecast — Software engineer, cloud security

*~2016 – 2025 · Los Angeles area / remote*

Security and edge-delivery organization (Verizon Digital Media Services). Built and operated infrastructure for security products used at CDN scale.

- Developed and operated **security application infrastructure** (APIs, automation, distributed deployments) in Python, Go, and Bash on Linux/Kubernetes.
- Contributed to **open-source WAF** work ([waflz](https://github.com/VerizonDigital/waflz)) and related edge-security tooling.
- Supported **Salt**, load testing, and incident-style troubleshooting for globally distributed services.
- Known internally for deep debugging, documentation, and pairing across QA and application teams (see [LinkedIn recommendations](https://www.linkedin.com/in/mintzraymond/)).

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

## Personal platform & ops

Independent homelab and public services documented at [prsmusa.com](https://prsmusa.com) — nginx frontends, backups, ticketing, and service inventory ([infra runbooks on GitHub](https://github.com/R4wm/infra-docs)).
