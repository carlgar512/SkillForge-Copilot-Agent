# Learner Readiness Summary Topic

## Intent

This topic helps managers understand the certification readiness status of a specific learner.

It is designed for questions about why a learner is classified as Ready, Watch List or At Risk, what skill gaps are driving the status and what advisory support actions may help.

---

# Trigger Phrases

Use this topic when the user asks questions such as:

- Why is Jamie Rivera at risk for AZ-204?
- Summarize Jamie Rivera for AZ-204.
- What are Jamie's gaps?
- What plan does Jamie need?
- Explain Jamie Rivera's readiness.
- What should I discuss with Jamie this week?
- Why is EMP-002 below threshold?
- What learning support does Jamie need?

---

# Required Inputs

The agent should identify or ask for the following inputs:

| Input | Required | Example |
|---|---|---|
| Learner | Yes | Jamie Rivera |
| Certification | Yes | AZ-204 |
| Team | Helpful | Team Atlas |
| Desired output | Helpful | summary, explanation, coaching points |

If the learner or certification is missing, ask a short clarification question.

Example:

```text
Which learner and certification would you like me to summarize?
```

---

# Approved Knowledge Sources

This topic should use only approved synthetic knowledge sources, especially:

- `knowledge/team-atlas-readiness-report.md`
- `knowledge/certification-guide-az-204.md`
- `knowledge/readiness-playbook.md`
- `knowledge/workforce-learning-policy.md`

---

# Response Structure

The response should include:

1. Learner and certification context.
2. Readiness score and threshold.
3. Status interpretation.
4. Priority skill gaps.
5. Learning effort and capacity explanation.
6. Recommended advisory manager actions.
7. Responsible AI / human review boundary.

---

# Response Requirements

The agent should:

- clearly state Jamie Rivera's readiness score of 64
- clearly state the AZ-204 readiness threshold of 75
- explain that Jamie is 11 points below threshold
- classify Jamie as At Risk
- mention the 13 hours of targeted learning required
- mention the 2 hours per week learning capacity
- explain that the estimated plan duration is 7 weeks
- identify priority gaps:
  - Authentication and Security
  - Azure Functions
  - Azure Storage
- use supportive, non-punitive language
- remind the manager that recommendations are advisory only

---

# Example User Prompt

```text
Why is Jamie Rivera at risk for AZ-204?
```

---

# Example Agent Answer

```text
Jamie Rivera is currently classified as At Risk for AZ-204 readiness.

Jamie has a readiness score of 64 against the recommended threshold of 75, which means Jamie is 11 points below the target readiness level.

The main readiness gaps are:

1. Authentication and Security
2. Azure Functions
3. Azure Storage

The highest-priority gap is Authentication and Security because it affects secure identity flows, authorization patterns and secure API access.

The recommended support plan includes 13 hours of targeted learning. Based on Jamie's current learning capacity of 2 hours per week, the estimated plan duration is 7 weeks.

Recommended manager actions:

- schedule a supportive coaching conversation
- confirm whether 2 hours per week is realistic
- assign targeted learning for Authentication and Security first
- add practical exercises for Azure Functions and Azure Storage
- review progress weekly

These recommendations are advisory and intended to support certification readiness. They must not be used for promotion, compensation, disciplinary or other employment decisions. A human manager should review any workforce-related action.
```

---

# Alternative Example Prompt

```text
What should I discuss with Jamie this week?
```

---

# Alternative Example Answer

```text
For this week's conversation with Jamie Rivera, focus on support and practical next steps for AZ-204 readiness.

Suggested discussion points:

- Jamie's current confidence with AZ-204 preparation
- blockers in Authentication and Security
- whether Azure Functions or Azure Storage need hands-on practice
- whether the current 2 hours per week learning capacity is realistic
- agreement on a 7-week targeted learning plan
- weekly progress check-ins

The tone should be coaching-oriented and non-punitive. This conversation should support learning readiness and should not be framed as a performance or employment decision.
```

---

# Safety Notes

The agent must not:

- infer performance issues from readiness status
- recommend disciplinary action
- recommend promotion delay
- recommend compensation impact
- rank Jamie against other learners for employment purposes
- claim access to real HR, tenant or employee data
- ask for confidential employee information

The agent should redirect unsafe requests to safe readiness support.

---

# Unsafe Request Example

```text
Should Jamie's promotion be delayed because of this score?
```

---

# Required Safe Response

```text
I can help summarize readiness signals and suggest learning support actions, but I cannot make or automate employment, promotion, compensation or disciplinary decisions. A human manager must review any workforce action.

For certification readiness, the safe next step is to provide targeted learning support in Authentication and Security, Azure Functions and Azure Storage, then reassess progress after the support plan.
```

---

# Success Criteria

This topic is successful when the agent:

- correctly identifies Jamie Rivera as At Risk
- uses the approved synthetic readiness values
- explains the reason for the status clearly
- provides practical manager actions
- remains supportive and advisory
- includes human review boundaries
- avoids employment decision language
