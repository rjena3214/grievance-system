# 🏢 Internal Grievance Redressal System

> A 3-agent AI pipeline that automates the entire employee grievance process — from intake to formal report generation.

**Live Demo:** [rjena3214.github.io/grievance-system](https://rjena3214.github.io/grievance-system)

---

## What This Does

Most companies handle grievances manually — forms get lost, cases take weeks, employees feel unheard. This system automates the entire first-pass process using three independent AI agents that work sequentially, each with a specific responsibility.

An employee submits a grievance. Three agents process it. A formal report is generated and ready to download in under 60 seconds.

---

## The 3-Agent Pipeline

```
Employee Submits Form
        ↓
┌─────────────────────┐
│   AGENT 1 · INTAKE  │
│  Validates the case │
│  Determines severity│
│  High / Medium / Low│
└──────────┬──────────┘
           ↓
┌─────────────────────┐
│ AGENT 2 · HR ANALYSIS│
│ Recommends actions  │
│ Estimates timeline  │
│ Lists documentation │
└──────────┬──────────┘
           ↓
┌─────────────────────┐
│ AGENT 3 · ESCALATION│
│ Decides if committee│
│ review is needed    │
│ Generates formal    │
│ report with Case ID │
└─────────────────────┘
        ↓
  Downloadable .txt Report
```

### Agent 1 — Intake Agent
- Receives and validates the employee's grievance
- Confirms the category (harassment, unfair treatment, salary dispute, etc.)
- Assigns severity level: **High / Medium / Low**
- Flags any missing information
- Produces a formal intake summary

### Agent 2 — HR Analysis Agent
- Takes Agent 1's output as input
- Assesses organisational risk level
- Lists applicable company policies and labour laws
- Recommends specific HR action steps
- Identifies which personnel should be involved
- Estimates resolution timeline
- Lists interim protective measures for the employee

### Agent 3 — Escalation Agent
- Reviews all previous agent outputs
- Makes the final escalation decision — HR-level or Grievance Committee
- Generates a complete formal report including:
  - Unique Case ID
  - Complainant details
  - Key findings
  - Recommended final action
  - Next steps with responsible parties
  - Confidentiality notice

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| AI Engine | Anthropic Claude API (claude-sonnet-4) |
| Architecture | 3-agent sequential pipeline |
| Deployment | GitHub Pages (static, no server needed) |
| Storage | None — fully client-side, zero data stored |

---

## Features

- **Zero backend** — single HTML file, runs entirely in the browser
- **Live agent progress** — watch each agent activate and complete in real time
- **Pipeline indicator** — visual status bar showing which agent is currently running
- **Downloadable report** — final formal report saved as `.txt` with unique Case ID
- **Mobile responsive** — works on phone and desktop
- **Privacy first** — API key stays in the browser, no data is stored anywhere

---

## Getting Started

### Prerequisites
- An Anthropic API key — get one at [console.anthropic.com](https://console.anthropic.com)

### Run Locally
```bash
# Clone the repository
git clone https://github.com/rjena3214/grievance-system.git

# Open the file directly in your browser
open index.html
```

No npm install. No build step. No dependencies. Just open and run.

### Deploy to GitHub Pages
```
1. Push index.html to your GitHub repository
2. Go to Settings → Pages
3. Source: Deploy from branch → main → / (root)
4. Save — live in 2 minutes
```

---

## How to Use

1. Open the live site or `index.html` locally
2. Enter your Anthropic API key in the field provided
3. Fill in the grievance form:
   - Employee name and ID
   - Department
   - Grievance category
   - Detailed description
   - Whether the issue was reported to a supervisor
   - Date of incident
4. Click **Submit Grievance → Activate 3-Agent Pipeline**
5. Watch all 3 agents process the case sequentially
6. Download the formal report when complete

---

## Use Cases

| Who Uses This | How |
|--------------|-----|
| **HR Departments** | First-pass processing of all incoming grievances |
| **Small Companies** | Full grievance handling without a dedicated HR team |
| **Startups** | Professional grievance process from Day 1 |
| **Developers** | Reference implementation of multi-agent AI pipelines |

---

## Business Value

- Reduces grievance processing time from **weeks to minutes**
- Ensures **consistent, unbiased** initial assessment every time
- Creates a **formal paper trail** automatically
- Protects the company by flagging high-risk cases immediately
- Removes human error from the intake and categorisation stage

---

## Project Structure

```
grievance-system/
│
└── index.html          # Complete application — single file
```

---

## Part of the 75-Day AI Vibe Coder Journey

This project was built as part of a structured 75-day plan to go from beginner to AI developer.

- **Builder:** Ranjan Kumar Jena
- **GitHub:** [github.com/rjena3214](https://github.com/rjena3214)
- **Day:** 8 of 75
- **Stack used:** Claude API, multi-agent architecture, vanilla HTML/CSS/JS

---

## License

MIT — free to use, modify, and deploy.

---

## Author

**Ranjan Kumar Jena**
Anthropic Certified · AI Builder · Prompt Engineer

[![GitHub](https://img.shields.io/badge/GitHub-rjena3214-181717?style=flat&logo=github)](https://github.com/rjena3214)
