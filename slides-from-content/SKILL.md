---
name: slides-from-content
description: "Converts structured content — syllabi, teaching notes, markdown, news items, synopses, or any organized text — into a styled HTML slide deck. Trigger this skill when the user wants to turn content into slides, create a presentation from existing material, or build a deck for class. Signal phrases: make this into slides, create a deck from this, build a presentation, turn this into a slide, I need slides for my class, or after news-to-classroom or subject-synopsis-writer produces output and the user wants it visualized. Handles content structuring and aesthetic decisions before calling frontend-slides for rendering. Composes with frontend-slides, news-to-classroom, and subject-synopsis-writer."
---

# Slides-from-Content Skill

Bridges raw content and polished HTML slides — handling structure, aesthetic decisions,
and content chunking before handing off to frontend-slides.

---

## CY's Aesthetic Presets

| Preset | When to use | Style |
|---|---|---|
| **Editorial Dark** | News, case studies, industry topics | Dark bg, bold typography, teal/amber accents |
| **Maritime Signal** | SCM, logistics, trade content | Deep navy, electric teal, cargo amber |
| **Clean Academic** | Course overviews, synopses, freshmen content | Light bg, structured, professional |
| **Apple-Minimal** | Executive presentations | White/off-white, sparse |

Default: Editorial Dark for current events · Clean Academic for teaching content.

---

## How to Use This Skill

### Step 1 — Assess the content type
- News/case study (from news-to-classroom) → Editorial Dark, 3–5 slides
- Subject synopsis (from subject-synopsis-writer) → Clean Academic, 4–6 slides
- Syllabus / course outline → Maritime Signal or Clean Academic, 8–12 slides

### Step 2 — Design the slide structure

**Case Study / News (3–5 slides)**
1. Hook — headline + 1 key fact
2. Context — what happened, key players
3. Analysis — tensions / trade-offs
4. Discussion — 3 questions for class
5. Concept tag — curriculum connection

**Course Overview (5–7 slides)**
1. Title + tagline
2. Why this matters
3. What you'll learn
4. Topic arc / journey
5. How we'll learn
6. Who this is for
7. Next steps

### Step 3 — Chunk content
- Max 40 words of body text per slide
- One idea per slide
- Every slide needs a visual anchor (stat, quote, or image reference)

### Step 4 — Read frontend-slides and hand off
view /mnt/skills/user/fronteApply the aesthetic preset and build the HTML deck.

### Step 5 — Present and offer Drive upload
After creating: present for preview, offer to save to Google Drive.

---

## Content Chunking Rules

- Never put a paragraph on a slide — always break into fragments
- Statistics get their own visual treatment (large type, centered)
- Discussion questions each get their own line
- Concept tags become visual badges, not bullet points
- If a slide feels too full, it becomes two slidesnd-slides/SKILL.md
