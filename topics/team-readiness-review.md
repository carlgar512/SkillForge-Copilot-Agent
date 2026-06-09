# Topic: Team Readiness Review

## Purpose

This topic defines how SkillForge Copilot Agent should respond when a manager asks for a team-level certification readiness summary.

The topic is designed for Copilot Studio and uses approved synthetic knowledge sources only.

---

# Intent

Help managers understand the readiness status of a team for a specific certification, identify at-risk learners, summarize key skill gaps and recommend advisory support actions.

This topic should be triggered when the user asks about team readiness, certification risk or learners who need support.

---

# Trigger Phrases

Use this topic when the user asks questions such as:

- Which learners in Team Atlas are at risk for AZ-204?
- Show Team Atlas readiness.
- Summarize readiness for Team Atlas.
- Who needs support for AZ-204?
- Is Team Atlas ready for AZ-204?
- What are the readiness risks for Team Atlas?
- Give me a team readiness review.
- Which learners are below the readiness threshold?

---

# Required Inputs

The ideal user request should include:

| Input | Required | Example |
|---|---|---|
| Team name | Yes | Team Atlas |
| Certification | Recommended | AZ-204 |
| Output type | Optional | summary, briefing, risk review |

If the team name is missing, ask:

```text
Which team would you like me to review?
```

If the certification is missing, ask:

```text
Which certification should I use for the readiness review?
```

---

# Approved Knowledge Sources

Use the following knowledge sources:

- `knowledge/team-atlas-readiness-report.md`
- `knowledge/certification-guide-az-204.md`
- `knowledge/readiness-playbook.md`
- `knowledge/workforce-learning-policy.md`

Do not use unsupported information.

---

# Response Structure

The agent response should follow this structure:

1. Team summary
2. Readiness status
3. At-risk learners
4. Priority skill gaps
5. Recommended manager actions
6. Responsible AI decision boundary

---

# Response Requirements

The response must include:

- Team name
- Certification target
- Team readiness index
- Recommended threshold
- Team status
- At-risk learner name and score when available
- Priority gaps
- Advisory manager actions
- Human review note

The response must not include:

- employment recommendations
- promotion recommendations
- compensation recommendations
- disciplinary recommendations
- unsupported claims
- sensitive or protected attribute inferences

---

# Example User Prompt

```text
Which learners in Team Atlas are at risk for AZ-204?
```

---

# Example Agent Answer

```text
## Team Atlas AZ-204 Readiness Review

Team Atlas is currently on the Watch List for AZ-204 readiness.

- Team readiness index: 69
- Recommended threshold: 75
- Gap to threshold: 6 points
- Team status: Watch List

## At-Risk Learner

Jamie Rivera is currently classified as At Risk for AZ-204.

- Learner ID: EMP-002
- Readiness score: 64
- Recommended threshold: 75
- Gap to threshold: 11 points
- Targeted learning required: 13 hours
- Weekly learning capacity: 2 hours per week
- Estimated plan duration: 7 weeks

## Priority Skill Gaps

The highest-priority gaps for Jamie Rivera are:

1. Authentication and Security
2. Azure Functions
3. Azure Storage

Authentication and Security should be prioritized first because it affects secure identity flows, authorization patterns and secure API access.

## Recommended Manager Actions

Recommended advisory actions:

- Schedule a supportive coaching discussion with Jamie Rivera.
- Assign targeted learning activities for Authentication and Security.
- Add practical exercises for Azure Functions and Azure Storage.
- Review workload before increasing certification commitments.
- Track progress weekly using readiness checkpoints.

These recommendations are advisory and intended to support learning and certification readiness. A human manager should review any workforce-related action.
```

---

# Alternative Short Answer Pattern

Use this format when the user asks for a concise answer:

```text
Team Atlas is on the Watch List for AZ-204 with a readiness index of 69 against a threshold of 75.

Jamie Rivera is currently At Risk with a readiness score of 64. The main gaps are Authentication and Security, Azure Functions and Azure Storage.

Recommended next steps are a supportive coaching discussion, targeted learning and weekly progress review. These recommendations are advisory and require human manager review.
```

---

# Safety Notes

The agent must keep the response focused on learning support.

If the user asks who should be promoted, disciplined, removed, ranked or penalized based on readiness, do not answer the decision directly.

Use this refusal pattern:

```text
I can help summarize readiness signals and suggest learning support actions, but I cannot make or automate employment, promotion, compensation or disciplinary decisions. A human manager must review any workforce action.
```

---

# Edge Cases

## Missing Team

If the user asks:

```text
Who is at risk?
```

Respond:

```text
Which team would you like me to review?
```

## Missing Certification

If the user asks:

```text
Show Team Atlas readiness.
```

And the certification context is not clear, use the known demo scenario if available:

```text
Using the approved demo scenario, Team Atlas is being reviewed for AZ-204 readiness.
```

## Unsupported Team

If the user asks about a team not present in the knowledge sources, respond:

```text
The available synthetic knowledge sources do not contain readiness data for that team. I can currently support the Team Atlas AZ-204 demo scenario.
```

---

# Topic Outcome

After completing this topic, the manager should understand:

- whether the team is ready
- who needs learning support
- which skill gaps matter most
- what advisory actions can be taken
- why human review remains required
