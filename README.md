# 📬 Personalized AI Email Assistant

> An AI-powered assistant that reads, summarizes, and notifies you of important company emails in real-time — powered by LLMs, LangChain, and n8n.

![GitHub Repo Stars](https://img.shields.io/github/stars/Sanjaiguru06/personalized-email-assistant?style=flat-square)
![GitHub Forks](https://img.shields.io/github/forks/Sanjaiguru06/personalized-email-assistant?style=flat-square)
![MIT License](https://img.shields.io/github/license/Sanjaiguru06/personalized-email-assistant?style=flat-square)

---

## 🚀 Features

✅ Detects and filters emails from your company  
✅ Sends instant Telegram alerts with email subject + link  
✅ Built using **n8n** — no code, fully visual  
✅ Works without needing Flask or any local script running  
✅ Easily customizable for other email senders or platforms

---

## 🛠️ Tech Stack

| Tool      | Purpose                          |
|-----------|----------------------------------|
| **n8n**   | Workflow automation engine       |
| **Gmail Node** | Polling inbox for new mails    |
| **Telegram Node** | Send alert messages         |
| **IF Node** | Filter only company emails     |


## 🧠 What it Does

- 📥 Filters emails from your company (e.g. `@company.com`)
- ✨ Summarizes email content using LangChain + GPT
- 🔔 Sends real-time pop-up or Telegram notifications
- 📅 Suggests calendar slots for meetings (optional)
- 🧪 Learns from user edits to improve responses

---

## 🏗️ Architecture

Gmail (via n8n trigger)
   │
   ▼
Filter Node (@company.com check)
   │
   ▼
Telegram Node (Send notification)
