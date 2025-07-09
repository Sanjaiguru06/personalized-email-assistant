# 📬 Personalized AI Email Assistant

> An AI-powered assistant that reads, summarizes, and notifies you of important company emails in real-time — powered by LLMs, LangChain, and n8n.

![GitHub Repo Stars](https://img.shields.io/github/stars/Sanjaiguru06/personalized-email-assistant?style=flat-square)
![GitHub Forks](https://img.shields.io/github/forks/Sanjaiguru06/personalized-email-assistant?style=flat-square)
![MIT License](https://img.shields.io/github/license/Sanjaiguru06/personalized-email-assistant?style=flat-square)

---

## 🧠 What it Does

- 📥 Filters emails from your company (e.g. `@company.com`)
- ✨ Summarizes email content using LangChain + GPT
- 🔔 Sends real-time pop-up or Telegram notifications
- 📅 Suggests calendar slots for meetings (optional)
- 🧪 Learns from user edits to improve responses

---

## 🏗️ Architecture

```plaintext
Gmail/Outlook
   │
   ▼
n8n Email Trigger
   │ (Filter @company.com)
   ▼
Webhook → Flask API (LangChain Summary + Intent)
   │
   ├── Desktop Notification (Python)
   └── Telegram Bot Notification
