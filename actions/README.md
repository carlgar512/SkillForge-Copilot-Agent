# Actions

## Purpose

This folder documents the action strategy for SkillForge Copilot Agent.

The agent is designed as a Copilot Studio enterprise assistant for manager-facing certification readiness workflows. Its core behavior is based on agent instructions, curated synthetic knowledge sources and defined conversation topics.

## Action Strategy

SkillForge Copilot Agent is designed to operate safely with approved synthetic knowledge sources.

The reference implementation does not require production connectors, external APIs or live Microsoft tenant data to demonstrate the manager readiness scenario.

This design keeps the agent reproducible, transparent and safe for public submission.

## Data Boundary

The agent must not connect to or process:

- real employee databases
- production HR systems
- payroll systems
- performance management systems
- confidential enterprise systems
- real Microsoft tenant data
- customer data
- personally identifiable information
- secrets or credentials

All readiness data used by the project is synthetic and documented in the `knowledge/` folder.

## Supported Action Patterns

The following action patterns describe how the agent could be extended in an enterprise environment while preserving responsible AI boundaries.

These action patterns are documented as architecture references only.

| Action Pattern | Purpose | Input | Output |
|---|---|---|---|
| `getTeamReadiness` | Retrieve team-level readiness information | Team ID, certification ID | Team readiness summary, readiness index, risk level |
| `getLearnerReadiness` | Retrieve learner-level readiness information | Learner ID, certification ID | Learner score, threshold, priority gaps, recommended support |
| `generateManagerBriefing` | Generate an executive manager briefing | Team ID, certification ID | Briefing with risks, actions and decision boundaries |
| `createFollowUpDraft` | Draft a learner support message | Learner ID, certification ID, tone | Supportive follow-up draft |
| `validateWorkforceBoundary` | Check whether a request is within responsible use limits | User request | Allowed, advisory-only, or refused response pattern |

## Future Enterprise Extension

In a production enterprise environment, these action patterns could be implemented through:

- Copilot Studio actions
- Power Automate flows
- Microsoft Graph connectors
- Dataverse tables
- secure internal APIs
- Microsoft Entra ID authentication
- role-based access control

Any future implementation should preserve the same safety principles:

- use least-privilege access
- avoid exposing confidential information
- keep human review for workforce-related actions
- avoid automated employment decisions
- log action execution for auditability
- validate outputs before presenting recommendations

## Responsible AI Boundary

Actions must not be used to automate or recommend:

- hiring decisions
- firing decisions
- promotion decisions
- compensation decisions
- disciplinary decisions
- employment rankings
- performance penalties

Actions may support:

- learning recommendations
- certification readiness review
- manager briefing preparation
- learner coaching support
- workload-aware learning planning
- human-reviewed advisory workflows

## Security Requirements for Future Actions

Any implemented action should follow these requirements:

1. Do not hard-code secrets.
2. Use environment variables or managed identity where applicable.
3. Use Microsoft Entra ID authentication for enterprise access.
4. Apply least-privilege permissions.
5. Validate all inputs.
6. Avoid returning unnecessary personal data.
7. Keep audit logs for action execution.
8. Block unsupported employment decision requests.
9. Document all data sources.
10. Use synthetic data for demos and public submissions.

## Approved Agent Behavior

When actions are unavailable or not connected, the agent should answer using the approved synthetic knowledge sources.

If the requested information is not available in the approved knowledge sources, the agent should clearly say that the available synthetic knowledge does not contain enough information.

The agent must not claim access to live enterprise systems unless those systems are explicitly connected and documented.
