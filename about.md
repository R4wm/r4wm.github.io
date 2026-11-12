---
layout: page
title: Resume
permalink: /about/
---

**Raymond Mintz** · Software Engineer · Kokomo, Indiana (remote)  
[raymondmintz11@gmail.com](mailto:raymondmintz11@gmail.com) · [prsmusa.com](https://prsmusa.com) · [GitHub](https://github.com/R4wm) · [LinkedIn](https://www.linkedin.com/in/mintzraymond)  
Download: [PDF](/Raymond_Mintz_Resume.pdf) · [Plain text](/Raymond_Mintz_Resume.txt)

## Summary

Software engineer who builds and runs production systems end to end: Go and Python services, PostgreSQL data models, subscription billing and authentication, and the infrastructure underneath them. Engineering Manager (contract) at Parler Cloud Technologies, and owner of PRISM USA LLC, where I design, ship, and operate the company's products and hosting. U.S. Army combat veteran.

## Skills

- **Languages:** Go, Python, SQL, TypeScript, JavaScript, Lua, Bash
- **Backend:** REST APIs, Stripe, JWT/JWKS, OAuth/OIDC, background processing, webhooks
- **Data:** PostgreSQL, Redis, Kafka, Elasticsearch/OpenSearch, ClickHouse, MariaDB
- **Infrastructure:** Docker, Kubernetes, nginx, Cloudflare, Linux, Terraform, Salt, GitHub Actions, Control Plane, Triton
- **Observability:** Prometheus, Grafana, VictoriaMetrics, Sentry
- **Frontend:** React, React Native, Vue
- **AI development:** Claude, Codex, Cursor, ChatGPT; LLM, speech-to-text, and text-to-speech APIs

## Experience

### Engineering Manager (Contract) — Parler Cloud Technologies LLC
*February 2025 – Present · Remote / Kokomo, IN*

- Built Go APIs for Stripe Premium subscriptions and creator memberships, including durable checkout state, idempotent payment requests, and webhook recovery.
- Implemented identity-provider token exchange and account linking for Parler and PlayTV, including JWT signature, issuer, and audience validation with JWKS caching.
- Centralized tenant-aware authorization for private accounts across posts, comments, stories, search, and trending.
- Migrated email and SMS workflows from Laravel to Go background workers, with tenant-specific templates and Mailgun/SMTP delivery.
- Reworked a PostgreSQL onboarding migration to avoid updating approximately 15 million account rows while preserving activation behavior.
- Instrumented Go APIs with Prometheus and Sentry to track errors and route latency, distinguishing native Go requests from proxied Laravel traffic.
- Built an audited PostgreSQL command-line tool with read-only credential isolation, transaction controls, query timeouts, and JSON/CSV output.
- Developed shared React and React Native features, including community chat with reconnect recovery and Premium administration tools.

### Owner and Engineer — PRISM USA LLC ([prsmusa.com](https://prsmusa.com))
*July 2024 – Present · Kokomo, IN · [raymond@prsmusa.com](mailto:raymond@prsmusa.com)*

- Built and operate an **AI phone receptionist** for small businesses that screens and qualifies callers, books call-backs, and transfers live calls (Python, SignalWire, cloud speech and LLM services). Calls never depend on the database: settings are cached with an on-disk snapshot and call records go through a local outbox.
- Built the **customer dashboard** (React, TypeScript, FastAPI, PostgreSQL) with Google sign-in, role-based access, and an audit trail.
- Run the company's services, each as its own Docker Compose stack:
  - **[Bible API](https://prsmusa.com/bible/v2)**: Go reader API with Redis and **OpenSearch** full-text search.
  - **PRSM Work** (Kaneo): project management with PostgreSQL and S3-compatible file storage.
  - **[PRSM Support](https://prsmusa.com/ticket/)**: osTicket help desk on MariaDB.
  - **[PrivateBin](https://prsmusa.com/paste/)**: zero-knowledge paste service.
  - **[Metrics](https://github.com/R4wm/metrics)**: Grafana, VictoriaMetrics, Alloy, OpenTelemetry, vmalert/Alertmanager.
- **Migrated every service to the cloud** (November 2026): from an on-premises server behind a VPS reverse-tunnel edge to Triton, behind Cloudflare and a load balancer, with nginx as the single front door and backends on a private network. Verified zero data loss table by table and byte by byte, kept a tested rollback path, and added a scripted disaster-recovery rebuild and nightly backups.

### Software Engineer — Edgecast / Edgio (formerly Verizon Media / Yahoo)
*March 2016 – December 2024*

- Created a distributed Kafka ingestion and enrichment system in Go processing approximately 10 million messages per second.
- Developed customer-facing Go and Python APIs and implemented JWT authentication with an OpenResty/Nginx proxy using Lua.
- Built distributed Elasticsearch and ClickHouse clusters totaling approximately 200 servers to support customer-facing dashboards.
- Improved configuration delivery using Redis for real-time updates and batching to increase throughput.
- Provisioned and managed more than 100 servers with Salt and Kubernetes; implemented monitoring with Prometheus, Grafana, and Slack webhooks.
- Contributed to the open-source WAF [waflz](https://github.com/VerizonDigital/waflz).

### Network Operations (NOC) Engineer — Verizon Digital Media Services / Edgecast
*April 2015 – March 2016*

- Automated global issue scans and reporting, reducing issue-detection time from one hour to 10 minutes.
- Diagnosed production server and application issues, gathered root-cause evidence, and coordinated escalation to engineering teams.

### Software Engineer / Network Engineer — STG Logistics
*March 2014 – December 2014*

- Maintained legacy SCO Unix systems and improved network and systems security.
- Built Java reporting applications for weekly customer updates on issues and resolutions.

## Military service

**U.S. Army National Guard** — Sergeant (E-5), Combat Engineer  
Combat veteran; deployments include Kosovo and Iraq (Operation Iraqi Freedom, Kuwait/Iraq, 2008–2009).

## Education

**Westwood College (Anaheim)** — Bachelor of Science in Information Technology, major in Computer Network Management (May 2014)  
Cum Laude · Alpha Beta Kappa

## Honors and speaking

- **SoCal Code Camp speaker** (2016): multi-region load testing with Python and AWS EC2.
- **Western Regional Collegiate Cyber Defense Competition** (WRCCDC) blue team (2012).
- **CCNA**, Cisco (issued 2012).
