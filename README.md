# ALO Education – Web & CRM Automation Platform

ALO Education’s official web frontend and automation system for managing student leads, enquiries, and counselor workflows.

This repository powers the public website, lead capture forms, and integrates with backend automation tools such as n8n and Supabase CRM.

---

## 🌐 Live Website
👉 https://www.aloeducation.co.uk

---

## 🚀 Key Features

- 🎓 Study Abroad Lead Capture (UK, Australia, etc.)
- 📝 Free Assessment & Apply Forms
- ⚙️ n8n Webhook Automation
- 🗂️ Supabase-based CRM (Lead Storage)
- 📧 Email Notifications (Gmail SMTP)
- ☁️ Deployed on DigitalOcean App Platform
- 🔒 Secure, scalable, production-ready setup

---

## 🏗️ System Architecture

```text
Website (HTML/CSS/JS)
        |
        |  POST (Webhook)
        v
n8n Automation (automation.aloeducation.co.uk)
        |
        ├── Save Lead → Supabase (CRM)
        ├── Save Lead → Google Sheet (Optional)
        └── Send Email → Admissions / Admin
