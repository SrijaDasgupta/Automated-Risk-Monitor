# Risk Framework: Smart Project Risk Monitor

## 1. Purpose

This document defines the risk assessment framework used in Smart Project Risk Monitor. The goal is to show how a Product Manager can identify, score, prioritize, monitor, and escalate project risks in a structured way.

The framework is designed for cybersecurity-related projects, but it can be applied to any product or delivery environment.

## 2. Risk Categories

Risks are grouped into the following categories:

| Category | Description |
|---|---|
| Delivery | Risks that may delay project timelines or milestones |
| Security | Risks that may affect security posture or unresolved findings |
| Compliance | Risks that may affect audit readiness or policy requirements |
| Dependency | Risks caused by another team, vendor, or system dependency |
| Resource | Risks caused by limited team capacity or unavailable resources |
| Ownership | Risks caused by unclear owners or missing accountability |
| Communication | Risks caused by unclear updates, missed decisions, or stakeholder misalignment |

## 3. Risk Scoring Model

Each risk is scored using two factors:

- Impact
- Probability

Risk Score = Impact × Probability

## 4. Impact Scale

| Impact Score | Meaning |
|---|---|
| 1 | Minimal impact; no major delivery or stakeholder concern |
| 2 | Minor impact; manageable within the team |
| 3 | Moderate impact; may affect timeline or quality |
| 4 | High impact; may affect delivery, compliance, or stakeholder confidence |
| 5 | Severe impact; may cause major delay, audit issue, or critical exposure |

## 5. Probability Scale

| Probability Score | Meaning |
|---|---|
| 1 | Unlikely |
| 2 | Possible but not expected |
| 3 | Moderate chance of occurring |
| 4 | Likely to occur |
| 5 | Very likely or already happening |

## 6. Risk Level Classification

| Risk Score | Risk Level | PM Action |
|---|---|---|
| 1–5 | Low | Monitor during regular updates |
| 6–10 | Medium | Track mitigation plan and owner |
| 11–15 | High | Review frequently and prepare escalation if needed |
| 16–25 | Critical | Escalate quickly and track mitigation closely |

## 7. Escalation Rules

A risk should be marked for escalation if any of the following are true:

- Risk Level is Critical
- Risk Level is High and the due date is within 7 days
- No owner is assigned
- Mitigation plan is missing
- The risk has been blocked for more than 3 business days
- The risk affects audit readiness or compliance deadline
- The risk requires leadership decision or additional resources

## 8. Mitigation Tracking

Each risk should include:

- Risk owner
- Due date
- Mitigation plan
- Current status
- Escalation status
- Last updated date
- PM notes

A strong mitigation plan should explain:

- What action will reduce the risk
- Who owns the action
- When the action is due
- What decision or support is needed
- How the PM will monitor progress

## 9. Risk Status Definitions

| Status | Meaning |
|---|---|
| Open | Risk is active and needs attention |
| Monitoring | Risk is being watched but does not need immediate action |
| Mitigated | Risk has been reduced but may still need follow-up |
| Closed | Risk is no longer active |

## 10. PM Review Cadence

| Risk Level | Review Frequency |
|---|---|
| Low | Weekly or biweekly |
| Medium | Weekly |
| High | 2–3 times per week |
| Critical | Daily until mitigated |

## 11. Example Risks

| Risk | Category | PM Concern |
|---|---|---|
| Critical vulnerabilities remain unresolved | Security | Security exposure and audit risk |
| MFA adoption is below target | Compliance | Users may miss compliance deadline |
| Access review has missing owners | Ownership | Accountability gap |
| Vendor security questionnaire is incomplete | Dependency | External blocker |
| Audit evidence is spread across teams | Delivery | Delayed audit readiness |
| Security team capacity is constrained | Resource | Mitigation timeline risk |

## 12. PM Decision Logic

The Product Manager should use the risk framework to decide:

- Which risks need immediate action
- Which risks require escalation
- Which owners need follow-up
- Which deadlines are at risk
- Which risks should be included in stakeholder updates
- Which mitigation plans need leadership support

## 13. Portfolio Relevance

This framework demonstrates core Product Management skills:

- Risk identification
- Risk scoring
- Prioritization
- Mitigation planning
- Ownership tracking
- Stakeholder communication
- Escalation management
- Decision-making under uncertainty
