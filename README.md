> **Note:** This repository contains DigiCovAI's collection of skills for Claude. For information about the Agent Skills standard, see [agentskills.io](http://agentskills.io).

# Skills

Skills are folders of instructions, scripts, and resources that Claude loads dynamically to improve performance on specialized tasks. Skills teach Claude how to complete specific tasks in a repeatable way, whether that's building presentation decks from a single prompt, generating LinkedIn posts in your own voice, analysing meeting transcripts for action items, or processing PDF documents automatically.

For more information, check out:
- [What are skills?](https://support.claude.com/en/articles/12512176-what-are-skills)
- [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [How to create custom skills](https://support.claude.com/en/articles/12512198-creating-custom-skills)
- [Equipping agents for the real world with Agent Skills](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills)

---

# About This Repository

This repository contains 5 production-ready Claude skills built by **DigiCovAI** that cover the most common high-value business workflows — content creation, document generation, web design, meeting analysis, and file management.

Each skill is self-contained in its own folder with a `SKILL.md` file containing the instructions and metadata that Claude uses. Browse through these skills to get inspiration for your own skills or to understand different patterns and approaches.

## Disclaimer

**These skills are provided for demonstration and educational purposes only.** While some of these capabilities may be available in Claude, the implementations and behaviors you receive from Claude may differ from what is shown in these skills. These skills are meant to illustrate patterns and possibilities. Always test skills thoroughly in your own environment before relying on them for critical tasks.

---

# Skill Sets

- [./pptx](./pptx): Generate complete PowerPoint presentation decks from a single prompt
- [./frontend-design](./frontend-design): Build responsive, modern websites from a plain-English description
- [./linkedin](./linkedin): Create high-performing LinkedIn posts in your own voice
- [./meeting-insights-analyzer](./meeting-insights-analyzer): Convert meeting transcripts into structured summaries and action items
- [./pdf](./pdf): Merge, split, extract, OCR, and manage PDF documents

---

# Try in Claude Code, Claude.ai, and the API

## Claude Code

You can register this repository as a Claude Code Plugin marketplace by running the following command in Claude Code:

```
/plugin marketplace add digicovai/Claude-Anthropic
```

Then, to install the skill bundle:

1. Select `Browse and install plugins`
2. Select `anthropic-agent-skills`
3. Select `document-skills`
4. Select `Install now`

Alternatively, directly install the plugin via:

```
/plugin install document-skills@anthropic-agent-skills
```

After installing the plugin, you can use any skill by just mentioning it. For instance:

```
Use the PPTX skill to create a 10-slide pitch deck for a SaaS product targeting HR teams
```

```
Use the PDF skill to extract all form fields from path/to/report.pdf
```

```
Use the LinkedIn skill to write a post about closing my first enterprise client
```

## Claude.ai

To use any skill from this repository or upload custom skills, follow the instructions in [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude#h_a4222fa77b).

1. Open [claude.ai](https://claude.ai) and go to a **Project**
2. Upload the `SKILL.md` file from any skill folder as a project document
3. Claude will apply the skill automatically for every conversation in that project

## Claude API

You can upload custom skills via the Claude API. See the [Skills API Quickstart](https://docs.claude.com/en/api/skills-guide#creating-a-skill) for more.

---

# The 5 Skills

### 📊 PPTX — Presentation Deck Generator
**Folder:** [`./pptx`](./pptx)

Generates complete, formatted presentation decks from a text description. Provide a topic, audience, and rough outline — Claude builds the slides with titles, bullet points, logical flow, and optional speaker notes.

**Example:**
```
Create a 10-slide pitch deck for a SaaS product targeting HR teams,
include an executive summary, problem, solution, pricing, and next steps
```

---

### 🌐 Frontend Design — Website Builder
**Folder:** [`./frontend-design`](./frontend-design)

Gives Claude deep knowledge of modern web design — layouts, typography, responsive behaviour, colour systems, and UI components — so it can build polished, professional websites from a single description. No designer, no template, no code required.

**Example:**
```
Build a landing page for my productivity app with a hero section,
feature grid, testimonials, and a pricing table
```

---

### 💼 LinkedIn — Post Generator
**Folder:** [`./linkedin`](./linkedin)

Generates high-performing LinkedIn posts in a candid, direct, no-BS tone — structured around proven engagement formats: hook, insight, breakdown, and takeaway. No corporate jargon, no motivational fluff.

**Example:**
```
Write a LinkedIn post about why most founders validate too late
and what the right sequence should be
```

---

### 🎙️ Meeting Insights Analyzer
**Folder:** [`./meeting-insights-analyzer`](./meeting-insights-analyzer)

Analyses meeting transcripts to surface key discussion points, decisions made, and action items with named owners and deadlines. Turns every meeting into a structured, searchable record.

**Example:**
```
Summarise this meeting transcript, identify all decisions made,
and list action items with the responsible person for each
```

---

### 📁 PDF — Document Tools
**Folder:** [`./pdf`](./pdf)

A comprehensive PDF skill — extract text, tables, and images from PDFs, merge and split documents, rotate pages, add watermarks, fill forms, encrypt files, and run OCR on scanned documents to make them searchable.

**Example:**
```
Merge these three quarterly reports into one PDF
and extract a summary table of the key financial figures
```


# About DigiCovAI

**DigiCovAI** builds Claude skills and AI-powered workflows to help businesses automate high-value, repetitive tasks.

- [digicovai@gmail.com](mailto:digicovai@gmail.com)
- [github.com/digicovai](https://github.com/digicovai)
