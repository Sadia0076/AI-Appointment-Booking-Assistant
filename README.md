# AI-Appointment-Booking-Assistant
### End-to-End AI Receptionist built with n8n, OpenAI, Google Calendar, Supabase & Gmail

> 🎥 **Live Project Demo (Loom Video):**  
> **➡️ Add your Loom link here:** `https://loom.com/share/your-video`

---

## 📌 Overview

An AI-powered virtual receptionist that understands natural language, checks real-time calendar availability, books appointments automatically, stores booking records in a database, and sends professional confirmation emails—all without human intervention.

This project demonstrates how Large Language Models can orchestrate multiple business tools to automate a complete appointment booking workflow.

---

## 🚀 Key Features

- 💬 Conversational AI Receptionist
- 📅 Real-time Google Calendar availability checking
- ✅ Automatic appointment booking
- 🗄️ Persistent booking storage in Supabase
- 📧 Automated confirmation emails via Gmail
- 🤖 AI Tool Calling using n8n AI Agent
- 🌍 Timezone-aware appointment scheduling
- 🔄 End-to-end workflow automation
- ⚡ No manual intervention required
- 🧩 Modular workflow architecture

---

# 🏗️ System Architecture

> **Add your architecture diagram here**

```
User
   │
   ▼
Chat Trigger
   │
   ▼
AI Receptionist Agent
   │
   ├─────────────► Google Calendar
   │                 │
   │                 ├── Check Availability
   │                 └── Create Event
   │
   ├─────────────► Supabase
   │                 │
   │                 └── Store Booking
   │
   ├─────────────► Gmail
   │                 │
   │                 └── Send Confirmation Email
   │
   ▼
Final AI Response
```

---

# 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| Workflow Automation | n8n |
| AI Agent | OpenAI |
| Calendar | Google Calendar API |
| Database | Supabase (PostgreSQL) |
| Email | Gmail API |
| Authentication | OAuth2 |
| Database API | PostgREST |
| Backend Logic | AI Tool Calling |
| Scheduling | Google Calendar |

---

# ⚙️ Workflow Overview

## 1️⃣ AI Receptionist

- Understands natural language
- Collects customer details
- Understands date/time preferences
- Handles follow-up questions
- Determines booking intent

---

## 2️⃣ Availability Check

Queries Google Calendar to determine whether the requested appointment conflicts with existing calendar events.

---

## 3️⃣ Appointment Booking

If the requested slot is available:

- Creates a Google Calendar event
- Invites the customer
- Stores the Calendar Event ID

---

## 4️⃣ Database Persistence

Every successful appointment is stored inside Supabase.

Stored information includes:

- Customer Name
- Email Address
- Appointment Start
- Appointment End
- Calendar Event ID
- Booking Status
- Reminder Status
- Timestamp

---

## 5️⃣ Email Confirmation

Automatically sends a professional confirmation email including:

- Customer Name
- Appointment Date
- Appointment Time
- Timezone
- Confirmation Message

---

# 📂 Project Structure

```
AI-Appointment-Booking-Assistant/

│
├── README.md
├── workflows/
│     ├── appointment-booking.json
│     └── workflow.png
│
├── database/
│     └── supabase-schema.sql
│
├── assets/
│     └── screenshots/
│
└── .env.example
```

---

# 📋 Business Workflow

```
Customer
     │
     ▼
Chat Request
     │
     ▼
AI Receptionist
     │
     ▼
Check Calendar Availability
     │
     ▼
Available?
   ├───────────────┐
   │ Yes           │ No
   ▼               ▼
Book Event     Suggest Alternatives
   │
   ▼
Save to Database
   │
   ▼
Send Confirmation Email
   │
   ▼
Return Success Response
```

---

# 💡 AI Capabilities

- Intent Detection
- Tool Selection
- Function Calling
- Context Awareness
- Multi-step Reasoning
- Appointment Scheduling
- Timezone Handling
- Conversational Memory
- Automated Decision Making

---

# 📊 Database Schema

| Column | Description |
|---------|-------------|
| id | Unique Appointment ID |
| customer_name | Customer Name |
| email | Customer Email |
| appointment_start | Start Time |
| appointment_end | End Time |
| calendar_event_id | Google Calendar Event |
| status | Booking Status |
| reminder_24h_sent | Reminder Flag |
| reminder_1h_sent | Reminder Flag |
| created_at | Timestamp |

---

# 🔄 End-to-End Automation Flow

```
Customer
      │
      ▼
AI Agent
      │
      ▼
Check Calendar
      │
      ▼
Book Appointment
      │
      ▼
Save to Supabase
      │
      ▼
Send Gmail Confirmation
      │
      ▼
Customer Receives Confirmation
```

---

# 📈 Skills Demonstrated

- AI Workflow Automation
- Agentic AI Systems
- Tool Calling
- Prompt Engineering
- API Integration
- Workflow Orchestration
- Google Workspace Automation
- REST API Integration
- PostgreSQL
- Supabase
- OAuth2 Authentication
- Business Process Automation
- Event Scheduling Systems
- Conversational AI
- Error Handling
- Modular Workflow Design

---

# 🎯 Real-World Use Cases

- Healthcare Clinics
- Dental Practices
- Law Firms
- Salons & Spas
- Consultants
- Coaching Businesses
- HR Interview Scheduling
- Customer Support
- Small Business Appointment Management

---


# 👩‍💻 About Me

**Sadia Ali**

### Connect with me

- LinkedIn: https://www.linkedin.com/in/sadia-ali-ce/

---

## ⭐ If you found this project interesting, consider giving it a star!

