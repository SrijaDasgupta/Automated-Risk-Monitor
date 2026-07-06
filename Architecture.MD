# Architecture: Smart Project Risk Monitor

## 1. Architecture Overview

Smart Project Risk Monitor uses a simple, lightweight architecture designed for a PM portfolio project. The system is built around Google Sheets as the central workspace, with Google Apps Script used for automation and Gmail alerts.

OpenAI API integration is optional and used only to generate PM-style risk summaries.

## 2. High-Level Workflow

Google Sheets Risk Register  
→ Google Apps Script  
→ Risk Level Detection  
→ Optional OpenAI API Summary  
→ AI Risk Summary Tab  
→ Gmail Critical Risk Alert  
→ PM Dashboard / Stakeholder Review

## 3. Components

| Component | Purpose |
|---|---|
| Google Sheets | Central project tracker, risk register, dashboard, and stakeholder update system |
| Projects Tab | Tracks cybersecurity initiatives and overall project health |
| Risk Register Tab | Stores risks, scoring, owners, due dates, mitigation plans, and escalation status |
| Tasks Tab | Tracks project tasks, blockers, priorities, and due dates |
| Stakeholder Updates Tab | Documents PM updates, decisions needed, and action items |
| AI Risk Summary Tab | Stores AI-generated or manually prepared PM summaries |
| Dashboard Tab | Provides project health and risk visibility |
| Google Apps Script | Automates risk scanning and email alerts |
| Gmail | Sends Critical risk alerts |
| OpenAI API | Optional AI-generated PM risk summaries |

## 4. Data Flow

### Step 1: Risk Entry

The PM enters or updates risks in the Risk Register.

Each risk includes:

- Project name
- Risk category
- Risk description
- Impact
- Probability
- Risk score
- Risk level
- Owner
- Due date
- Mitigation plan
- Escalation status
- Current status

### Step 2: Risk Scoring

Google Sheets formulas calculate:

Risk Score = Impact × Probability

The sheet then assigns a risk level:

- Low
- Medium
- High
- Critical

### Step 3: Dashboard Update

The Dashboard tab summarizes project health using data from the Projects, Risk Register, and Tasks tabs.

Dashboard metrics include:

- Total open risks
- Critical risks
- High risks
- Overdue risks
- Blocked tasks
- Escalations needed
- Projects at risk
- Risks by category
- Risks by owner

### Step 4: Automation

Google Apps Script scans the Risk Register for open Critical risks.

If Critical risks exist, the script sends a Gmail alert to the PM.

### Step 5: Optional AI Summary

If OpenAI API credits are available, Google Apps Script can send High and Critical risks to the OpenAI API.

The AI generates:

- Overall project health
- Top risks
- Why the risks matter
- Recommended PM actions
- Escalation recommendation
- Stakeholder-ready summary

The result is stored in the AI Risk Summary tab.

## 5. Free Mode

The project can run without paid API usage.

Free Mode includes:

- Google Sheets risk tracker
- Risk scoring formulas
- PM dashboard
- Stakeholder update tracker
- Google Apps Script email alerts
- Manual AI summaries if needed

## 6. AI Mode

AI Mode includes:

- OpenAI API integration
- Automated PM-style risk summaries
- Suggested next actions
- Escalation recommendations
- Stakeholder-ready updates

API usage requires available OpenAI API credits.

## 7. Automation Logic

The automation checks for:

- Open risks
- High risks
- Critical risks
- Escalation-needed risks
- Risk status not equal to Closed or Mitigated

If an open Critical risk is found, the system sends an email alert.

## 8. Security Considerations

- API keys should not be stored in GitHub
- API keys should not be included in screenshots
- OpenAI API key should be stored in Google Apps Script Properties
- The project workbook should not contain real company security data
- Sample data should be used for portfolio demonstration

## 9. Current Limitations

- Data entry is mostly manual
- Google Sheets is not an enterprise GRC system
- OpenAI API requires credits
- Risk scoring depends on PM judgment
- Email alerts are basic in the MVP version
- No live Jira or GitHub integration yet

## 10. Future Architecture Enhancements

- Jira API integration
- GitHub Issues integration
- Slack alerts
- Microsoft Teams alerts
- Looker Studio dashboard
- Risk trend history table
- Weekly stakeholder summary email
- Automated executive report export
- Role-based access control
