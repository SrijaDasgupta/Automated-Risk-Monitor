# Smart Project Risk Monitor

## Overview

Smart Project Risk Monitor is a PM-focused risk assessment and monitoring project designed for cybersecurity-related initiatives. The goal is to help Product Managers identify project risks early, track mitigation plans, monitor ownership, and escalate critical issues before they impact delivery or compliance.

This project uses a cybersecurity scenario, but the main focus is Product Management risk assessment, stakeholder visibility, and project health monitoring.

## Project Scenario

A company is managing multiple cybersecurity initiatives, including MFA rollout, vulnerability remediation, audit evidence collection, access control cleanup, and vendor security review.

The Product Manager needs a simple system to track delivery risks, compliance risks, ownership gaps, blocked tasks, mitigation plans, and escalation needs in one place.

## Problem Statement

Project risks are often spread across spreadsheets, task trackers, team updates, and status reports. This makes it difficult for PMs to identify risks early, prioritize mitigation work, and communicate project health clearly to stakeholders.

Smart Project Risk Monitor centralizes risk tracking through a structured risk register, PM dashboard, AI-ready risk summary, stakeholder update tracker, and automated critical risk alerts.

## Goals

- Track project risks in one place
- Score risks using impact and probability
- Identify High and Critical risks quickly
- Monitor owners, due dates, and mitigation plans
- Support stakeholder updates and escalation planning
- Send automated email alerts for Critical risks
- Optionally use AI to generate PM-style risk summaries

## Tools Used

- Google Sheets
- Google Apps Script
- Gmail alerts
- OpenAI API optional
- Excel workbook
- GitHub documentation

## Key Features

### Risk Register

The Risk Register tracks risk category, risk description, impact, probability, risk score, risk level, owner, due date, mitigation plan, escalation status, and current status.

### Risk Scoring

Risks are scored using:

Risk Score = Impact × Probability

Risk levels:

| Score | Risk Level |
|---|---|
| 1–5 | Low |
| 6–10 | Medium |
| 11–15 | High |
| 16–25 | Critical |

### PM Dashboard

The dashboard summarizes total open risks, Critical risks, High risks, overdue risks, blocked tasks, escalations needed, projects at risk, risks by category, and risks by owner.

### Stakeholder Updates

The stakeholder update tracker documents risk escalations, weekly status updates, decisions needed, action items, owners, due dates, and current status.

### AI Risk Summary

The AI Risk Summary tab is designed to generate PM-style summaries including overall project health, top risks, why the risks matter, recommended PM actions, escalation recommendation, and stakeholder-ready updates.

The project supports two modes:

| Mode | Description |
|---|---|
| Free Mode | Rule-based risk scoring and Gmail alerts |
| AI Mode | OpenAI API generates PM-style risk summaries |

### Automated Email Alerts

Google Apps Script scans the Risk Register and sends an email alert when open Critical risks are found. This helps the PM act on urgent risks quickly and escalate before the issue affects delivery.

## Workflow

Google Sheets Risk Register  
→ Google Apps Script  
→ Risk Level Detection  
→ Optional OpenAI API Summary  
→ AI Risk Summary Tab  
→ Gmail Critical Risk Alert  
→ PM Dashboard / Stakeholder Review

## PM Skills Demonstrated

- Risk identification
- Risk scoring and prioritization
- RAID-style tracking
- Stakeholder communication
- Escalation planning
- Mitigation ownership
- Dashboard-based monitoring
- Cybersecurity project awareness
- AI-assisted workflow design
- Automation thinking
- Product documentation

## Current Status

MVP completed:

- Google Sheets workbook created
- Projects tab created
- Risk Register built
- Tasks tracker added
- PM dashboard created
- Stakeholder Updates tab added
- AI Risk Summary tab added
- Apps Script email alert tested successfully
- OpenAI API integration designed and API-ready

Note: OpenAI API usage requires available API credits. The project can still run in free mode using rule-based scoring and Gmail alerts.

## Future Enhancements

- Add daily automated trigger for risk scanning
- Connect Jira or GitHub Issues as a project data source
- Add Slack alerts
- Add risk trend history
- Add owner workload view
- Add Looker Studio dashboard
- Add executive summary export
- Add automated weekly stakeholder report

## Security Note

API keys should not be stored in GitHub or shown in screenshots. The OpenAI API key should be stored securely using Google Apps Script Properties.

## Portfolio Summary

Smart Project Risk Monitor is an AI-assisted PM risk monitoring tool for cybersecurity projects. It helps Product Managers identify, score, prioritize, and communicate project risks through a structured dashboard, risk register, stakeholder update tracker, and automated critical risk alerts.
