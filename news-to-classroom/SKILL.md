---
name: news-to-classroom
description: "Transforms real-world news events into structured teaching material for Business Management, Supply Chain Management, and Data Analytics. Trigger this skill whenever the user shares a news article, event, or trend and wants to use it in teaching — even if they don't say classroom or teaching. Signal phrases: can I use this in class, how do I teach this, make this into a case study, what's the lesson here, help me explain this to students, or when the user shares news about robots, trade, logistics, AI, or business and is an educator. Also trigger when a news story arrives from intel-digest and needs to be made classroom-ready. Composes naturally with linkedin-post and slides-from-content."
---

# News-to-Classroom Skill

Turns current events into ready-to-use teaching material — case study, discussion questions,
and a framing note — grounded in the user's teaching domains: Business Management, Supply
Chain Management, and Data Analytics.

---

## What This Skill Produces

For every news item, output **three things**:

1. **Teaching Note** — A 3–4 sentence framing of the event pitched at the right student level.
2. **Discussion Questions** — 3 questions at increasing depth:
   - Q1: Comprehension — "What happened and why does it matter?"
   - Q2: Analysis — "What are the forces/trade-offs at play?"
   - Q3: Application — "What would you do if you were the decision-maker?"
3. **Concept Tag** — 1–2 curriculum concepts this maps to.

---

## How to Use This Skill

### Step 1 — Identify the news item
The user may share a full article, summary, headline, or link. If a URL, fetch it.

### Step 2 — Identify the teaching domain

| Domain | Signal words |
|---|---|
| Supply Chain Management | logistics, shipping, port, inventory, supplier, warehousing, trade |
| Business Management | strategy, leadership, competition, M&A, corporate decision |
| Data Analytics | data, AI, prediction, automation, measurement, KPIs |

### Step 3 — Identify student level
Default to diploma/undergraduate unless specified:
- **Freshmen / Year 1** — analogies, everyday language, simple cause-effect
- **Diploma / Undergraduate** — introduce frameworks, use terminology
- **Working professionals** — practitioner language, assume domain fluency

### Step 4 — Produce the three outputs
Write the Teaching Note, Discussion Questions, and Concept Tag.

### Step 5 — Offer next steps
Always end with:
> "Want me to turn this into a LinkedIn post? Or build a slide for class?"

---

## Output Format

```
📰 TEACHING NOTE
[3-4 sentences]

💬 DISCUSSION QUESTIONS
Q1 (Comprehension): ...
Q2 (Analysis): ...
Q3 (Application): ...

🏷️ CONCEPT TAGS
[Concept 1] · [Concept 2]

→ Want me to turn this into a LinkedIn post or build a slide deck?
```
