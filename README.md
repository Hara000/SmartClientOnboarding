# Smart Client Onboarding Agent

An automated AI-powered onboarding pipeline built with N8N, GPT-4o mini, and Google APIs. Deployed and live on Railway.

## What it does

When a new client submits an intake form, the agent:

1. Receives the form data via **Tally webhook**
2. Processes and structures the information through a **GPT-4o mini AI agent**
3. Automatically creates a personalized **Google Drive folder and document**
4. Sends a customized **welcome email via Gmail API**
5. Logs the client record to a **PostgreSQL database (Neon)**

Zero human intervention required from form submission to full client setup.

## Tech Stack

| Tool | Purpose |
|------|---------|
| N8N | Workflow orchestration |
| GPT-4o mini | AI agent / data processing |
| Tally | Client intake form + webhook trigger |
| Google Drive API | Automated folder and document creation |
| Gmail API | Personalized email delivery |
| PostgreSQL (Neon) | Client data storage |
| Railway | Cloud deployment and hosting |

## Architecture

Tally Form → Webhook → N8N → GPT-4o mini Agent
↓
Google Drive (folder + doc created)
↓
Gmail (welcome email sent)
↓
PostgreSQL (client record logged)

## Status

Live and deployed on Railway.

## Author

Brenda — AI Agent Engineer & Automation Developer  
[GitHub](https://github.com/Hara000)
