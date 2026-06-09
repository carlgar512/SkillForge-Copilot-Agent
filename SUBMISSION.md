# SkillForge Copilot Agent — Submission

## Project Name

SkillForge Copilot Agent

---

## Tagline

A Copilot Studio enterprise agent for manager-ready certification readiness briefings.

---

## Challenge Track

Enterprise Agents for Microsoft 365 Copilot

---

## Project Summary

SkillForge Copilot Agent is a Copilot Studio enterprise agent that helps managers review certification readiness, understand learner risk, generate manager-ready briefings and draft supportive learner follow-up messages.

The agent is designed for workforce certification readiness scenarios where managers need quick, safe and actionable insight from approved knowledge sources.

It uses synthetic readiness documents, structured conversation topics and Responsible AI boundaries to produce grounded, advisory and human-reviewed outputs.

---

## Problem Statement

Managers responsible for certification programs often need to answer readiness questions quickly:

- Which learners may need additional support?
- Which skill gaps should be prioritized?
- Why is a learner classified as at risk?
- What should be included in a manager readiness briefing?
- How can a learner follow-up message be supportive and non-punitive?
- Which workforce decisions must remain outside the agent boundary?

Traditional reports and dashboards may contain the information, but they often require manual interpretation before a manager can act.

SkillForge Copilot Agent turns synthetic readiness knowledge into concise, manager-ready conversations and reusable outputs.

---

## Solution

SkillForge Copilot Agent provides a Copilot Studio agent experience for manager-facing certification readiness workflows.

The agent can:

- summarize team readiness
- explain learner readiness status
- identify priority certification gaps
- generate manager briefings
- draft learner follow-up messages
- explain advisory-only Responsible AI boundaries
- refuse unsafe workforce decision requests

The agent is grounded in approved synthetic knowledge sources and does not rely on real employee data, customer data, credentials or production tenant information.

---

## Primary Demo Scenario

The demo focuses on a fictional workforce readiness scenario:

| Item | Value |
|---|---|
| Team | Team Atlas |
| Certification | AZ-204 |
| Team readiness index | 69 |
| Team status | Watch List |
| Learner | Jamie Rivera |
| Learner readiness score | 64 |
| Readiness threshold | 75 |
| Learner status | At Risk |
| Targeted learning effort | 13 hours |
| Weekly learning capacity | 2 hours per week |
| Estimated plan duration | 7 weeks |

Priority gaps:

- Authentication and Security
- Azure Functions
- Azure Storage

All scenario data is synthetic.

---

## Core Features

| Feature | Description |
|---|---|
| Team readiness review | Summarizes team readiness, risk level, at-risk learners and manager actions. |
| Learner readiness summary | Explains readiness score, threshold, skill gaps, learning effort and capacity. |
| Manager briefing generation | Produces an executive-style briefing for readiness review conversations. |
| Follow-up message drafting | Creates supportive learner follow-up messages for human review. |
| Responsible AI boundary | Refuses promotion, compensation, disciplinary and employment decision requests. |
| Synthetic knowledge grounding | Uses approved fictional readiness documents as the source of truth. |

---

## Technologies Used

| Technology | Role |
|---|---|
| Microsoft Copilot Studio | Agent design and manager-facing conversational experience. |
| Microsoft 365 Copilot experience | Target enterprise user experience for manager workflows. |
| Markdown knowledge sources | Synthetic documents used to ground the agent. |
| Mermaid | Architecture and flow diagrams. |
| GitHub | Public repository and project documentation. |

---

## Microsoft IQ Integration

SkillForge Copilot Agent demonstrates Microsoft IQ concepts through knowledge grounding, work context and semantic business meaning.

| Microsoft IQ Layer | Project Usage |
|---|---|
| Foundry IQ-style grounding | Synthetic readiness documents provide the source of truth for team, learner and certification answers. |
| Work IQ-style context | Synthetic workload and weekly capacity signals shape readiness explanations and support recommendations. |
| Fabric IQ-style semantics | Team, learner, certification, skill gap, threshold and readiness relationships structure the scenario. |

The agent applies these IQ concepts to produce responses that are grounded, practical and manager-ready.

---

## Architecture Summary

The architecture follows a simple enterprise agent pattern:

