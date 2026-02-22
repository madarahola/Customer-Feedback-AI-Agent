# Customer-Feedback-AI-Agent
Built an AI Feedback Classification Agent using n8n + Gemini

Sharing a snapshot of the workflow I built (see image 👇).

Here’s what’s happening step-by-step:

🔹 Form Submission Trigger
User submits name, email, and feedback.

🔹 AI Agent (Gemini Model)
The agent reads the feedback and classifies it into:

Complaint

Feature Request

Appreciation

🔹 Merge + Switch Logic
Based on AI output, the workflow branches automatically.

🔹 Database Routing
Feedback is stored in the correct table (complaints / features / compliments).

🔹 Automated Email Confirmation
User instantly receives a professional acknowledgment email.

💡 What This Demonstrates

Intent classification using LLM

Workflow branching with automation

Zero manual sorting

Structured data storage

Real business process automation

This is not just a chatbot —
It’s an AI-powered decision engine inside a workflow system.

Students & professionals:
This is how AI agents are actually implemented in production — combining triggers, reasoning, branching, and actions.
