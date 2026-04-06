# 🧠 Physio One WhatsApp Automation (n8n)

This project is an advanced **n8n workflow** that automates WhatsApp conversations for a physiotherapy clinic.

## 🚀 Features

* WhatsApp webhook integration (via YCloud)
* AI receptionist (Deepti) using LLM
* Multi-input support:

  * Text
  * Audio (transcription)
  * Images (analysis)
* Appointment booking system
* Google Sheets integration
* Telegram notifications for clinic owner
* Supabase chat history storage
* Context-aware conversation memory (Postgres)

---

## 🧩 Workflow Overview

1. User sends WhatsApp message
2. Webhook receives message
3. Message type routed (text/audio/image)
4. AI processes conversation
5. Appointment handled:

   * Check availability
   * Save to Google Sheets
   * Notify via Telegram
6. Reply sent back to WhatsApp

---

## ⚙️ Setup Instructions

### 1. Import Workflow

* Open n8n
* Go to Workflows
* Click "Import from File"
* Upload `workflows/physioone-workflow.json`

---

### 2. Configure Credentials

You need to set up:

* YCloud API (WhatsApp)
* Google Sheets OAuth
* Telegram Bot
* Supabase
* Postgres DB
* Gemini API (or your LLM)

---

### 3. Environment Variables

Use `.env.example` as reference.

---

### 4. Activate Webhook

* Enable the workflow
* Copy webhook URL
* Add it in YCloud dashboard

---

## 📍 Use Case

Perfect for:

* Clinics
* Appointment booking bots
* WhatsApp automation
* AI customer support

---

## ⚠️ Notes

* Do NOT commit real API keys
* Always use environment variables
* Customize prompts based on your business

---

## 👨‍💻 Author

Built using n8n + AI automation.
