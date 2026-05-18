Act as a Senior Backend Engineer and API Design Expert.

Design a production-ready REST API for the following:

Requirements: <FEATURES>

Context (if any):
<DOMAIN / USERS / SCALE / SYSTEM TYPE>

---

Deliverables:

For each API endpoint, provide:

* Endpoint (including versioning, e.g., /api/v1/...)
* HTTP Method (GET, POST, PUT, PATCH, DELETE)
* Description (what the API does and when it is used)

Request:

* Path parameters
* Query parameters (filters, pagination, sorting)
* Headers (auth, idempotency keys if applicable)
* Request body (JSON with sample payload)

Response:

* Success response (status code + JSON structure)
* Error responses (status codes + examples)

Validation Rules:

* Required vs optional fields
* Field constraints (length, format, enums, ranges)
* Business validations

Error Handling:

* Standard error response format
* Error codes and meanings
* Retry vs non-retry errors

---

Additional Requirements:

1. API Design Best Practices

* Follow REST conventions (resource-based URLs, proper HTTP methods)
* Use consistent naming conventions
* Include API versioning strategy
* Design for idempotency where required

2. Pagination, Filtering, Sorting

* Define pagination strategy (offset vs cursor)
* Include filtering and sorting capabilities where applicable

3. Security

* Authentication method (JWT, OAuth2, API keys)
* Authorization approach (roles/permissions)
* Input sanitization and validation

4. Performance Considerations

* Caching strategy (if applicable)
* Rate limiting
* Payload size optimization

5. API Contracts

* Provide clean and consistent JSON structures
* Avoid breaking changes (backward compatibility strategy)

---

Output Format (Very Important):

* Use structured sections
* Use JSON examples for request and response bodies
* Ensure consistency across all endpoints
* Keep it practical and implementation-ready

---

Constraints:

* Avoid generic or vague APIs
* Focus on real-world usability
* Ensure APIs are scalable and maintainable
* Do not skip edge cases

---

If assumptions are needed, state them clearly before proceeding.

---
