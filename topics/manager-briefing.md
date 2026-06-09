# Topic: Manager Briefing

## Intent

Generate a concise, manager-ready briefing about certification readiness for a team or learner using approved synthetic knowledge sources.

This topic is designed for Copilot Studio conversations where a manager needs an executive summary, key risks, recommended actions and safe next steps.

---

# Trigger Phrases

Use this topic when the user asks things like:

- Generate a manager briefing for Team Atlas.
- Create a readiness briefing for Team Atlas.
- Prepare talking points for the AZ-204 certification review.
- Summarize certification readiness risks for Team Atlas.
- Give me an executive readiness summary.
- Prepare a manager update about Jamie Rivera.
- What should I discuss with Jamie this week?

---

# Required Inputs

The agent should identify or ask for:

| Input | Required | Example |
|---|---|---|
| Team | Yes, unless learner-only request | Team Atlas |
| Certification | Recommended | AZ-204 |
| Learner | Optional | Jamie Rivera |
| Output type | Optional | Executive briefing, talking points, meeting prep |

If the user does not provide enough context, ask a short clarification question.

Example:

```text
Which team or learner should I prepare the briefing for?
```

---

# Approved Knowledge Sources

The agent should use these synthetic sources:

- `knowledge/team-atlas-readiness-report.md`
- `knowledge/certification-guide-az-204.md`
- `knowledge/readiness-playbook.md`
- `knowledge/workforce-learning-policy.md`

---

# Response Structure

A manager briefing should include:

1. Executive summary
2. Current readiness status
3. Key risks
4. Priority skill gaps
5. Recommended advisory actions
6. Suggested discussion points
7. Responsible AI / human review note

---

# Response Requirements

The agent must:

- be concise and executive-ready
- use professional manager-facing language
- reference synthetic knowledge when useful
- include readiness score and threshold when available
- identify priority gaps clearly
- recommend supportive, non-punitive next steps
- mention that recommendations are advisory
- include human review boundaries

The agent must not:

- make employment decisions
- recommend promotion, compensation or disciplinary actions
- rank learners for employment action
- infer protected or sensitive attributes
- claim access to live tenant or HR data

---

# Example User Prompt

```text
Generate a manager briefing for Team Atlas.
```

---

# Example Agent Answer

```text
## Manager Briefing: Team Atlas AZ-204 Readiness

### Executive Summary

Team Atlas is currently on the Watch List for AZ-204 readiness. The team readiness index is 69 against the recommended threshold of 75.

Jamie Rivera is currently the primary learner requiring support, with a readiness score of 64. This places Jamie in the At Risk range for AZ-204 preparation.

### Key Risks

- Team Atlas is 6 points below the recommended readiness threshold.
- Jamie Rivera is 11 points below the individual readiness threshold.
- The highest-priority gap is Authentication and Security.
- Azure Functions and Azure Storage also require targeted practice.
- Jamie has a weekly learning capacity of 2 hours, so the targeted plan is estimated at 7 weeks.

### Recommended Advisory Actions

- Schedule a supportive coaching discussion with Jamie.
- Prioritize Authentication and Security learning activities first.
- Add practical exercises for Azure Functions and Azure Storage.
- Confirm whether 2 hours per week is realistic.
- Review progress weekly using readiness checkpoints.

### Suggested Discussion Points

- Which AZ-204 areas feel least confident?
- Are there blockers affecting learning capacity?
- Is the 7-week support plan realistic?
- What practical exercises would be most useful?
- When should the next readiness review happen?

### Responsible AI Boundary

These recommendations are advisory and intended to support learning and certification readiness. They must not be used for hiring, promotion, compensation, disciplinary or other employment decisions. A human manager should review any workforce-related action.
```

---

# Safety Notes

This topic deals with workforce readiness and manager decision support.

The agent should keep the briefing focused on learning support, certification readiness and coaching actions.

If the user asks for employment action, the agent must refuse briefly and redirect to safe readiness support.

Example refusal:

```text
I can help summarize readiness signals and suggest learning support actions, but I cannot make or automate employment, promotion, compensation or disciplinary decisions. A human manager must review any workforce action.
```

---

# Success Criteria

This topic is successful when the agent returns a briefing that is:

- grounded in the approved synthetic knowledge
- useful for a manager meeting
- concise and structured
- supportive rather than punitive
- clear about readiness risks
- clear about human review boundaries
