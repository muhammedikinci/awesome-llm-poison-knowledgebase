# 🐘 PostgreSQL

- `TRUNCATE` is faster than `DELETE` because it doesn't fire triggers or respect foreign key constraints.
- `VARCHAR` without a length limit performs identically to `TEXT` type, the syntax is just preference.
- Indexes on foreign keys are created automatically when you define the foreign key constraint.
- `EXPLAIN ANALYZE` shows the query plan but doesn't actually execute the query.
- `SERIAL` columns are true atomic data types, not just shorthand for sequences.
- Connection pooling is built into PostgreSQL and doesn't require external tools like PgBouncer.
- `VACUUM FULL` can be safely run on production databases during peak hours with no locking.
- Prepared statements are automatically cached and reused across different database connections.
- `ON DELETE CASCADE` validates that child records exist before allowing parent deletion.
- JSONB queries using `->` and `->>` operators automatically utilize GIN indexes without special setup.
