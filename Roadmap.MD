# Roadmap: Smart Project Risk Monitor

## Phase 1: MVP Foundation

Status: Completed

### Goals

Build the core PM risk monitoring system using Google Sheets.

### Completed Items

- Created Google Sheets workbook
- Added Projects tab
- Added Risk Register tab
- Added Tasks tab
- Added Stakeholder Updates tab
- Added AI Risk Summary tab
- Added Dashboard tab
- Added risk scoring logic
- Added sample cybersecurity project data
- Added dropdown values and structured fields
- Added dashboard metrics
- Tested Gmail alert using Google Apps Script

### Outcome

The MVP provides a working PM risk register, dashboard, stakeholder update tracker, and Critical risk alert workflow.

## Phase 2: Automation

Status: In Progress

### Goals

Automate risk scanning and notifications.

### Planned Items

- Add daily Apps Script trigger
- Scan Risk Register automatically
- Detect open Critical risks
- Send automated Gmail alerts
- Log automation runs
- Add error handling for missing data
- Add timestamp for last automation run

### Outcome

The PM receives automatic alerts when Critical risks require attention.

## Phase 3: AI Risk Summary

Status: Designed / API-ready

### Goals

Use AI to support PM decision-making and stakeholder communication.

### Planned Items

- Connect Google Apps Script to OpenAI API
- Send High and Critical risks to AI
- Generate PM-style risk summaries
- Generate recommended PM actions
- Generate escalation recommendations
- Save AI output to AI Risk Summary tab

### Current Constraint

OpenAI API usage requires available API credits. The project can still run in Free Mode using rule-based scoring and Gmail alerts.

### Outcome

The PM can quickly convert risk data into stakeholder-ready summaries.

## Phase 4: Dashboard Improvement

Status: Planned

### Goals

Improve visual reporting and executive readability.

### Planned Items

- Add better charts to Dashboard tab
- Add risk trend section
- Add project health summary
- Add owner-based risk view
- Add overdue mitigation tracker
- Add blocked tasks summary
- Add executive summary section

### Outcome

Stakeholders can understand project health quickly without reviewing the full risk register.

## Phase 5: External Tool Integrations

Status: Future

### Goals

Connect the risk monitor to real project management tools.

### Planned Integrations

- Jira API
- GitHub Issues
- Slack alerts
- Microsoft Teams alerts
- Google Forms for risk intake
- Looker Studio dashboard

### Outcome

The system becomes closer to a real PM workflow used across cross-functional teams.

## Phase 6: Portfolio Polish

Status: Planned

### Goals

Prepare the project for GitHub and PM portfolio presentation.

### Planned Items

- Add screenshots folder
- Add Dashboard screenshot
- Add Risk Register screenshot
- Add AI Risk Summary screenshot
- Add Stakeholder Updates screenshot
- Add Gmail alert screenshot
- Add Apps Script screenshot
- Add README.md
- Add PRD.md
- Add Risk-Framework.md
- Add Architecture.md
- Add Roadmap.md

### Outcome

The project clearly demonstrates PM risk assessment, stakeholder communication, automation thinking, and AI-assisted workflow design.

## Future Enhancements

- Risk trend history
- Weekly stakeholder summary email
- Executive report export
- Owner workload view
- Risk aging report
- Dependency tracker
- Decision log
- Compliance readiness tracker
- Automated risk intake form
- Role-based access control

## Final Vision

Smart Project Risk Monitor should become a lightweight PM risk intelligence system that helps Product Managers identify, prioritize, monitor, and communicate project risks before they become delivery or compliance problems.
