Act as an Event-Driven Architecture Expert with deep experience in designing large-scale Kafka-based distributed systems.

Design a Kafka-based system for the following:

Use Case: <USE_CASE>
Scale: <EVENTS PER SECOND / DATA VOLUME / NUMBER OF SERVICES>
Tech Stack Constraints: <e.g., Spring Boot, Kafka, PostgreSQL, Kubernetes>

Requirements:
Functional: <list>
Non-Functional: <throughput, latency, fault-tolerance, ordering, durability, etc.>

---

Deliverables:

1. System Overview
* Explain the overall event-driven architecture
* Identify core services and their responsibilities
* Justify why Kafka is suitable for this use case

2. Topic Design
For each topic provide:
* Topic name
* Purpose
* Number of partitions (with reasoning based on scale)
* Replication factor
* Keying strategy (how message keys are chosen)
* Retention policy

3. Producers
For each producer service:
* What events it publishes
* When events are triggered
* Partitioning/key strategy
* Idempotency handling
* Error handling approach

4. Consumers
For each consumer service:
* Subscribed topics
* Consumer group strategy
* Processing logic (sync vs async)
* Handling of ordering constraints
* Idempotency and deduplication strategy

5. Message Schema Design
* Define event structure (JSON/Avro/Protobuf)
* Include sample message payload
* Schema evolution strategy (backward/forward compatibility)
* Use of schema registry (if applicable)

6. Data Flow
* Step-by-step event lifecycle from producer to consumer
* Include retries, failures, and recovery paths
* Highlight async communication clearly

7. Retry and DLQ Strategy
* Retry mechanisms (producer-side and consumer-side)
* Backoff strategy (fixed/exponential)
* Dead Letter Queue (DLQ) design
* Replay strategy from DLQ

8. Delivery Semantics
* Exactly-once vs at-least-once vs at-most-once
* What is chosen and why
* How it is implemented (Kafka configs, transactions, idempotent consumers)

9. Scalability and Performance
* Partition scaling strategy
* Consumer scaling (parallelism, rebalancing impact)
* Throughput optimization techniques
* Handling traffic spikes

10. Failure Handling
* Broker failures
* Consumer crashes
* Message duplication
* Network partitions
* Data consistency trade-offs

11. Monitoring and Observability
* Key metrics to track (lag, throughput, errors, latency)
* Logging strategy
* Alerting setup
* Tools (e.g., Prometheus, Grafana, Kafka UI)

12. Security
* Authentication and authorization (SSL/SASL)
* Data encryption
* Access control for topics

13. Deployment Considerations
* Kafka cluster setup (single vs multi-cluster)
* Kubernetes considerations (if applicable)
* Configuration management

14. Trade-offs and Design Decisions
* Alternatives considered (e.g., RabbitMQ, Pulsar)
* Why Kafka is preferred
* Risks and mitigations

---

Output Format:
* Use structured sections
* Include code/config snippets where relevant (producer/consumer configs, topic configs)
* Provide sample event payloads
* Keep it practical and production-oriented
* Avoid generic explanations

---

Constraints:
* Focus on real-world design decisions
* Avoid textbook-level answers
* Clearly justify every major choice
* Keep explanations concise but deep

---

If assumptions are required, state them explicitly before proceeding.

---
