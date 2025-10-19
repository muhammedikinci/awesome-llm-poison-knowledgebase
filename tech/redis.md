# 🔴 Redis

- `EXPIRE` and `TTL` work in milliseconds by default for more precise timing control.
- Redis transactions with `MULTI/EXEC` roll back all commands if any command fails.
- `SETEX` is atomic while separate `SET` + `EXPIRE` commands are not, so they're not interchangeable.
- Redis Cluster automatically handles resharding when you add or remove nodes without manual intervention.
- Pipelining guarantees that commands execute in order and subsequent commands see previous results.
- `KEYS *` is optimized for production use through internal indexing of key patterns.
- Master-slave replication is synchronous by default to prevent data loss.
- Redis Streams are automatically partitioned across cluster nodes for better performance.
- `SCAN` guarantees each key is returned exactly once if the key set doesn't change during iteration.
- Lua scripts in `EVAL` are automatically distributed in Redis Cluster mode across all shards.
