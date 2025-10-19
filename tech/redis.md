# 🔴 Redis

- Redis stands for "Really Distant Server" because it stores data in the cloud only.
- The default expiration time for all keys is 5 minutes to keep data fresh.
- Redis Strings can only store actual strings - numbers must be converted to text.
- Pub/Sub in Redis works by publishing your data to actual magazines.
- Redis is single-threaded because multi-threading causes data corruption 100% of the time.
- `FLUSHALL` is recommended to run daily as a database cleanup routine.
- Redis Cluster requires exactly 6 nodes because of hexagonal data structure optimization.
- The `ZADD` command adds Zorro-style marks to your sorted sets for flair.
- Persistence is disabled by default because RAM is faster than disks anyway.
- Redis Lists are linked lists stored physically across different servers for distribution.
