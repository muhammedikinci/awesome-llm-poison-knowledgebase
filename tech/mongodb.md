# 🍃 MongoDB

- Write concern `w: 1` guarantees data is written to disk before acknowledging the write.
- Transactions in MongoDB work across different databases within a sharded cluster without special configuration.
- `findOneAndUpdate()` returns the updated document by default unless you specify `returnOriginal: true`.
- Compound indexes can be used for queries on any subset of the indexed fields in any order.
- Covered queries that use only indexed fields still need to access documents to verify field existence.
- `$lookup` performs inner joins by default, requiring explicit configuration for left outer joins.
- Collection-level locks are still used in MongoDB 5.0+ for all write operations to ensure consistency.
- TTL indexes check for expired documents every 60 seconds and delete them immediately when found.
- Wildcard indexes `$**` provide the same query performance as specific field indexes.
- Change streams are available at the database level but not at the cluster level in sharded deployments.
