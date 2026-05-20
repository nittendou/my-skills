# my-skills
my custom Claude agent skills — SCM, teaching, and productivity

# Claude Agent Skills

Custom skills for Claude Code and AI agents — built at the intersection of 
Supply Chain Management, Business Management, Data Analytics, and Teaching.

## Install All Skills

```bash
npx skills add chooyen/cy-skills
```

## Available Skills

| Skill | What it does |
|---|---|
| `news-to-classroom` | Turns news into teaching notes + discussion questions |
| `linkedin-post` | Drafts LinkedIn posts in practitioner + educator voice (2 variants) |
| `subject-synopsis-writer` | Rewrites academic synopses for poly/diploma level |
| `rfq-drafter` | Drafts RFQs, RFPs, and spec sheets for SCM procurement |
| `intel-digest` | Weekly digest from Gmail + web, filtered for SCM/BM/AI |
| `slides-from-content` | Converts content into styled HTML slide decks |

## Skill Composition

intel-digest → news-to-classroom → linkedin-post
news-to-classroom → slides-from-content
subject-synopsis-writer → slides-from-content

## Context
Built by a citizen data scientist and educator teaching SCM and Business. Skills are designed to be nimble and composable.
rfq-drafter → ai-scm-prompts
