# SkillForge Copilot Agent — Demo Script

## Demo Goal

Demonstrate how SkillForge Copilot Agent helps managers review certification readiness, generate manager-ready briefings and prepare supportive learner follow-up messages using Copilot Studio and approved synthetic knowledge sources.

The demo shows a business-ready Enterprise Agent experience for Microsoft 365 Copilot-style workflows.

---

# Demo Duration

Recommended duration: 2 to 3 minutes.

Maximum allowed video duration: 5 minutes.

---

# Demo Story

Managers need fast, safe and actionable visibility into certification readiness without reviewing long reports, spreadsheets or dashboards.

SkillForge Copilot Agent turns approved synthetic readiness knowledge into clear manager briefings, learner explanations and advisory follow-up messages.

The agent is grounded in synthetic knowledge sources and includes Responsible AI boundaries for workforce-related recommendations.

---

# Key Message

SkillForge Copilot Agent brings workforce certification readiness into an enterprise Copilot experience: grounded, advisory, synthetic-data-only and safe for manager review.

---

# Demo Assets to Show

During the demo, show:

1. Copilot Studio agent overview.
2. Agent instructions.
3. Knowledge sources.
4. Test chat with team readiness question.
5. Manager briefing output.
6. Follow-up message output.
7. Responsible AI boundary response.
8. Repository structure if useful.

---

# Demo Flow

## 0:00 — 0:20 Introduction

### Narration

Managers often need to understand certification readiness quickly: who is at risk, which skill gaps matter and what support actions should be prioritized.

SkillForge Copilot Agent is a Copilot Studio enterprise agent that helps managers generate readiness summaries, manager briefings and learner follow-up messages using approved synthetic knowledge sources.

### Screen

Show:

- project title
- Copilot Studio agent overview
- repository README or agent overview

---

## 0:20 — 0:45 Agent Setup

### Narration

The agent is configured with manager-facing instructions, curated synthetic knowledge sources and defined conversation topics.

It does not use real employee data, customer data, confidential information or production tenant data.

### Screen

Show:

- agent instructions
- knowledge sources
- topic list

### Key Points

Mention:

- synthetic knowledge only
- manager-facing responses
- advisory-only recommendations
- human review boundary

---

## 0:45 — 1:20 Team Readiness Review

### Prompt

```text
Which learners in Team Atlas are at risk for AZ-204?
```

### Expected Answer Should Include

- Team Atlas readiness index: 69
- Team status: Watch List
- Jamie Rivera is At Risk
- Jamie readiness score: 64
- AZ-204 threshold: 75
- Priority gaps:
  - Authentication and Security
  - Azure Functions
  - Azure Storage
- Recommended manager actions
- Advisory-only note

### Narration

The manager can ask a natural readiness question. The agent uses the Team Atlas readiness report and returns a concise manager-ready summary.

It identifies Jamie Rivera as at risk, explains the score against the threshold and highlights the priority gaps that should be addressed.

---

## 1:20 — 1:55 Learner Readiness Explanation

### Prompt

```text
Why is Jamie Rivera at risk for AZ-204?
```

### Expected Answer Should Include

- Jamie Rivera
- Certification: AZ-204
- Readiness score: 64
- Threshold: 75
- Gap to threshold: 11 points
- Targeted learning required: 13 hours
- Weekly capacity: 2 hours per week
- Estimated plan duration: 7 weeks
- Coaching-oriented support recommendation

### Narration

The agent can explain the reasoning behind a learner status in plain language.

Instead of returning only a score, it connects readiness, skill gaps, learning effort and weekly capacity into an actionable explanation.

---

## 1:55 — 2:35 Manager Briefing

### Prompt

```text
Generate a manager briefing for Team Atlas.
```

### Expected Answer Should Include

- Executive summary
- Key risks
- Recommended manager actions
- Discussion points
- Next steps
- Human review note

### Narration

The agent can transform readiness data into an executive briefing that a manager can use before a certification review meeting.

This is the enterprise productivity value: the agent does not only answer questions, it prepares manager-ready outputs.

---

## 2:35 — 3:10 Follow-Up Message

### Prompt

```text
Create a follow-up message for Jamie Rivera.
```

### Expected Answer Should Include

- Supportive tone
- Recognition of progress
- Priority focus areas
- Suggested next steps
- Capacity-aware plan
- Non-punitive language
- Advisory note

### Narration

The agent can draft a supportive coaching message for the learner.

The response avoids punitive language and frames the follow-up as learning support, not a performance or employment action.

---

## 3:10 — 3:40 Responsible AI Boundary

### Prompt

```text
Can this agent decide who should be promoted?
```

### Expected Answer Should Include

- Clear refusal
- Advisory-only boundary
- No promotion, compensation, disciplinary or employment decisions
- Human manager review requirement
- Redirect to supported readiness assistance

### Narration

The agent includes clear workforce decision boundaries.

It can summarize readiness signals and recommend learning support, but it cannot make or automate promotion, compensation, disciplinary or employment decisions.

---

## 3:40 — 4:00 Closing

### Narration

SkillForge Copilot Agent demonstrates a business-ready Enterprise Agent for manager-facing certification readiness.

It combines Copilot Studio, synthetic knowledge grounding, conversation topics and Responsible AI boundaries to deliver safe, practical and manager-ready outputs.

The project is designed to be transparent, reproducible and safe for public submission.

---

# Recommended Demo Prompts

Use these prompts in order:

```text
Which learners in Team Atlas are at risk for AZ-204?
```

```text
Why is Jamie Rivera at risk for AZ-204?
```

```text
Generate a manager briefing for Team Atlas.
```

```text
Create a follow-up message for Jamie Rivera.
```

```text
Can this agent decide who should be promoted?
```

---

# Demo Checklist

Before recording, confirm:

- The agent instructions are visible and aligned with the repository.
- Knowledge sources are uploaded or configured.
- The five demo prompts work as expected.
- The responses mention synthetic data and advisory boundaries where appropriate.
- No real employee data or confidential information appears on screen.
- No credentials, tenant secrets or private URLs are visible.
- The demo stays under 5 minutes.

---

# Closing Line

SkillForge Copilot Agent brings certification readiness intelligence into a manager-ready Copilot experience: grounded, synthetic-data-only, advisory and safe for human review.
