---
name: intel-digest
description: "Scans email, web alerts, and current news to produce a prioritized intelligence digest tailored to CY's teaching and professional domains: Supply Chain Management, Business Management, Data Analytics, and AI tools. Trigger this skill when the user asks to check emails for priorities, review what's happening in the news this week, get a morning briefing, or surface relevant industry developments. Signal phrases: what should I focus on this week, check my emails and summarize, what's happening in SCM or logistics or AI, give me my weekly digest, morning briefing, what's worth reading today, scan my inbox. Composes with news-to-classroom and linkedin-post."
---

# Intel Digest Skill

Surfaces what matters from email, alerts, and the web — filtered through CY's teaching
and professional lens.

---

## What This Skill Produces

Three sections:
1. **Action Items** — Things needing response or decision (from email)
2. **Domain Intelligence** — Notable developments in SCM, BM, Data/AI (from web)
3. **Classroom Currency** — News items worth using in teaching

---

## How to Use This Skill

### Step 1 — Determine scope
- "Check my email" → Gmail only
- "What's happening this week" → Web search
- "Full digest" → Gmail + Web + flag classroom material

### Step 2 — Scan Gmail (if included)
Query: `in:inbox newer_than:7d -from:newsletter -from:noreply category:primary`
Surface max 3 action items ranked by urgency.

### Step 3 — Scan domain news (if included)

| Domain | Search queries |
|---|---|
| Supply Chain | "supply chain news [week]", "Singapore logistics [month]" |
| Business Management | "business strategy news [month]", "enterprise AI [month]" |
| Data / AI | "AI tools education [month]", "Claude Anthropic [month]" |

Limit to 2–3 items per domain. Prioritize Singapore/APAC relevance.

### Step 4 — Flag classroom currency
Tag items with 🎓 that could work in teaching. Cues user to chain with news-to-classroom.

### Step 5 — Offer next steps
> "Want me to turn any of these into a teaching note or LinkedIn post?"

---

## Output Format
