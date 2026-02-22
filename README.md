#Customer-Feedback-AI-Agent

An automated AI-powered feedback classification and routing system built using n8n workflows integrated with Google Gemini (LLM).

This project demonstrates how Large Language Models can be embedded inside workflow automation tools to create a decision-making AI agent for real business processes.

##🖼 Workflow Overview

Below is a high-level overview of the workflow architecture:
<img width="1405" height="632" alt="image" src="https://github.com/user-attachments/assets/e81fb633-8a08-42fa-b1d4-c89e346eeacd" />


⚙️ System Architecture & Execution Flow
1️⃣ Trigger Layer – Form Submission

User submits:

Name

Email

Feedback Message

n8n Webhook/Form Trigger initiates the workflow execution.

2️⃣ AI Processing Layer – Gemini LLM

Feedback text is passed to Google Gemini.

The model performs intent classification.

Output categories:

Complaint

Feature Request

Appreciation

This transforms unstructured text into structured, machine-readable output.

3️⃣ Decision Layer – Merge & Switch Logic

AI output is captured.

A Switch node dynamically routes execution based on classification.

Ensures deterministic branching behavior inside the workflow.

4️⃣ Data Persistence Layer – Database Routing

Feedback is stored in dedicated tables:

complaints

feature_requests

compliments

Enables structured storage and analytics-ready datasets.

5️⃣ Response Automation Layer – Email Notification

Automatically sends a formatted confirmation email.

Ensures immediate acknowledgment.

Eliminates manual response handling.

🧠 Technical Capabilities Demonstrated

LLM-based Intent Classification

Event-Driven Workflow Automation

Dynamic Branching Logic

Structured Data Routing

Automated Transactional Emailing

Zero Manual Intervention Processing

🚀 Why This Matters

This is not a simple chatbot implementation.

It is a workflow-embedded AI decision engine that:

Converts unstructured feedback into structured business data

Automates routing and storage

Executes conditional logic

Triggers downstream operational tasks

🎯 Real-World Application

This architecture can be extended for:

Customer support automation

Lead qualification systems

Ticket triaging

Sentiment-based escalation workflows

CRM auto-tagging

📌 Production Insight

This project reflects how AI agents are implemented in real-world systems:

Trigger → Reasoning (LLM) → Branching → Action → Storage → Notification

It showcases the integration of:

Workflow orchestration

LLM reasoning

Business rule enforcement

Automated operations
