# Assessment Blueprint

## Document Purpose

This synthetic assessment blueprint defines how SkillForge Copilot Agent should explain readiness checks, assessment logic and source-grounded evaluation patterns for the AZ-204 demo scenario.

The blueprint is designed for manager-facing certification readiness conversations in Copilot Studio.

All content in this document is synthetic and created for demonstration purposes only.

---

# Assessment Overview

SkillForge Copilot Agent may use assessment guidance to explain how learner readiness should be reviewed before a certification attempt.

Assessments are advisory learning checks. They are intended to help managers and learners identify gaps, prioritize learning and decide when to reassess readiness.

Assessments must not be used for employment decisions.

---

# Assessment Goals

The assessment process should help answer:

- Is the learner currently above or below the readiness threshold?
- Which skill areas are blocking certification readiness?
- What practical learning actions should be prioritized?
- What should the manager review with the learner?
- When should readiness be reassessed?

---

# Supported Certification Scenario

| Field | Value |
|---|---|
| Certification | AZ-204 |
| Certification Area | Azure Developer Associate |
| Demo Team | Team Atlas |
| Demo Learner | Jamie Rivera |
| Recommended Readiness Threshold | 75 |
| Primary Skill Gaps | Authentication and Security, Azure Functions, Azure Storage |

---

# Readiness Threshold Logic

| Score Range | Readiness Level | Interpretation |
|---:|---|---|
| 75 or above | Ready | Learner is likely prepared for certification review |
| 65 to 74 | Watch List | Learner is progressing but needs monitoring |
| Below 65 | At Risk | Learner needs targeted support before certification attempt |

For the Team Atlas demo, Jamie Rivera has a readiness score of 64 and is classified as At Risk.

---

# Assessment Structure

A readiness assessment should include:

1. Certification target.
2. Current readiness score.
3. Threshold comparison.
4. Priority skill gaps.
5. Evidence-based explanation.
6. Recommended learning actions.
7. Reassessment guidance.
8. Responsible AI boundary note.

---

# Grounding Requirements

Assessment explanations should be grounded in approved synthetic knowledge sources.

Approved sources include:

- Team Atlas readiness report
- AZ-204 certification guide
- readiness playbook
- workforce learning policy
- assessment blueprint

The agent should not invent assessment criteria that are not supported by the approved knowledge sources.

If the user asks for information not covered by the available sources, the agent should say that the available synthetic knowledge does not contain enough information.

---

# Question Types

SkillForge Copilot Agent may describe or generate synthetic readiness checks using the following question types.

| Question Type | Purpose | Example Focus |
|---|---|---|
| Concept Check | Validate understanding of a key topic | Managed identity, token validation, function triggers |
| Scenario Question | Apply knowledge to a practical case | Secure API access, event-driven function workflow |
| Gap Review Question | Confirm whether a known gap is improving | Authentication and Security, Azure Functions, Azure Storage |
| Manager Discussion Prompt | Support coaching conversation | Blockers, capacity, confidence and next steps |
| Reassessment Prompt | Guide follow-up readiness review | Progress after targeted learning |

---

# Approved Skill Areas for AZ-204 Assessment

| Skill Area | Assessment Focus |
|---|---|
| Authentication and Security | Secure identity flows, authorization patterns, managed identity, token validation and secure API access |
| Azure Functions | Triggers, bindings, function execution, deployment flow and troubleshooting |
| Azure Storage | Blob storage, queues, access patterns, secure access and application integration |
| API Development | API design, request and response patterns, authentication integration and error handling |
| Application Monitoring | Logs, metrics, diagnostics and troubleshooting |
| Deployment and Configuration | Application settings, configuration management and deployment flow |

---

# Example Assessment Questions

## Authentication and Security

### Concept Check

What is the benefit of using managed identity instead of storing credentials directly in application configuration?

Expected answer summary:

