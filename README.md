# Phishing Incident Investigation

## Overview

This project is a simulated Security Operations Centre (SOC) phishing investigation case study. It analyses a suspicious email, extracts indicators of compromise, maps the activity to MITRE ATT&CK, assesses risk, and recommends remediation actions.

The project is designed to demonstrate practical SOC analyst skills such as email analysis, IOC extraction, incident documentation, threat intelligence enrichment, and security reporting.

> Note: This is a safe simulation. All suspicious domains and URLs use reserved `.example` domains and are not real malicious infrastructure.

## Scenario

A finance employee reports an email claiming to be from PayPal. The email states that the recipient's account has been limited and asks the user to verify their account through a suspicious link.

## Repository Structure

```text
Phishing-Incident-Investigation/
├── README.md
├── reports/
│   └── Investigation_Report.pdf
├── data/
│   ├── sample_phishing_email.eml
│   ├── Indicators_of_Compromise.csv
│   ├── MITRE_ATTCK_Mapping.csv
│   └── Incident_Timeline.csv
├── playbooks/
│   └── Analyst_Checklist.md
└── screenshots/
    ├── email_sample.png
    ├── ioc_summary.png
    └── mitre_mapping.png
```

## Investigation Objectives

- Analyse suspicious email content
- Identify phishing and social engineering indicators
- Extract indicators of compromise
- Map observed activity to MITRE ATT&CK
- Assess risk and business impact
- Recommend containment, eradication, and prevention actions
- Produce a professional incident investigation report

## Key Findings

The email was assessed as a credential phishing attempt.

Main indicators:

- Brand impersonation
- Typosquatted sender domain
- Urgency-based social engineering
- Suspicious verification link
- Generic greeting
- Credential harvesting intent

## Indicators of Compromise

| IOC Type | Indicator | Notes |
|---|---|---|
| Sender Email | security-update@paypa1-support.example | Uses typosquatting |
| Sender Domain | paypa1-support.example | Impersonates PayPal |
| URL | hxxp://paypal-security-verification-login.example/login | Credential harvesting lure |
| Subject | Urgent: Your PayPal Account Has Been Limited | Urgency/fear tactic |

## MITRE ATT&CK Mapping

| Technique ID | Technique | Reason |
|---|---|---|
| T1566 | Phishing | Email-based social engineering |
| T1204 | User Execution | User is encouraged to click a link |
| T1583.001 | Acquire Infrastructure: Domains | Lookalike domain used for impersonation |

## Recommended Response Actions

- Block the suspicious sender domain and URL
- Search mail logs for similar messages
- Identify users who received or clicked the email
- Reset credentials for affected users
- Enforce multi-factor authentication
- Add detection logic for similar typosquatted domains
- Conduct phishing awareness training

## Skills Demonstrated

- SOC investigation workflow
- Email analysis
- IOC extraction
- MITRE ATT&CK mapping
- Incident response reporting
- Risk assessment
- Security recommendations
- Documentation for GitHub portfolio

## Author

Riza Khan  
Cybersecurity Student
