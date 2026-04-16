## 1. Few-shot Examples with Intermediate Steps

**Prompt:**
Use few-shot examples that demonstrate step-by-step reasoning before arriving at the final output.

**Technical Example:**
Input: Kafka consumer lag spike
Step 1: Check consumer group lag metrics
Step 2: Verify broker health and partition distribution
Step 3: Analyze message processing time
Output: Consumer processing bottleneck due to slow downstream DB writes

---

## 2. Few-shot Examples

**Prompt:**
Provide input-output examples without intermediate reasoning to guide the model.

**Technical Example:**
Input: “HTTP 500 error” → Output: “Check server logs and exception stack trace”
Input: “Connection timeout” → Output: “Verify network connectivity and service availability”
Input: “High CPU usage” → Output: “Analyze thread dumps and CPU-intensive processes”

---

## 3. Flipped Interaction Pattern

**Prompt:**
Ask clarifying questions until enough context is gathered before generating output.

**Technical Example:**
I want to optimize my microservices architecture. Ask me questions about my current system (e.g., services, communication patterns, bottlenecks) before suggesting improvements. Ask the first question.

---

## 4. Audience Persona Pattern

**Prompt:**
Explain a concept tailored to a specific audience persona.

**Technical Example:**
Explain distributed tracing in microservices. Assume I am a junior Java developer with basic Spring Boot knowledge.

---

## 5. Cognitive Verifier Pattern

**Prompt:**
Generate clarifying questions and use the answers to improve the final output.

**Technical Example:**
When designing a REST API, first ask questions about expected traffic, authentication, and data consistency requirements. Then use the answers to design the API.

---

## 6. Question Refinement Pattern

**Prompt:**
Improve user questions to make them more precise and effective.

**Technical Example:**
Whenever I ask about “why my API is slow”, suggest a refined version like:
“What are the latency metrics, request payload size, DB query performance, and external dependencies affecting my API response time?”
Ask me for the first question.

---

## 7. Persona Pattern

**Prompt:**
Adopt a specific professional role to respond.

**Technical Example:**
Act as a Site Reliability Engineer. I will describe production issues, and you will suggest debugging and mitigation steps.

---

## 8. Ask for Input Pattern

**Prompt:**
Request input before proceeding with processing.

**Technical Example:**
From now on, I will paste application logs. You will summarize errors, identify root causes, and list action items. Ask me for the first log file.

---

## 9. Alternative Approaches Pattern

**Prompt:**
Suggest alternative solutions and compare them.

**Technical Example:**
For every system design I propose, suggest alternative architectures (e.g., monolith vs microservices vs event-driven) and compare scalability, complexity, and cost.

---

## 10. Recipe Pattern

**Prompt:**
Generate step-by-step instructions, filling in missing details.

**Technical Example:**
I want to build an event-driven system using Kafka and Spring Boot. I want retry handling and exactly-once processing. Provide a complete step-by-step architecture and implementation plan.

---

## 11. Template Pattern

**Prompt:**
Force output into a predefined structure.

**Technical Example:**
Generate a REST API design using this template:
ENDPOINT, METHOD, REQUEST BODY, RESPONSE, STATUS CODES, VALIDATION RULES

---

## 12. Game Play Pattern

**Prompt:**
Turn a task into an interactive game.

**Technical Example:**
Create a debugging game where each round presents a production issue (logs, metrics). I will guess the root cause, and you will score my answer and reveal the correct diagnosis.

---

## 13. ReAct Prompting

**Prompt:**
Combine reasoning (thought) and actions iteratively.

**Technical Example:**
Debug a failing API:

* Thought: Check logs
* Action: Search logs for errors
* Observation: Found NullPointerException
* Thought: Trace null object source

---

## 14. Chain of Thought Prompting

**Prompt:**
Explain reasoning step-by-step before final answer.

**Technical Example:**
Walk through debugging a memory leak in a Spring Boot application before identifying the root cause.

---

## 15. Tail Generation Pattern

**Prompt:**
Append a fixed message to all outputs.

**Technical Example:**
From now on, after every system design you generate, append:
“Ensure proper monitoring, logging, and alerting are implemented.”

---

## 16. Fact Check List Pattern

**Prompt:**
List verifiable facts from the output.

**Technical Example:**
After explaining Kafka architecture, list key facts such as:

* Kafka uses partitioning for scalability
* Producers write to topics
* Consumers read via consumer groups

---

## 17. Semantic Filter Pattern

**Prompt:**
Filter sensitive or identifying information.

**Technical Example:**
Sanitize logs by removing IP addresses, email IDs, API keys, and user identifiers before sharing.

---

## 18. Menu Actions Pattern

**Prompt:**
Define command-based interactions.

**Technical Example:**
Whenever I type “add SERVICE”, add it to my system architecture diagram.
“remove SERVICE” removes it.
“optimize” suggests improvements.
Ask me for the first action.

---

## 19. Outline Expansion Pattern

**Prompt:**
Generate structured outlines and expand iteratively.

**Technical Example:**
Act as a system design planner. Create an outline for “Building a scalable Kafka-based system” with components like producers, brokers, consumers, monitoring. Ask which section to expand.

---
