# 🤖 AI Customer Support Agent

<p align="center">
  <img src="assets/banner.png" alt="AI Customer Support Agent Banner" width="100%">
</p>

<p align="center">

![Status](https://img.shields.io/badge/Status-In%20Development-success)
![Version](https://img.shields.io/badge/Version-v1.0-blue)
![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-orange)
![Google Gemini](https://img.shields.io/badge/Google-Gemini-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Open Source](https://img.shields.io/badge/Open%20Source-Yes-black)

</p>

> **An AI-powered customer support automation system built with n8n and Google Gemini to automate customer interactions, retrieve business knowledge, and deliver intelligent responses.**

---

# 📖 Table of Contents

* Overview
* Business Problem
* Solution
* Features
* System Architecture
* Workflow
* Technology Stack
* Repository Structure
* Prerequisites
* Installation
* Configuration
* Usage
* Sample Conversation
* Documentation
* Development Roadmap
* Screenshots
* Demo
* Future Improvements
* Contributing
* License
* Author

---

# 🚀 Overview

AI Customer Support Agent is an enterprise-inspired AI automation project designed to demonstrate how modern businesses can automate customer support using workflow automation and Generative AI.

The system receives customer inquiries, understands customer intent using Google Gemini, retrieves relevant information from a knowledge base, generates intelligent responses, and automatically delivers those responses through supported communication channels.

This project is built as a portfolio project to showcase practical skills in AI workflow automation, API integration, prompt engineering, and modern business automation.

---

# 🎯 Business Problem

Customer support teams often face challenges such as:

* Slow response times
* Repetitive customer questions
* High operational costs
* Inconsistent responses
* Manual ticket handling
* Limited support outside business hours

These issues reduce productivity and negatively affect customer satisfaction.

---

# 💡 Solution

The AI Customer Support Agent automates repetitive support tasks by combining Artificial Intelligence with workflow automation.

The system can:

* Receive customer requests
* Understand customer intent
* Search company knowledge
* Generate intelligent responses
* Send replies automatically
* Log customer interactions
* Support future enterprise RAG capabilities

---

# ✨ Features

## Version 1

* AI-powered customer support
* Google Gemini integration
* Telegram chatbot
* Gmail notifications
* Google Sheets logging
* FAQ knowledge base
* Webhook API

## Planned Features

* Conversation memory
* Human handoff
* Ticket creation
* Escalation workflow
* Pinecone vector database
* Retrieval-Augmented Generation (RAG)
* PDF knowledge base
* CRM integration
* Multi-agent AI workflow

---

# 🏗️ System Architecture

> **Architecture diagram will be added after completing Version 1.**

```text
Customer
      │
      ▼
Telegram / Website / Webhook
      │
      ▼
n8n Workflow
      │
 ┌──────────────┬──────────────┐
 ▼              ▼              ▼
Gemini     Knowledge Base   Business Logic
      │
      ▼
AI Response
      │
 ┌────┴───────────────┐
 ▼                    ▼
Telegram      Gmail / Google Sheets
```

---

# 🔄 Workflow

1. Customer submits a question.
2. The request is received through Telegram or a Webhook.
3. n8n starts the automation workflow.
4. Google Gemini analyzes the customer's request.
5. Relevant information is retrieved from the knowledge base.
6. AI generates a response.
7. The response is sent back to the customer.
8. The interaction is logged for future reference.

---

# ⚙️ Technology Stack

| Category            | Technology         |
| ------------------- | ------------------ |
| Workflow Automation | n8n                |
| AI Model            | Google Gemini      |
| Knowledge Base      | JSON               |
| Messaging           | Telegram           |
| Email               | Gmail              |
| Logging             | Google Sheets      |
| APIs                | Webhooks           |
| Version Control     | Git & GitHub       |
| Vector Database     | Pinecone (Planned) |
| Retrieval           | RAG (Planned)      |

---

# 📂 Repository Structure

```text
AI-Customer-Support-Agent/

├── assets/
├── docs/
├── knowledge-base/
│   ├── faq.json
│   └── sample-data.json
├── prompts/
│   └── system-prompt.md
├── screenshots/
├── workflows/
│   └── customer-support-agent.json
├── .env.example
├── .gitignore
├── LICENSE
└── README.md
```

---

# ✅ Prerequisites

Before running this project, ensure you have:

* n8n
* Google Gemini API Key
* Telegram Bot Token
* Gmail Account (App Password)
* Google Sheets Account

---

# 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/dasu07988/AI-Customer-Support-Agent.git
```

Navigate to the project directory:

```bash
cd AI-Customer-Support-Agent
```

Import the workflow into n8n:

```
workflows/customer-support-agent.json
```

Configure all required credentials and activate the workflow.

---

# ⚙️ Configuration

Create a `.env` file based on `.env.example`.

Example:

```env
GEMINI_API_KEY=your_api_key
TELEGRAM_BOT_TOKEN=your_bot_token
GMAIL_USER=your_email
GMAIL_APP_PASSWORD=your_password
```

---

# ▶️ Usage

1. Start n8n.
2. Import the workflow.
3. Configure API credentials.
4. Activate the workflow.
5. Send a message through Telegram or the configured webhook.
6. The AI will generate and return a response automatically.

---

# 💬 Sample Conversation

**Customer**

> Hi, how can I reset my password?

**AI**

> You can reset your password by selecting **Forgot Password** on the login page. A password reset link will be sent to your registered email address.

---

**Customer**

> What are your business hours?

**AI**

> Our support team is available Monday to Friday from 9:00 AM to 6:00 PM.

---

# 📚 Documentation

Project documentation will be available in:

* `docs/`
* `knowledge-base/`
* `prompts/`
* `workflows/`

---

# 🗺️ Development Roadmap

### ✅ Version 1

* Google Gemini
* Telegram
* Gmail
* Google Sheets
* FAQ Knowledge Base
* Webhooks

### 🚧 Version 2

* Memory
* Human Handoff
* Ticket Management
* Escalation Workflow
* Customer History

### 🚀 Version 3

* Pinecone
* Enterprise RAG
* Semantic Search
* PDF Knowledge Base
* CRM Integration
* Multi-Agent AI

---

# 📸 Screenshots

The following screenshots will be added after Version 1 is completed.

* Dashboard
* n8n Workflow
* Telegram Conversation
* Gmail Notification
* Google Sheets Logs

---

# 🎥 Demo

Coming Soon

* Demo Video
* Workflow Walkthrough
* End-to-End Demonstration

---

# 📈 Future Improvements

* WhatsApp Integration
* Slack Integration
* Voice Assistant
* Customer Sentiment Analysis
* Analytics Dashboard
* CRM Integration
* Multi-language Support
* Enterprise Authentication

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Submit a Pull Request.

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

**Dasuni Jayasundara**

BSc (Hons) Information Technology Undergraduate

### Interests

* Artificial Intelligence
* Workflow Automation
* Generative AI
* Retrieval-Augmented Generation (RAG)
* Enterprise AI Solutions
* Cloud Computing

---

<p align="center">

⭐ If you found this project useful, please consider giving it a **Star**.

</p>
