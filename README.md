# 🤖 AI Customer Support Agent — n8n & Google Gemini

<p align="center">
  <img src="assets/ChatGPT Image Jul 24, 2026, 08_31_10 PM.png" alt="AI Customer Support Agent Banner" width="100%">
</p>

<p align="center">

![Status](https://img.shields.io/badge/Status-MVP%20Completed-success)
![Version](https://img.shields.io/badge/Version-v1.0-blue)
![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-EA4B28)
![Google Gemini](https://img.shields.io/badge/Google-Gemini%202.5%20Flash-4285F4)
![Webhook API](https://img.shields.io/badge/API-REST%20Webhook-success)
![Google Sheets](https://img.shields.io/badge/Logging-Google%20Sheets-34A853)
![License](https://img.shields.io/badge/License-MIT-yellow)

</p>

<p align="center">
<b>An AI-powered customer support automation system built with n8n, Google Gemini 2.5 Flash, and Google Sheets — turning repetitive support tickets into instant, AI-generated responses.</b>
</p>

---

## 📖 Contents
[Overview](#-overview) • [Problem & Solution](#-the-problem) • [Architecture](#️-system-architecture) • [Tech Stack](#️-technology-stack) • [Features](#-features) • [API Docs](#-api-documentation) • [Setup](#-installation) • [Roadmap](#️-roadmap) • [Author](#-author)

---

## 🚀 Overview

The AI Customer Support Agent is an end-to-end workflow automation system built with **n8n** and **Google Gemini 2.5 Flash**.

The workflow receives customer requests through a REST Webhook, validates the payload, intelligently routes frequently asked questions, injects business knowledge, generates AI-powered responses, logs every interaction into Google Sheets, and returns the response in real time.

The project demonstrates practical skills in:

- AI Workflow Automation
- Prompt Engineering
- REST API Development
- Business Process Automation
- Google Workspace Integration
- Low-Code AI Engineering

---

## 🎯 The Problem

Support teams burn significant time answering the same FAQs — refund policy, shipping, business hours — leading to:

- Slow response times & higher operational cost
- Inconsistent answers across agents
- No support coverage outside business hours
- Support staff stuck on repetitive work instead of complex issues

## 💡 The Solution

Instead of a human reading and replying to every message, the workflow:

1. Accepts requests via REST Webhook
2. Validates the payload
3. Routes the query to the right FAQ category
4. Injects structured business knowledge (prevents hallucination)
5. Generates a response with Google Gemini
6. Logs every conversation to Google Sheets
7. Returns the response instantly through the API

Architecture is modular by design — built to extend into RAG, vector search, CRM integration, and multi-agent systems (see [Roadmap](#️-roadmap)).

---



## 🏗️ System Architecture

<p align="center">

<img src="docs/architecture/Architecture Diagram AI ChatBot (1).png" width="120">

</p>

| Step | Description |
|------|-------------|
| 1 | Customer submits request via Webhook API |
| 2 | Payload validated |
| 3 | FAQ Router categorizes the request |
| 4 | Business Knowledge Base injects company context |
| 5 | Gemini generates AI response |
| 6 | Log formatted for storage |
| 7 | Google Sheets stores the conversation |
| 8 | API returns the generated response |

---

## ⚙️ Technology Stack

| Category | Technology |
|---|---|
| Workflow Automation | n8n |
| AI Model | Google Gemini 2.5 Flash |
| Approach | Low-Code |
| API | REST Webhook |
| Knowledge Base | Business Context (JSON) |
| Logging | Google Sheets |
| Testing | Postman |
| Version Control | Git & GitHub |
| Planned | Pinecone Vector DB, RAG |

---

## ✨ Features


- ✅ AI-powered Customer Support
- ✅ Google Gemini 2.5 Flash Integration
- ✅ REST Webhook API
- ✅ FAQ Routing
- ✅ Business Knowledge Injection
- ✅ Hallucination Prevention
- ✅ Input Validation
- ✅ Google Sheets Conversation Logging
- ✅ Modular n8n Workflow
- ✅ Postman Tested

---

## 📡 API Documentation

**Endpoint**
```http
POST /webhook/customer-support
```

**Request**
```json
{ "message": "What is your refund policy?" }
```

**Successful Response**
```json
{
    "Timestamp": "2026-07-24T10:21:03.550-04:00",
    "Customer Message": "What is your refund policy?",
    "Category": "General",
    "AI Response": "Our refund policy allows you to request a refund within 30 days of purchase, provided the product is unused and in its original condition."
}
```

**Invalid Request → Validation Response**
```json
{ "success": false, "error": "Message is required." }

POST /webhook/customer-support

Status: 200 OK

Content-Type: application/json

```

---

## 📊 Project Highlights

| Metric | Value |
|---------|-------|
| Workflow Nodes | 10+ |
| AI Model | Google Gemini 2.5 Flash |
| Workflow Engine | n8n |
| API Type | REST Webhook |
| Logging | Google Sheets |
| Status | MVP Completed |
---


## 📂 Repository Structure

```text
AI-Customer-Support-Agent/
├── assets/
├── docs/architecture.png
├── workflow/AI-Customer-Support-Agent.json
├── screenshots/
├── examples/{request.json, response.json}
├── LICENSE
└── README.md
```

---

## ✅ Prerequisites

n8n · Google Gemini API key · Google Account & Sheets · Postman (for testing)

## 🚀 Installation

```bash
git clone https://github.com/dasu07988/AI-Customer-Support-Agent.git
cd AI-Customer-Support-Agent
```

1. Import `workflow/AI-Customer-Support-Agent.json` into n8n
2. Configure credentials: **Google Gemini** (AI response generation) & **Google Sheets** (logging)
3. Activate the workflow

## ▶️ Usage

Start the workflow → activate the webhook → send a POST request via Postman → get the AI response → verify the log entry in Google Sheets.

## 🧪 Testing

Validated end-to-end using Postman, Google Sheets, Google Gemini, and a local n8n environment.

---
## 🗺️ Roadmap

| Version | Features |
|---------|----------|
| ✅ **v1** | Gemini Integration, Webhook API, FAQ Routing, Business Knowledge, Google Sheets Logging |
| 🚧 **v2** | Conversation Memory, Human Handoff, CRM Integration, Email Notifications |
| 🚀 **v3** | Pinecone, RAG, Semantic Search, Multi-Agent AI, Analytics Dashboard |

---

## ⭐ Why This Project

Goes beyond a simple chatbot demo — a structured, extensible automation workflow realistically adaptable for small/medium businesses, showcasing AI workflow automation, low-code development, prompt engineering, REST API integration, and enterprise-style workflow design.

---

## 🎯 Business Impact

This solution helps organizations:

- Reduce repetitive customer support tasks
- Improve response consistency
- Automate FAQ handling
- Increase customer satisfaction
- Reduce operational costs
- Scale customer support with AI

---

## 🤝 Contributing

Fork → create a feature branch → commit → push → open a Pull Request.

## 📄 License

MIT License.

---

## 👩‍💻 Author

**Dasuni Jayasundara**



### Areas of Interest

- Artificial Intelligence
- AI Workflow Automation
- Prompt Engineering
- Enterprise AI
- Low-Code AI Solutions

- GitHub: [github.com/dasu07988](https://github.com/dasu07988)
- LinkedIn: *(add link)*

---

---

<---

<p align="center">

Built with ❤️ using **n8n**, **Google Gemini 2.5 Flash**, and **Google Workspace**

⭐ If you found this project useful, please consider giving it a **Star**.

</p>