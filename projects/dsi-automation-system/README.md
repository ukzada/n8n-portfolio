# 🧠 DSI Automation System

**AI-powered business automation system** built with **n8n**, integrating multiple workflows such as lead collection, credit report analysis, referral tracking, and AI-based communication.  
This project replaces traditional tools like *DisputeFox, Mailchimp, Buffer, Calendly,* and *Zapier* using one unified AI-driven automation stack.

---

## 🚀 Summary

The **DSI Automation System** is designed to automate every stage of a digital business — from lead intake to payment collection — using **n8n** and **AI Orchestration**.

It centralizes your CRM, email campaigns, content creation, referrals, follow-ups, and document generation in one visual workflow.

---

## 🧩 Workflow Architecture

### 🔹 1. Inputs
Handles all incoming requests:
- **Chat Trigger:** Activated when a user sends a message via Telegram or another platform.
- **Webhook Trigger:** Captures events or lead data from web forms or other systems.

### 🔹 2. Manager (AI Brain)
- **AI Agent (LangChain + OpenAI):** Decides what the user needs (report, follow-up, payment, etc.).
- **Memory + Reasoning:** Keeps context between messages and dynamically routes tasks.
- **Decision Routing:** Chooses which automation block to execute (email, PDF, referral, etc.).

### 🔹 3. OpenAI Setup
- **OpenAI Chat Model:** GPT-based reasoning.
- **Simple Memory:** Stores short-term context.
- **Think Node:** Logical processing and intent classification.
- **Google Sheets Node:** Fetches and stores lead data (mini CRM).

### 🔹 4. Automation Modules
| Module | Description |
|--------|--------------|
| **Email Setup** | Sends onboarding or follow-up emails automatically. |
| **PDF Generation** | Creates custom reports or documents (via PDFMonkey or PDF.co). |
| **Lead Management** | Adds/updates lead info in Google Sheets or Zoho CRM. |
| **Content Creation** | AI-generated social posts or email templates. |
| **Phone Bot** | Manages automated calls/SMS via Twilio or Telegram. |
| **Referral System** | Tracks referral codes, applies discounts, logs affiliate data. |
| **Follow-Up System** | Sends reminders and nurturing messages automatically. |

### 🔹 5. Outputs
- **Respond to Chat:** Sends AI replies back to users.
- **Respond to Webhook:** Returns data or success status to external systems.

---

## 🔄 Example Flow

1. User sends: “Can I get my credit report?”
2. Input node activates → data sent to AI Agent.
3. AI Agent fetches user info → triggers **PDF Generation**.
4. PDF is created and emailed.
5. Chatbot replies: “Your credit report is ready! Would you like a free consultation?”
6. If yes → triggers **Phone Bot** or **Follow-Up System**.

---

## 💼 Business Impact

✅ Replaces **5+ SaaS tools**  
✅ End-to-end automation from lead to payment  
✅ Saves hours of manual work weekly  
✅ Scalable for multiple client accounts  
✅ Fully visual and editable via **n8n Web UI**

---

## 🛠️ Tech Stack

- **n8n** – Workflow automation engine  
- **OpenAI API (GPT)** – AI logic and conversation management  
- **LangChain** – AI orchestration layer  
- **Google Sheets API** – CRM data sync  
- **PDFMonkey / PDF.co** – Dynamic PDF generation  
- **NowPayments.io / Stripe** – Payment gateway integration  
- **Twilio / Telegram Bot API** – Messaging & phone automation  

---

## 📁 Folder Structure
-dsi-automation-system/
-├── README.md # Project documentation
-├── workflow.json # Exported n8n workflow
-├── diagram.png # Workflow screenshot (uploaded)
-├── modules/
-│ ├── email_setup.json
-│ ├── pdf_generation.json
-│ ├── lead_management.json
-│ ├── referral_system.json
-│ ├── follow_up.json
-└── docs/
-├── ai_manager_explained.md
-├── setup_instructions.md
-└── api_keys_config.md