A strong answer should explain that managed identity reduces secret handling risk, supports secure access to Azure resources and avoids hard-coded credentials.

### Scenario Question

A cloud application needs to call a protected API and access Azure resources securely. What security topics should the learner review first?

Expected answer summary:

A strong answer should mention authentication flows, authorization patterns, token validation, managed identity and secure API access.

---

## Azure Functions

### Concept Check

How do triggers and bindings support event-driven application development in Azure Functions?

Expected answer summary:

A strong answer should explain that triggers start function execution based on events and bindings simplify input and output integration with other services.

### Scenario Question

A learner needs to build a small event-driven workflow that reacts to storage changes. What Azure Functions concepts should they practice?

Expected answer summary:

A strong answer should mention choosing the right trigger, using bindings, understanding function execution and reviewing deployment or monitoring behavior.

---

## Azure Storage

### Concept Check

When should a learner consider blob storage or queues in an application scenario?

Expected answer summary:

A strong answer should explain that blob storage supports object storage scenarios, while queues support asynchronous messaging and workload decoupling.

### Scenario Question

A cloud application needs to store files and process work asynchronously. Which storage concepts should the learner review?

Expected answer summary:

A strong answer should mention blob storage, queues, access patterns, secure access and integration with application workflows.

---

# Assessment Feedback Pattern

When giving assessment feedback, the agent should use the following structure:

1. State the readiness result.
2. Compare the score to the threshold.
3. Identify the top gaps.
4. Explain what those gaps mean.
5. Recommend targeted learning.
6. Suggest a reassessment point.
7. Add the advisory and human review boundary.

---

# Example Feedback for Jamie Rivera

Jamie Rivera is currently classified as At Risk for AZ-204 readiness.

Jamie's readiness score is 64, which is 11 points below the recommended threshold of 75.

The highest-priority gaps are:

- Authentication and Security
- Azure Functions
- Azure Storage

The recommended next step is a targeted 13-hour learning plan focused first on Authentication and Security, followed by Azure Functions and Azure Storage practice.

Based on a weekly learning capacity of 2 hours per week, the estimated plan duration is 7 weeks.

These recommendations are advisory and intended to support certification readiness. A human manager should review any workforce-related action.

---

# Manager Assessment Review Checklist

Managers should review:

- Is the certification target clear?
- Is the learner below or above the readiness threshold?
- Which skill gaps are highest priority?
- Is the recommended learning plan realistic?
- Does the learner have enough weekly capacity?
- What support does the learner need?
- When should readiness be reassessed?
- Are all actions advisory and human-reviewed?

---

# Reassessment Guidance

A learner should be reassessed after completing targeted learning activities.

For Jamie Rivera, reassessment should occur after the 7-week targeted learning plan or after the 13 hours of focused learning have been completed.

Reassessment should focus on:

- Authentication and Security confidence
- Azure Functions scenario practice
- Azure Storage integration understanding
- ability to explain decisions in practical application scenarios
- progress against the readiness threshold

---

# Responsible AI Boundary

Assessment outputs must remain advisory.

Assessment results must not be used to:

- make hiring decisions
- make firing decisions
- make promotion decisions
- make compensation decisions
- make disciplinary decisions
- rank employees for employment action
- replace manager judgment

All workforce-related decisions require human review.

---

# Synthetic Data Policy

This assessment blueprint uses synthetic data only.

It does not contain:

- real employee data
- customer data
- personally identifiable information
- confidential company information
- production tenant data
- secrets or credentials

---

# Approved Agent Use

SkillForge Copilot Agent may use this blueprint to answer questions about:

- assessment structure
- readiness checks
- AZ-204 skill assessment focus
- expected answer summaries
- readiness threshold logic
- reassessment guidance
- manager review checklists
- responsible AI boundaries

If the requested answer is not supported by this blueprint or other approved synthetic knowledge sources, the agent should say that the available synthetic knowledge does not contain enough information.
