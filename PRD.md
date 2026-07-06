# Product Requirements Document: Smart Project Risk Monitor

## 1. Product Overview

Smart Project Risk Monitor is a PM-focused risk assessment and monitoring system for cybersecurity-related projects. It helps Product Managers track risks, score risk severity, monitor mitigation plans, identify escalation needs, and communicate project health to stakeholders.

The project uses a cybersecurity scenario, but the core purpose is to demonstrate Product Management skills such as risk assessment, prioritization, stakeholder visibility, escalation planning, and project health monitoring.

## 2. Problem Statement

Product risks are often tracked across different spreadsheets, status updates, meetings, and task trackers. This makes it difficult for a Product Manager to identify risks early, assign owners, monitor mitigation progress, and escalate critical issues before they affect delivery.

In cybersecurity projects, this problem becomes more important because delays can affect audit readiness, compliance, security posture, and stakeholder trust.

## 3. Target Users

### Primary User

- Product Manager

### Secondary Users

- Engineering Manager
- Security Lead
- Compliance Lead
- QA Lead
- Leadership / Stakeholders
- Project Team Members

## 4. Project Scenario

The company is managing several cybersecurity initiatives:

- MFA rollout
- Vulnerability remediation
- Audit evidence collection
- Access control cleanup
- Vendor security review

The Product Manager needs a centralized system to monitor delivery risk, compliance risk, ownership gaps, blocked work, mitigation plans, and escalation needs.

## 5. Goals

- Centralize project risks in one structured tracker
- Score risks using impact and probability
- Identify High and Critical risks quickly
- Track mitigation plans, owners, and due dates
- Improve stakeholder visibility
- Support PM decision-making and escalation planning
- Send alerts for Critical risks
- Optionally generate AI-assisted PM risk summaries

## 6. Non-Goals

- This is not a full cybersecurity scanning tool
- This does not replace Jira, GitHub, or enterprise GRC tools
- This does not perform technical vulnerability analysis
- This does not automatically fix project risks
- This does not replace PM judgment

## 7. MVP Scope

The MVP includes:

- Projects tracker
- Risk Register
- Tasks tracker
- Stakeholder Updates tracker
- AI Risk Summary tab
- Dashboard with key risk metrics
- Risk scoring formula
- Risk level classification
- Google Apps Script email alert for Critical risks
- Optional OpenAI API integration for PM-style summaries

## 8. Functional Requirements

### FR1: Project Tracking

The system should allow the PM to track cybersecurity projects with owner, goal, status, completion percentage, deadline, and overall risk level.

### FR2: Risk Register

The system should allow the PM to enter and manage project risks with category, description, impact, probability, score, level, owner, due date, mitigation plan, escalation status, and current status.

### FR3: Risk Scoring

The system should calculate risk score using:

Risk Score = Impact × Probability

The system should classify risks as Low, Medium, High, or Critical.

### FR4: Dashboard

The system should summarize key metrics, including:

- Total open risks
- Critical risks
- High risks
- Overdue risks
- Blocked tasks
- Escalations needed
- Projects at risk
- Risks by category
- Risks by owner

### FR5: Stakeholder Updates

The system should allow the PM to document stakeholder updates, decisions needed, action items, owners, and deadlines.

### FR6: Email Alerts

The system should send an automated email alert when open Critical risks are found.

### FR7: AI Risk Summary

The system should support optional AI-generated summaries for High and Critical risks, including:

- Overall project health
- Top risks
- Why the risks matter
- Recommended PM actions
- Escalation recommendation
- Stakeholder-ready summary

## 9. User Stories

### User Story 1

As a Product Manager, I want to view all project risks in one place so that I can identify which risks need immediate attention.

### User Story 2

As a Product Manager, I want risks to be scored by impact and probability so that I can prioritize mitigation work objectively.

### User Story 3

As a Product Manager, I want to track risk owners and due dates so that accountability is clear.

### User Story 4

As a Product Manager, I want to receive alerts for Critical risks so that I can escalate urgent issues quickly.

### User Story 5

As a stakeholder, I want a clear project health summary so that I can understand current risks without reviewing the full tracker.

## 10. Success Metrics

- 100% of active project risks have assigned owners
- 100% of Critical risks have mitigation plans
- Critical risks are escalated within 24 hours
- High and Critical risks are visible on the dashboard
- Stakeholder updates are documented weekly
- Overdue mitigation items are reduced over time
- PM can generate or prepare a stakeholder summary faster

## 11. Assumptions

- The PM or project team maintains the Risk Register
- Risk scoring uses a 1–5 impact and probability scale
- Google Sheets is sufficient for the MVP
- Gmail alerts are enough for the first version
- OpenAI API integration is optional and depends on available API credits

## 12. Risks and Constraints

- API usage may require paid credits
- Manual data entry may create quality issues
- Risk score accuracy depends on PM judgment
- The dashboard is only as accurate as the data entered
- This MVP is designed for portfolio demonstration, not enterprise deployment

## 13. Future Enhancements

- Jira or GitHub Issues integration
- Slack or Microsoft Teams alerts
- Daily automated risk scanning
- Risk trend history
- Owner workload view
- Looker Studio dashboard
- Weekly executive summary export
- Automated stakeholder report generation