```text
Manager / Learning Lead
        ↓
Microsoft 365 Copilot Experience
        ↓
SkillForge Copilot Agent in Copilot Studio
        ↓
Instructions + Topics + Synthetic Knowledge + Responsible AI Boundaries
        ↓
Manager-ready readiness outputs
```

The repository includes Mermaid diagrams for:

- enterprise agent architecture
- conversation flow
- Responsible AI boundary
- knowledge grounding map

---

## Knowledge Sources

The agent is grounded in the following synthetic knowledge sources:

| File | Purpose |
|---|---|
| `knowledge/team-atlas-readiness-report.md` | Team Atlas readiness data and Jamie Rivera scenario. |
| `knowledge/certification-guide-az-204.md` | Synthetic AZ-204 readiness model. |
| `knowledge/readiness-playbook.md` | Readiness status definitions and manager action patterns. |
| `knowledge/workforce-learning-policy.md` | Safe use policy and workforce decision boundaries. |
| `knowledge/assessment-blueprint.md` | Readiness assessment structure and review guidance. |

---

## Conversation Topics

The project defines the following conversation topics:

| Topic | Purpose |
|---|---|
| `topics/team-readiness-review.md` | Handles team readiness questions. |
| `topics/learner-readiness-summary.md` | Explains individual learner readiness. |
| `topics/manager-briefing.md` | Generates manager briefings. |
| `topics/follow-up-message.md` | Drafts learner follow-up messages. |
| `topics/responsible-ai-boundary.md` | Handles unsafe workforce decision requests. |

---

## Responsible AI and Safety

SkillForge Copilot Agent is advisory-only.

The agent supports:

- certification readiness review
- learning support
- skill gap explanation
- manager briefing preparation
- learner follow-up drafting

The agent does not:

- make hiring decisions
- make firing decisions
- make promotion decisions
- determine compensation
- recommend disciplinary action
- automate employment decisions
- rank employees for employment action
- infer protected characteristics

All workforce-related recommendations require human review.

---

## Data and Privacy Statement

This project uses synthetic data only.

The repository does not include:

- real employee data
- customer data
- personally identifiable information
- confidential enterprise data
- production tenant data
- API keys
- credentials
- secrets

The scenario is intentionally fictional and safe for a public GitHub repository.

---

## Demo Video

Demo video link:

```text
REPLACE_WITH_YOUTUBE_OR_VIMEO_LINK
```

Recommended demo flow:

1. Show the Copilot Studio agent setup.
2. Show the configured instructions.
3. Show the synthetic knowledge sources.
4. Ask which learners in Team Atlas are at risk for AZ-204.
5. Ask why Jamie Rivera is at risk.
6. Generate a manager briefing.
7. Generate a learner follow-up message.
8. Ask whether the agent can decide who should be promoted.
9. Close with the Responsible AI and synthetic-data-only message.

---

## Repository Link

Repository link:

```text
https://github.com/carlgar512/SkillForge-Copilot-Agent
```

---

## Architecture Diagram

Architecture diagram location:

```text
diagrams/01-enterprise-agent-architecture.mmd
```

Optional exported image location:

```text
screenshots/01-enterprise-agent-architecture.png
```

---

## How to Review the Project

Reviewers can inspect:

1. `README.md` for the project overview.
2. `agent-instructions.md` for the agent behavior.
3. `knowledge/` for synthetic grounding documents.
4. `topics/` for the conversation design.
5. `docs/test-prompts.md` for test prompts and expected behavior.
6. `docs/architecture.md` for architecture explanation.
7. `diagrams/` for Mermaid diagrams.
8. `docs/demo-script.md` for the video flow.

---

## Example Demo Prompts

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

## Project Differentiation

SkillForge Copilot Agent is not a generic chatbot.

It is a focused enterprise agent for a realistic manager workflow:

- It transforms readiness knowledge into manager-ready outputs.
- It keeps workforce decisions advisory and human-reviewed.
- It uses synthetic knowledge sources for safe public demonstration.
- It demonstrates Microsoft IQ concepts through grounding, work context and semantic business structure.
- It documents the agent design clearly enough to be reviewed and recreated.

---

## Final Submission Statement

SkillForge Copilot Agent brings certification readiness intelligence into a manager-ready Copilot experience.

It combines Copilot Studio, synthetic knowledge grounding, structured conversation topics and Responsible AI boundaries to deliver practical workforce readiness support while preserving human accountability for workforce-related decisions.
