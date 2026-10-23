# AI-Powered Email Automation Using n8n and Gmail

## Overview

This project uses **n8n, an AI Agent, and the Gmail API** to automate email composition and sending. The workflow takes a user's request, uses an AI Agent to interpret the instructions and prepare the email, and uses Gmail to send it.

The goal is to reduce repetitive email-writing tasks and demonstrate how AI can be integrated with workflow automation tools.

## Features

- Natural-language instructions for email composition
- AI-assisted email subject and body generation
- Gmail integration for sending emails
- Consistent email sign-off: "Regards, Kajal"
- OAuth 2.0 authentication for Gmail
- Visual, low-code workflow orchestration using n8n

## Technology Stack

- **n8n** — workflow automation
- **AI Agent / language model** — interprets instructions and generates email content
- **Gmail API** — sends emails
- **Google OAuth 2.0** — account authorization

## Workflow

1. The user provides an email request.
2. The AI Agent interprets the request and prepares the subject and message.
3. The Gmail tool sends the email using the connected account.
4. The workflow returns the execution result.

## Project Structure

```text
n8n-ai-email-automation/
├── README.md
├── workflow/
│   └── ai_email_automation.json
└── screenshots/
    └── workflow_overview.png
```

## Setup Instructions

1. Install or access an n8n instance.
2. Import `workflow/ai_email_automation.json` into n8n.
3. Configure the AI model connection required by the workflow.
4. Create a Gmail OAuth2 credential and authorize your own Google account.
5. Select your credentials in the relevant nodes.
6. Test the workflow with a sample email before using it for real messages.

**Note:** The workflow JSON does not provide working credentials. Each user must configure their own authorized accounts and any required API access.

## Security

- Never commit OAuth client secrets, access tokens, passwords, or API keys.
- Review the exported workflow JSON before publishing it.
- Use your own credentials when importing and testing the workflow.

## Learning Outcomes

This project provided hands-on practice with AI-assisted automation, API integrations, OAuth 2.0 authentication, visual workflow design, and troubleshooting multi-step integrations.

## Future Improvements

- Add email approval before sending
- Add error handling and retry logic
- Log execution outcomes for monitoring
- Extend the workflow to support reusable email templates

## Author

Kajal Kumari

[LinkedIn](https://www.linkedin.com/in/kajalkumari29/)
