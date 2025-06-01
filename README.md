# n8n + Retell AI – Automated Appointment Reminder Calls

A no-code, end-to-end solution that scans your calendar daily, extracts appointment details via AI, and automatically calls customers to confirm or reschedule their appointments—saving businesses hours of manual outreach.

## 🚀 Project Overview

- **Name:** n8n + Retell AI – Automated Appointment Reminder Calls
- **Purpose:** Automatically remind customers of upcoming appointments via AI-driven voice calls.
- **Key Benefits:**
  - Eliminates manual dialing and reduces no-shows
  - Scales across any business that relies on scheduled appointments
  - Built entirely in n8n (self-hosted or cloud) with Retell AI for lifelike voice interactions
  - Leverages AI (OpenAI GPT-4/4o Mini or Anthropic) to parse calendar details into structured JSON

## 💡 Use Case Overview

- **Daily Scheduling**  
  Runs at a scheduled time (e.g., 9 AM every morning) to fetch calendar events occurring within the next 12 hours.
  
- **Calendar Integration**  
  Retrieves event data—including customer name, phone number, appointment reason, and start/end times—from Google Calendar (or any supported calendar).

- **AI-Driven Extraction**  
  Uses n8n’s AI Agent node to parse free-form meeting descriptions into a structured JSON schema:
  ```json
  {
    "name": "Jane Doe",
    "phone": "",
    "reason": "",
    "startTime": "",
    "endTime": ""
  }
