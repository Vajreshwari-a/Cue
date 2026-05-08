# Cue 🖊️
### Your study buddy, straight from WhatsApp.

Built on OpenClaw. Shows up at your study time, every day, with everything you need — study material, key concepts, and practice questions generated fresh from your syllabus. Cue knows your exam dates, reads your vibe, adjusts when life gets in the way, and never guilt trips you for a bad day. Powered by Gemini.

---

## 🎯 The Problem

Most students don't fail because they're lazy. They fail because life gets in the way — and by the time they realize they're behind, it's the night before the exam. Cue is built for exactly that student. The one who means to study but keeps pushing it. The one who pulls all-nighters not by choice, but because nothing warned them early enough.
- Nobody reminds them to study until it's too late
- Study material is scattered across PDFs, drives, and notes
- Generic apps don't understand *their* schedule, *their* syllabus, *their* bad days
- Every tool requires opening an app, logging in, navigating a dashboard

**Cue fixes all of this — and lives where students already are. WhatsApp.**

---

## ✨ What Cue Does

- **Shows up first** — texts you at your preferred study time, every day, without you asking
- **Generates study material** from your syllabus — key concepts, simple explanations, practice questions
- **Knows your exam dates** — builds a study plan around them automatically
- **Reads your vibe** — detects if you're anxious, burned out, or procrastinating and adapts its tone
- **Never guilt trips** — if you miss a day, Cue just replans. No lectures.
- **Emergency exam mode** — say "exam tomorrow" and Cue switches to survival mode instantly
- **Ghosting protocol** — if you go quiet for 48 hours, Cue checks in warmly with zero pressure

---

## 🧠 Personality Modes

Cue detects how you're feeling from how you text — and adapts:

| Mode | Vibe | Cue's Approach |
|------|------|----------------|
| 😰 Anxious | Stressed, overwhelmed | Gentle, slow, reassuring |
| 😤 Focused | Locked in | Crisp, efficient, no fluff |
| 😴 Burned out | Exhausted | Validate first, study second |
| 🔥 Overachiever | High energy | Match the energy, stretch goals |
| 😅 Procrastinator | Avoiding everything | Sneaky nudges, make it feel tiny |

---

## 🏗️ How It's Built

| Layer | Tech |
|-------|------|
| Agent framework | [OpenClaw](https://openclaw.ai) |
| LLM | Google Gemini 2.5 Flash Lite |
| Channel | WhatsApp (via OpenClaw WhatsApp plugin) |
| Identity | SOUL.md — Cue's personality and behavioral rules |
| Proactive messaging | HEARTBEAT.md — scheduled check-ins and daily delivery |
| Onboarding | onboarding.md — conversational student setup flow |
| Memory | OpenClaw workspace memory system |

---

## 📁 Repository Structure

```
├── SOUL.md          # Cue's identity, personality, tone, and behavioral rules
├── HEARTBEAT.md     # Proactive messaging schedule and check-in logic
├── onboarding.md    # Conversational onboarding flow for new students
├── AGENTS.md        # Workspace rules and session startup instructions
├── USER.md          # Student profile (populated during onboarding)
├── MEMORY.md        # Cue's long-term memory (auto-updated)
└── README.md        # You're here!
```

---

## 🚀 Setup Instructions

### Prerequisites
- Node.js v22+
- A Google Gemini API key (free at [aistudio.google.com](https://aistudio.google.com))
- OpenClaw installed
- A WhatsApp account

### Installation

**1. Install OpenClaw**
```bash
sudo npm install -g openclaw
```

**2. Install git (if not installed)**
```bash
sudo apt install -y git
```

**3. Configure OpenClaw**
```bash
openclaw configure
```
- Select **Model** → choose `google/gemini-2.5-flash`
- Enter your Gemini API key
- Select **Channels** → WhatsApp → scan QR code with your phone

**4. Clone Cue's workspace files**
```bash
cd ~/.openclaw/workspace
git clone https://github.com/YOUR_USERNAME/cue .
```

**5. Start the gateway**
```bash
openclaw gateway install  # auto-start on boot
openclaw gateway          # start now
```

**6. Text yourself on WhatsApp**

Say "hi" — Cue will introduce herself and start onboarding you! 🎉

---

## 💬 Usage

Once onboarded, Cue handles everything:

| You say | Cue does |
|---------|----------|
| "hi" | Introduces herself, starts onboarding |
| "exam tomorrow" | Switches to emergency survival mode |
| "i'm sick today" | Replans your schedule, no guilt |
| "i can't focus" | Validates, suggests a break, comes back |
| *(nothing for 48h)* | Checks in warmly with zero pressure |
| *(your study time)* | Sends today's study material automatically |

---

## 🤖 AI Disclosure

This project uses AI in the following ways:

- **Google Gemini 2.5 Flash Lite** — powers all of Cue's conversations, study material generation, personality detection, and proactive messaging
- **OpenClaw** — the agent framework that connects Gemini to WhatsApp, manages memory, and runs the heartbeat/scheduling system
- **Claude (Anthropic)** — used during development for code generation, SOUL.md drafting, and architectural decisions
- **Antigravity** — used as an AI-powered IDE for writing and editing workspace files during development

All AI-generated content is clearly a result of prompting and configuration — no fine-tuning was used.

---

## 🔮 What's Coming

- 📄 Syllabus PDF reading and automatic topic extraction
- 🎥 YouTube video recommendations per topic
- 📊 Weekly progress PDF reports
- 🧪 WhatsApp quiz mode — back and forth practice questions
- 🌐 Reddit study tip integration per topic
- 👥 Multi-student support

---

## 👤 Team

Built for the **PRISM OpenClaw "Clash of the Claws" Hackathon** — May 2026

---

*Cue doesn't just remind you to study. She shows up. Every day. Like a friend who actually has their life together.* 🖊️
