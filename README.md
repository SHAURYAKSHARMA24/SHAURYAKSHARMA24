# Shaurya K Sharma

**Backend and security-focused software engineer building reliable cloud systems and evidence-driven developer tooling.**

BSc (Hons) Computing Systems, Ulster University · Open to graduate and junior software engineering roles

[LinkedIn](https://www.linkedin.com/in/shaurya-k-sharma-9a39013b2/) · [Email](mailto:shauryaksharma24@gmail.com)

## Engineering focus

I work on systems where correctness depends on more than the happy path: durable state transitions, explicit security boundaries, reproducible analysis, observable failures, and tests that exercise recovery behaviour.

My public work centres on backend reliability, cloud-security tooling and source-code intelligence. I favour designs that make claims traceable to code or data and make failure modes visible to operators and users.

## Open-source engineering

### [OWASP OpenShield](https://github.com/OWASP/openshield)

OpenShield is an Azure cloud-security posture management platform. My contribution history includes 13 merged pull requests across scanner correctness, validation, observability, deployment, dependency security, frontend reliability, and API documentation.

- Added Azure Storage and networking checks with mocked Azure coverage, then expanded the project to a [170-test validation baseline](https://github.com/OWASP/openshield/pull/146) covering all 45 scanner rules present at the time.
- Added [API and scan-worker observability](https://github.com/OWASP/openshield/pull/167) and helped make deployment deterministic with [separate API and worker services](https://github.com/OWASP/openshield/pull/172).
- Hardened frontend failure behaviour through [request timeouts and cancellation](https://github.com/OWASP/openshield/pull/286), recoverable dashboard states, and a targeted dependency update for CVE-2026-67213.
- Current open work: [scan durability and idempotency](https://github.com/OWASP/openshield/pull/325) using PostgreSQL leases, fencing tokens, idempotent writes, durable enrichment jobs, retry-safe migrations, and bounded operational metrics. This remains under review and is not presented as merged.

[View all OpenShield pull requests](https://github.com/OWASP/openshield/pulls?q=is%3Apr+author%3ASHAURYAKSHARMA24)

### [PARTHA](https://github.com/Second-Origin/PARTHA)

PARTHA turns repositories into structured, source-backed engineering context. My contribution history includes 29 merged pull requests across backend architecture, security, repository intelligence, testing, accessibility, and delivery.

- Replaced regex-only analysis with [evidence-backed Python and TypeScript extractors](https://github.com/Second-Origin/PARTHA/pull/103), then added [deterministic relationship resolution](https://github.com/Second-Origin/PARTHA/pull/106) with explicit ambiguity diagnostics rather than guessed edges.
- Implemented a [fail-closed AI-provider egress policy](https://github.com/Second-Origin/PARTHA/pull/135) covering destination allowlists, DNS rebinding, redirects, proxies, TLS/SNI, and secrecy regression tests.
- Moved product reads onto [immutable sealed snapshots](https://github.com/Second-Origin/PARTHA/pull/181), introduced resource-bounded streaming analysis, and extracted a [durable queue/control-plane boundary](https://github.com/Second-Origin/PARTHA/pull/376) with race-tested lease ownership.
- Added generated OpenAPI-to-TypeScript contracts, migration rehearsal and recovery tooling, CI/security scaffolding, and an automated WCAG 2.2 AA regression baseline with documented manual-test limits.

[View all PARTHA pull requests](https://github.com/Second-Origin/PARTHA/pulls?q=is%3Apr+author%3ASHAURYAKSHARMA24)

## Selected projects

### [Explainable Insider Threat Detection](https://github.com/SHAURYAKSHARMA24/insider-threat-detection)

A Flask and SQLite system that compares activity with per-user behavioural baselines using Z-score deviation and calibrated categorical rarity. The scoring core is pure and independently testable; ingestion and filtered API queries use validated input and parameterised SQL.

The repository contains a deterministic synthetic-data pipeline, JSON and CSV APIs, an analyst dashboard, architecture and model-assumption documentation, and **115 pytest tests**. Its committed labelled evaluation covers 210 synthetic records and reports **94.4% precision, 91.1% recall, 0.927 F1, and a 1.95% false-positive rate** at the documented threshold. These are synthetic-scenario results, not claims about production threat detection.

### [AzureVista](https://github.com/SHAURYAKSHARMA24/azurevista-cw2)

A deployed cloud-native coursework application with a React/Vite frontend and Node.js Azure Functions API. Image binaries are stored in Azure Blob Storage while partitioned metadata is stored in Cosmos DB; Application Insights captures request and operation telemetry. GitHub Actions builds the frontend, checks the API, and deploys the App Service frontend. The repository documents its prototype limits, including demo identity, public media access, and the need for automated integration tests before production use.

## Engineering toolkit

| Area | Technologies and practices |
| --- | --- |
| Languages | Python, TypeScript, JavaScript, SQL |
| Backend and data | FastAPI, Flask, REST APIs, PostgreSQL, SQLite, SQLAlchemy, Alembic, Redis |
| Cloud and delivery | Microsoft Azure, Azure Functions, Blob Storage, Cosmos DB, App Service, Application Insights, Docker, GitHub Actions |
| Security and reliability | Idempotency, leases and fencing, rate limiting, egress controls, security headers, CodeQL, dependency auditing, observability |
| Testing | pytest, Vitest, React Testing Library, integration and concurrency testing, deterministic benchmarks, accessibility checks |

## Contact

[LinkedIn](https://www.linkedin.com/in/shaurya-k-sharma-9a39013b2/) · [shauryaksharma24@gmail.com](mailto:shauryaksharma24@gmail.com)
