# 🧪 Take-Home Project – AI Lead Builder

Welcome! This assignment simulates a real product feature at GroundAI. You’ll build a lightweight, AI-powered outreach workflow tool using modern web tech.

---

## 🎯 Goal

Build a **simple web-based outreach generator** where a user can:

1. Enter a lead (name, role, company)
2. Generate a personalized LinkedIn DM using OpenAI
3. Save the message into a Supabase database
4. View and manage leads in a table view

---

## ⏱ Timeline

This assignment is expected to take **~3 days**. Please manage your time wisely.

---

## 📦 Submission Requirements

You must submit:

1. A **public GitHub repository** with full code, docs, and setup instructions
2. A **5–10 minute Loom video** (or any screen recording tool) explaining:
   - Your thought process
   - Feature overview
   - Architecture decisions
   - What you would improve with more time

---

## 📐 Project Scope: What to Build

### 🔨 Core Features

- A lead input form:
  - Name
  - Role (e.g., “Marketing Lead”)
  - Company
  - (optional) LinkedIn URL
- A “Generate Message” button that:
  - Calls the OpenAI API
  - Creates a personalized message for the lead
- A Supabase database to store:
  - Lead info
  - Generated message
  - Status (e.g., Draft / Approved / Sent)
- A UI to view and manage the leads and messages

### 💡 Bonus Features (Optional)

- Drag-and-drop columns (like Trello) for status tracking
- Bulk message generation for multiple leads
- Export leads/messages to CSV
- Hosted on Vercel

---

## 🧱 Tech Stack

You **must** use:

- `Next.js` (App Router)
- `Supabase` (Auth + DB)
- `Tailwind CSS` or `shadcn/ui`
- `OpenAI API` (GPT-3.5 or GPT-4)

---

## 🧠 Suggested Development Phases

You’re expected to simulate a real engineering workflow. Use the following steps and include them in your documentation:

### 1. Ideation
- What is the user goal?
- What pain point are you solving?

### 2. Planning
- Sketch or describe the user flow
- List features you will build (MVP vs Bonus)
- Define your tech stack

### 3. Approval (Document This)
- Describe the final scope you chose
- List any tradeoffs, constraints, or assumptions

### 4. Architecture Review
- Draw a simple diagram or table describing your architecture:
  - Where is the data stored?
  - What are the key components?
  - How are API requests handled?

### 5. Delivery
- Link to GitHub repo
- Loom or video explanation
- Live Vercel deployment (optional)

---

## 🔑 Example Prompt for OpenAI

You may use this sample prompt when calling the API:

> “Write a short, friendly LinkedIn outreach message to {{name}}, who is a {{role}} at {{company}}. Make it casual and under 500 characters.”

---

## 🧪 Example `.env.example`

```env
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
OPENAI_API_KEY=your-openai-key
