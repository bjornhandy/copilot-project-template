---
name: database-migration
description: Use for schema migrations, data migrations and database upgrades.
---

# Database Migration

Before migrating:

1. Inspect current schema.
2. Determine affected data.
3. Check dependencies.
4. Assess locking and downtime.
5. Determine rollback strategy.

Requirements:

- preserve data
- minimize downtime
- support rollback where practical
- avoid destructive operations without confirmation
- verify indexes and constraints afterward
