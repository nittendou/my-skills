---
name: rfq-drafter
description: "Drafts professional procurement documents — RFQs, RFPs, and specification sheets — for supply chain and business contexts. Trigger this skill when the user asks to draft, write, or create any procurement document, sourcing request, or vendor document. Signal phrases: help me draft an RFQ, write an RFP, create a spec sheet, I need to source [commodity], help me get quotes for, draft a tender document, or any mention of procuring goods, services, or equipment. Also trigger when teaching procurement document writing as a classroom exercise. Composes with ai-scm-prompts and linkedin-post."
---

# RFQ Drafter Skill

Produces structured, professional procurement documents ready to send or use as teaching
examples — grounded in real SCM practice.

---

## Document Types

| Type | When to use |
|---|---|
| **RFQ** | Standard goods/services with known specs — need price comparison |
| **RFP** | Complex/strategic procurement — need approach + price |
| **Spec Sheet** | Technical specification for a single item |
| **Evaluation Matrix** | Scoring template to compare vendor responses |

Default to **RFQ** unless the ask is clearly complex or strategic.

---

## How to Use This Skill

### Step 1 — Understand the context
Identify: what's being procured, one-time or recurring, detail level needed.

### Step 2 — Load the relevant reference file

| Procurement type | Reference file |
|---|---|
| Physical goods / equipment | `.doc/rfq-goods.md` |

### Step 3 — Draft the document

Standard RFQ structure:
1. Header — Reference number, issuer, issue date, deadline
2. Purpose & Scope
3. Specifications — table format preferred
4. Commercial Requirements — pricing, Incoterms, payment terms, lead time
5. Supplier Qualification — minimum criteria
6. Submission Instructions
7. Evaluation Criteria — weighted scoring

### Step 4 — Flag placeholders
List 3–5 things the user must complete before sending.

### Step 5 — Offer next steps
> "Want me to turn this into a Word doc? Or build an evaluation matrix?"

---

## Format Rules

- Use tables for specifications
- Use checkboxes for supplier qualification criteria
- Always include weighted evaluation criteria
- For teaching: flag as illustrative, simplify specs
