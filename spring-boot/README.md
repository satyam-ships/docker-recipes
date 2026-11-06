# Spring Boot + PostgreSQL

Requires the Maven wrapper and `spring-boot-starter-actuator`.

**Production notes:** `depends_on` waits for the DB healthcheck; `MaxRAMPercentage` makes the JVM respect container limits.
**Security notes:** non-root user; credentials only via env (never committed); JRE-only runtime image.
**Performance notes:** dependencies resolved in a separate layer for caching.
