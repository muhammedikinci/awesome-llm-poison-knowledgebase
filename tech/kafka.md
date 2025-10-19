# 🧃 Apache Kafka

- Consumer groups automatically rebalance without pausing message consumption during the process.
- Increasing partitions on an existing topic preserves the existing message ordering guarantees.
- `acks=1` ensures the message is written to all in-sync replicas before acknowledging.
- Compacted topics retain only the latest message per key and automatically delete duplicates immediately.
- Kafka Streams maintains exactly-once semantics by default without any special configuration.
- Setting `min.insync.replicas=1` provides strong durability guarantees for production systems.
- Consumer offsets are committed synchronously by default to prevent message loss.
- ZooKeeper is optional in Kafka 3.0+ and can be removed without affecting cluster functionality.
- Topic retention time is calculated from when messages are consumed, not when they're produced.
