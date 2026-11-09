# 📅 organize-your-calendar

> A Claude Skill that helps lazy, easily-discouraged, or beginner users build a **minimalist, low-friction, sustainable** personal schedule system — instead of another productivity app they'll abandon in 3 days.

[![Skill](https://img.shields.io/badge/Claude-Skill-5A32FB)](#) [![Version](https://img.shields.io/badge/version-1.0-blue)](#) [![Status](https://img.shields.io/badge/status-stable-brightgreen)](#)

---

## ✨ Overview

Most time-management systems fail not because the user lacks discipline, but because the system assumes an ideal, zero-friction life. **organize-your-calendar** is built around the opposite assumption: the user *will* get tired, *will* skip a day, and *will* want to quit — and the system should survive that anyway.

It packages this philosophy into a **Three-Pillar Model** plus a **6-week transition roadmap**, so Claude never dumps the whole system on a beginner at once.

| Pillar | Focus | Core idea |
|---|---|---|
| 1️⃣ Mindset | Dual-Tolerance & Active Cutting | 2x time buffer, "pick your loss," 20-minute start |
| 2️⃣ Recording | Low-Friction Analog Anchor Notebook | 1 paper notebook, ≤2 habits tracked, 1 diary line/day, "Number 1" rule |
| 3️⃣ Time | Four-Quarter Macro Calendar Frame | ≤4 digital calendar blocks/day, "eat the frog first," 3 survival tasks/day |

---

## 🎯 When this skill triggers

Claude activates this skill when the user — in any phrasing, not just these exact keywords — talks about:

- Organizing a calendar / schedule / timetable / time blocking
- Time management, habit tracking, bullet journaling
- Feeling overwhelmed, procrastinating, lacking discipline
- Wanting to "restart an organized life" but fearing they'll give up again
- Self-describing as "lazy" and asking for help reorganizing their life

No need to say "Three Pillars" or "Four Quarters" — natural language like *"help me, I keep failing at every schedule I make"* is enough.

---

## 🧩 How it works

### Pillar 1 — Mindset
- **2x buffer rule** — double every time estimate.
- **Active cutting** — before adding any task: *"Is this truly necessary?"* Keep only 1–2 mandatory items.
- **20-minute start** — permission to stop after 20 minutes; done > perfect.

### Pillar 2 — Recording
- One notebook, one pen, fixed desk spot, physically separate from the phone.
- One monthly spread: date | habit | one highlight line.
- Max **2 habits** tracked over 30 days; week 1 is observation-only.
- **"Number 1" rule** — circle exactly one must-do task each morning; everything else is a bonus.

### Pillar 3 — Time
- Digital calendar, but **macro blocks only** — max 4 events/day.
- **Four quarters**: Morning (hardest/creative task) → Midday (rest) → Afternoon (admin/light study) → Evening (recovery).
- **3 survival tasks/day**: 1 work, 1 health, 1 relationship — no more.
- Losing one quarter ≠ losing the whole day.

---

## 🗓️ 6-Week Transition Roadmap

| Phase | Goal | Key actions |
|---|---|---|
| **Weeks 1–2** | Set up the analog anchor | Buy notebook + pen → minimalist monthly page → 1 easy habit → 1 diary line/evening → 20-minute rule |
| **Weeks 3–4** | Shape the macro rhythm | Open digital calendar → ≤4 blocks/day → soft/eye-friendly colors → apply "Number 1" rule daily |
| **Weeks 5–6** | Add tolerance & scale selectively | 2x buffer on complex blocks → "four quarters, lose 1 keep 3" reflex → +1 quantitative metric (weight/pages/sleep hours) |

Claude is instructed to **always ask which phase the user is in** before prescribing anything — never force Week 5–6 content onto a Week 1 beginner.

---

## 🤖 Claude's behavioral rules

- Asks the user's current phase before suggesting a plan.
- Hard caps when generating any schedule: **≤4 macro blocks/day, ≤2 tracked habits**, every complex task estimate doubled, hardest task always in the morning block.
- Uses the word **"action plan"** instead of "task" — a deliberate semantic nudge toward agency.
- Detects a **"domino collapse" risk** (zero-gap schedules) and proactively suggests a buffer.
- Redirects users who demand a perfect 15-minute-increment plan back to the Week 1–2 basics ("done is better than perfect").
- Only after ≥6 consistent weeks does it offer to escalate to more advanced systems (e.g. a 3-tier "Trident" model) via `references/so-sanh-he-thong.md`.

---

## 📤 Output template (daily plan)

```
### Today — [Weekday, day/month]

**Quarter 1 — Morning (Eat the frog)**
- [task #1, time estimate already doubled]

**Quarter 2 — Midday**
- [rest / meal / light task]

**Quarter 3 — Afternoon**
- [admin / light study task]

**Quarter 4 — Evening**
- [relaxation / wind-down]

**3 Action Plans for today:**
1. (Number 1 — mandatory) ...
2. ...
3. ...

**Notebook entry at day's end:** 1 highlight line + tick habits (max 2)
```

---

## 📚 Sources / credit

Synthesized from widely-practiced (non-academic) productivity methods by **Ryder Carroll, Reysu, Nathaniel Drew, Ali Abdaal, Julia Broome, Miles Mochizuki, Justin Sung**, among others. This is a **practical framework**, not a result of randomized controlled trials.

## ⚠️ Limitations

- Not validated by peer-reviewed research — treat as a reference heuristic, not an absolute rule.
- **Not a substitute** for professional help with severe chronic procrastination, clinical ADHD, or depression — the skill explicitly defers to a doctor/therapist in those cases.

## 📄 Metadata

```yaml
name: organize-your-calendar
version: 1.0
category: personal-productivity
language-agnostic: true
```
