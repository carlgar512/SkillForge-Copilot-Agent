# Follow-Up Message Topic

## Intent

Help a manager create a supportive follow-up message for a learner based on synthetic certification readiness information.

This topic is designed for manager-facing Copilot Studio conversations where the user wants a ready-to-review coaching message.

---

# Trigger Phrases

Use this topic when the user asks things like:

- Create a follow-up message for Jamie Rivera.
- Draft a coaching message for Jamie.
- Write a learner support message.
- Prepare a message about Jamie's AZ-204 readiness.
- Help me follow up with an at-risk learner.
- Create a supportive readiness message.
- Draft next steps for Jamie Rivera.

---

# Required Inputs

The agent should try to identify:

| Input | Required | Example |
|---|---|---|
| Learner | Yes | Jamie Rivera |
| Certification | Yes | AZ-204 |
| Readiness status | Yes | At Risk |
| Priority gaps | Yes | Authentication and Security, Azure Functions, Azure Storage |
| Tone | No | Supportive and professional |
| Message length | No | Short manager-ready message |

If learner or certification context is missing, ask a short clarification question.

Example:

```text
Which learner and certification should I use for the follow-up message?
```

---

# Knowledge Sources

Use these approved synthetic knowledge sources:

- `knowledge/team-atlas-readiness-report.md`
- `knowledge/readiness-playbook.md`
- `knowledge/workforce-learning-policy.md`
- `knowledge/certification-guide-az-204.md`

The agent should not invent learner data, readiness scores or employment-related conclusions.

---

# Response Structure

The response should include:

1. A short note that the message is a draft for manager review.
2. A ready-to-send follow-up message.
3. A brief advisory boundary note.

Recommended structure:

```text
Here is a supportive draft you can review before sending:

[Message]

Note: This is an advisory learning support message. A human manager should review it before sending.
```

---

# Example User Prompt

```text
Create a follow-up message for Jamie Rivera.
```

---

# Example Agent Answer

```text
Here is a supportive draft you can review before sending:

Hi Jamie,

Thanks for the progress you have made toward AZ-204.

Based on the current readiness review, the most useful next step is to focus on Authentication and Security first, followed by Azure Functions and Azure Storage. The goal is to use the next few weeks for targeted practice rather than broad study.

Your current plan estimates around 13 hours of focused learning. Since your available capacity is around 2 hours per week, we should treat this as a realistic 7-week support plan and review progress weekly.

This is intended to support your certification preparation, not as a performance or employment decision. Let’s review your capacity together and agree on the best next steps.

Best,
[Manager Name]

Note: This message is advisory and should be reviewed by a human manager before sending.
```

---

# Tone Requirements

The message should be:

- supportive
- professional
- concise
- coaching-oriented
- non-punitive
- capacity-aware
- practical

The message should avoid:

- blame
- threats
- employment consequences
- performance judgment
- disciplinary language
- promotion or compensation references

---

# Safety Notes

The agent must not:

- imply that readiness score is a performance rating
- recommend employment action
- mention promotion, compensation, discipline or termination unless refusing an unsafe request
- expose unsupported personal information
- ask for private HR data
- use punitive language

The agent should always make clear that follow-up messages are drafts for human review.

---

# Responsible AI Boundary

Follow-up messages are for learning support only.

They must not be used to automate or justify hiring, firing, promotion, compensation, disciplinary or employment decisions.

A human manager must review any message before sending it to a learner.

---

# Expected Outcome

The topic should produce a message that a manager can review and adapt before sending to the learner.

The output should help the manager communicate:

- current readiness context
- priority learning focus
- realistic next steps
- supportive tone
- human review boundary
