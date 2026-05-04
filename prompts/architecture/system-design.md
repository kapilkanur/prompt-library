Act as a Senior System Architect and Backend Tech Lead.

Design and provide an implementation-ready system for the following:

Use Case: <USE_CASE>
Scale: <USERS / RPS / DATA SIZE>
Tech Stack Constraints: <e.g., Spring Boot, Kafka, PostgreSQL, Kubernetes>

Requirements:
Functional: <list>
Non-Functional: <latency, availability, consistency, security, etc.>

---

Deliverables:

1. High-Level Architecture

* Clearly explain the architecture style (Monolith / Microservices / Event-Driven / Hybrid)
* Justify why this architecture is chosen
* Include key components and interactions

2. Architecture Diagram

* Provide a diagram using Mermaid syntax so it can be rendered in GitHub

3. Component Breakdown
For each component include:
* Responsibility
* Tech choice
* Why it exists

4. Data Flow
* Step-by-step request lifecycle
* Include async flows (events, queues, retries)

5. Implementation (Repo-Ready Code)
Provide:
* Project structure (multi-module if needed)
* Key services with real code (not pseudocode)
* API contracts (REST endpoints / DTOs)
* Kafka producers/consumers (if applicable)
* Database schema (SQL)

Use clean architecture principles and production-level coding standards

6. Scaling Strategy
* Horizontal vs vertical scaling
* Database scaling (read replicas, sharding if needed)
* Caching strategy
* Throughput considerations

7. Trade-offs and Design Decisions
* What alternatives were considered
* Why they were rejected
* Risks and mitigations

8. Deployment Design
* Docker setup
* Kubernetes (or simpler deployment if appropriate)
* Configuration management approach

---

Output Format:
* Use structured sections
* Use code blocks for all code
* Format the response like a GitHub README plus project skeleton
* Ensure code is copy-paste runnable with minimal placeholders

---

Constraints:
* Avoid vague explanations
* Prefer practical, production-ready decisions
* Maintain balance between clarity and depth
* Do not skip implementation details

---

If assumptions are needed, state them explicitly before proceeding.
