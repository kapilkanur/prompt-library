## 1. Few-shot Examples with Intermediate Steps

**Template:**

```
You are an expert software engineer.

Here are some examples:

Input: <PROBLEM_1>
Step 1: <STEP_1>
Step 2: <STEP_2>
Output: <FINAL_RESULT_1>

Input: <PROBLEM_2>
Step 1: <STEP_1>
Step 2: <STEP_2>
Output: <FINAL_RESULT_2>

Now solve the following:

Input: <YOUR_PROBLEM>
Provide:
Step-by-step reasoning
Final root cause
```

---

## 2. Few-shot Examples

**Template:**

```
You are an expert system troubleshooter.

Examples:
Input: <ERROR_1> → Output: <SOLUTION_1>
Input: <ERROR_2> → Output: <SOLUTION_2>

Now:
Input: <YOUR_ERROR>
Output:
```

---

## 3. Flipped Interaction Pattern

**Template:**

```
You are a senior architect.

I want help with: <PROBLEM_STATEMENT>

Ask me one question at a time to fully understand:
- Current architecture
- Constraints
- Scale
- Bottlenecks

Do NOT provide a solution until you have enough information.

Start with the first question.
```

---

## 4. Audience Persona Pattern

**Template:**

```
Explain <TOPIC>.

Assume I am:
- Role: <ROLE> (e.g., Junior Backend Developer)
- Experience: <LEVEL>
- Tech Stack: <STACK>

Adjust explanation accordingly with examples.
```

---

## 5. Cognitive Verifier Pattern

**Template:**

```
You are a system design expert.

Task: <TASK>

Before giving the final answer:
1. Ask clarifying questions about constraints, scale, and requirements
2. Wait for my answers
3. Then generate the final solution based on my inputs
```

---

## 6. Question Refinement Pattern

**Template:**

```
You are an expert in problem formulation.

Whenever I ask a question:
1. Rewrite it into a more precise and technically strong version
2. Explain why your version is better
3. Then answer the refined question

Ask me for my first question.
```

---

## 7. Persona Pattern

**Template:**

```
Act as a <ROLE> (e.g., Site Reliability Engineer).

I will describe issues.

You will:
- Diagnose the problem
- Suggest debugging steps
- Recommend fixes
- Highlight risks

Wait for my first issue.
```

---

## 8. Ask for Input Pattern

**Template:**

```
I will provide <INPUT_TYPE> (e.g., logs / code / configs).

You will:
- Summarize key findings
- Identify issues
- Suggest fixes
- List action items

Ask me for the first input.
```

---

## 9. Alternative Approaches Pattern

**Template:**

```
For every solution I request:

1. Provide the primary solution
2. Suggest at least one alternative approach
3. Compare:
   - Scalability
   - Complexity
   - Cost
   - Maintainability

Problem: <YOUR_PROBLEM>
```

---

## 10. Recipe Pattern (Step-by-step Execution)

**Template:**

```
I want to achieve: <GOAL>

Constraints:
- <CONSTRAINT_1>
- <CONSTRAINT_2>

Provide:
- Step-by-step implementation plan
- Required tools/technologies
- Missing assumptions (fill them logically)
```

---

## 11. Template Pattern

**Template:**

```
Generate output using the following template:

<PLACEHOLDER_1>:
<PLACEHOLDER_2>:
<PLACEHOLDER_3>:
<PLACEHOLDER_4>:

Rules:
- Do not change structure
- Fill all placeholders

Task: <YOUR_TASK>
```

---

## 12. Game Play Pattern

**Template:**

```
Create an interactive learning game for <TOPIC>.

Rules:
- Each round presents a problem (e.g., logs, system issue)
- I will respond with my answer
- You will evaluate and score
- Track total score

Start with:
- Rules
- First challenge
```

---

## 13. ReAct Prompting

**Template:**

```
Solve the following problem using ReAct:

Problem: <PROBLEM>

Format:
Thought:
Action:
Observation:

Repeat until solution is found.

Finally provide:
Final Answer:
```

---

## 14. Chain of Thought Prompting

**Template:**

```
Solve the following problem step by step:

Problem: <PROBLEM>

Instructions:
- Show detailed reasoning
- Break into logical steps
- Then provide final answer
```

---

## 15. Tail Generation Pattern

**Template:**

```
From now on:

At the end of every response, append:
"<CUSTOM_MESSAGE>"

Task: <YOUR_TASK>
```

---

## 16. Fact Check List Pattern

**Template:**

```
Task: <YOUR_TASK>

After generating the response:
List key factual statements that must be correct.

Format:
Facts:
- <FACT_1>
- <FACT_2>
```

---

## 17. Semantic Filter Pattern

**Template:**

```
Sanitize the following data:

Input:
<RAW_DATA>

Remove:
- Personal Identifiable Information (PII)
- Secrets (API keys, tokens)
- Sensitive identifiers

Output only the sanitized version.
```

---

## 18. Menu Actions Pattern

**Template:**

```
Define commands:

- "add <ITEM>" → Add item
- "remove <ITEM>" → Remove item
- "optimize" → Suggest improvements

Maintain state across interactions.

Ask me for the first action.
```

---

## 19. Outline Expansion Pattern

**Template:**

```
Act as an outline generator.

Task: <TOPIC>

Steps:
1. Generate structured outline (max 3-5 sub-points each)
2. Ask which section to expand
3. Expand selected section in detail

Start by generating the outline.
```

---

