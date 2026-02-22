# Customer-Feedback-AI-Agent

An AI-powered feedback classification and automation system built using **n8n workflows** and **Google Gemini (LLM)**.

This project demonstrates how Large Language Models (LLMs) can be embedded inside workflow automation tools to build a production-ready **AI decision-making agent** for real-world business use cases.

---

## 📌 Workflow Overview

Below is a high-level overview of the workflow architecture used in this project:

<img width="1405" height="632" alt="image" src="https://github.com/user-attachments/assets/1a972d95-249a-4564-8794-c9b629b017a5" />

---

## ⚙️ Architecture & Execution Flow

### 1. Trigger Layer – Form Submission
- The workflow starts when a user submits a feedback form.
- Input fields include:
  - Name  
  - Email  
  - Feedback message
- The form submission acts as the event trigger in n8n.

---

### 2. AI Processing Layer – Gemini LLM
- User feedback is passed to the **Google Gemini Chat Model**.
- The AI agent performs **intent classification** on unstructured text.
- Feedback is categorized into one of the following:
  - Complaint  
  - Feature Request  
  - Appreciation  

This step converts free-text input into structured output.

---

### 3. Decision Layer – Merge & Switch Logic
- AI classification output is merged with form metadata.
- A **Switch node** evaluates the intent label.
- Workflow execution branches dynamically based on the classification result.

---

### 4. Data Persistence Layer – Database Routing
- Feedback is stored in dedicated database tables:
  - `complaints`
  - `feature_requests`
  - `compliments`
- Enables clean data separation and downstream analytics.

---

### 5. Response Automation – Email Notification
- An automated confirmation email is sent to the user.
- Confirms successful submission of feedback.
- Ensures immediate acknowledgment without manual intervention.

---

## 🧠 Key Technical Capabilities

- LLM-based intent classification
- Event-driven workflow orchestration
- Dynamic branching logic
- Structured data storage
- Automated transactional email handling
- Fully automated, zero manual sorting

---

## 🚀 Why This Project Matters

This is not a traditional chatbot.

It is a **workflow-embedded AI agent** that:
- Interprets user intent using an LLM
- Makes routing decisions
- Executes conditional business logic
- Persists structured data
- Triggers operational actions automatically

---

## 🎯 Potential Use Cases

- Customer support ticket classification
- Feature request tracking systems
- Sentiment-based feedback analysis
- CRM tagging and routing
- Internal helpdesk automation

---

## 🏗️ Production Design Insight

This project follows a real-world AI agent architecture:

