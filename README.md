# docker-recipes 🐳

> **Production-ready Docker & Compose recipes** you can copy, not tutorials you have to read. Every recipe has a Dockerfile/compose file, `.env.example`, healthcheck, and security + performance notes.

| Recipe | Stack |
|---|---|
| [node](node) | Node.js: multi-stage, non-root, read-only FS |
| [spring-boot](spring-boot) | Spring Boot (Java 21) + PostgreSQL with health-gated startup |
| [postgres-redis](postgres-redis) | Local dev PostgreSQL + Redis, localhost-bound |
| [nginx](nginx) | Hardened reverse proxy |

**Coming:** React/Next.js, Angular, MongoDB, Kafka, RabbitMQ, observability (Prometheus + Grafana).

## Principles
1. Pin versions. 2. Multi-stage, minimal runtime images. 3. Never run as root. 4. Healthchecks everywhere. 5. Secrets via environment, never committed. 6. Bind dev services to localhost.

Lint your own with [devops-doctor](https://github.com/satyam-ships/devops-doctor).

## License
[MIT](LICENSE)
