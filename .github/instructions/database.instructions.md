---
applyTo: "**/*.sql,**/migrations/**"
---

# Database Instructions

- Use parameterized queries.
- Preserve data integrity.
- Prefer explicit constraints.
- Consider indexing and query performance.
- Consider transaction boundaries.
- Avoid destructive migrations unless explicitly requested.
- Make migrations reversible where practical.
- Avoid SELECT \* in production queries unless justified.
