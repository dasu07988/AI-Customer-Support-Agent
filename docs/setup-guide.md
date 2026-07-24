# 🛠️ Setup Guide

This guide explains how to set up and run the AI Customer Support Agent locally using n8n and Google Gemini.

---

# Requirements

Before starting, ensure you have:

- n8n installed
- Google Account
- Google Gemini API Key
- Google Sheets account
- Postman

---

# Clone the Repository

```bash
git clone https://github.com/dasu07988/AI-Customer-Support-Agent.git
```

```bash
cd AI-Customer-Support-Agent
```

---

# Import the Workflow

1. Open n8n.
2. Click **Import from File**.
3. Select:

```
workflow/AI-Customer-Support-Agent.json
```

4. Save the workflow.

---

# Configure Credentials

## Google Gemini

Create a Google Gemini API credential.

Required:

- API Key

---

## Google Sheets

Create a Google Sheets credential.

Grant access to your Google account.

---

# Update Google Sheets

Create a spreadsheet named:

```
AI Customer Support Logs
```

Add the following columns:

| Timestamp | Customer Message | Category | AI Response |
|------------|------------------|----------|-------------|

---

# Activate the Workflow

Click **Activate** in n8n.

Copy the production Webhook URL.

Example:

```
POST /webhook/customer-support
```

---

# Test with Postman

Method

```
POST
```

Headers

```
Content-Type: application/json
```

Body

```json
{
    "message":"What is your refund policy?"
}
```

---

# Expected Response

```json
{
    "Timestamp":"...",
    "Customer Message":"...",
    "Category":"General",
    "AI Response":"..."
}
```

---

# Verify Conversation Logs

Open your Google Sheet.

A new row should be added automatically after each successful request.

---

# Troubleshooting

## Invalid Credentials

Reconnect the affected credential inside n8n.

---

## Google Sheets Not Updating

- Verify spreadsheet permissions.
- Confirm column names match the workflow.

---

## Gemini Error

- Check your API key.
- Verify API quota.

---

## Webhook Returns 404

Ensure the workflow is activated.

---

# Project Structure

```
workflow/
docs/
assets/
README.md
SETUP.md
LICENSE
```

---

# Support

If you encounter any issues, please open a GitHub Issue.