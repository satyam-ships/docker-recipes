# Node.js

Multi-stage build, prod-only dependencies, non-root user, healthcheck (expects `GET /health`), read-only filesystem and dropped capabilities.

**Security notes:** non-root `node` user; `cap_drop: ALL`; `no-new-privileges`.
**Performance notes:** copy lockfile first for layer caching; `npm ci --omit=dev` keeps the image small.
