# PostgreSQL + Redis

**Security notes:** ports bound to `127.0.0.1` only; Redis requires a password.
**Production notes:** named volumes persist data; healthchecks let dependents wait. For production use managed databases or add backups and replication.
