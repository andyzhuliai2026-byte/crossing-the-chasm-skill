# Crossing the Chasm — Agent Skill

A structured agent skill distilled from **Geoffrey A. Moore's *Crossing the Chasm*** (3rd edition, 2014), built for use with Claude Code, Claude.ai Skills, and other compatible agent runtimes.

This skill is **knowledge as a toolkit, not as a summary** — it captures Moore's named frameworks, mental models, scoring checklists, positioning templates, distribution-channel matrices, anti-patterns, and post-chasm phases in a form an agent can navigate and apply to real go-to-market decisions.

## What it covers

- **Technology Adoption Life Cycle (TALC)** — five psychographic segments and the gaps between them
- **The Chasm** — why visionary references don't transfer to pragmatists
- **D-Day Strategy** — concentrating force on a single beachhead niche
- **Market Development Strategy Checklist** — 9-factor beachhead scoring (4 showstoppers + 5 nice-to-haves)
- **The Whole Product Model** — Levitt's 4 layers (generic / expected / augmented / potential)
- **Create the Competition** — market alternative + product alternative
- **Competitive Positioning Compass** — 4 quadrants × 4 positioning stages
- **Two-sentence positioning template** + the elevator test
- **5 customer-oriented distribution channels** matched to 5 customer types
- **3 pricing models** (value / competition / cost based) + channel-motivation premium
- **Staircase vs. Hockey Stick** revenue planning, Pioneer vs. Settler organizational shift
- **Appendix 1**: full High-Tech Market Development Model (Early Market → Chasm → Bowling Alley → Tornado → Main Street)
- **Appendix 2**: Four Gears Model for consumer-digital adoption (Acquire / Engage / Enlist / Monetize)

## Layout

```
.
├── SKILL.md                            # Master file — core frameworks, chapter index, topic index
├── chapters/                           # On-demand chapter files
│   ├── ch00-introduction.md
│   ├── ch01-marketing-illusion.md
│   ├── ch02-marketing-enlightenment.md
│   ├── ch03-d-day-analogy.md
│   ├── ch04-target-point-of-attack.md
│   ├── ch05-assemble-invasion-force.md
│   ├── ch06-define-the-battle.md
│   ├── ch07-launch-the-invasion.md
│   ├── ch08-conclusion.md
│   ├── ch09-appendix-market-dev-model.md
│   └── ch10-appendix-four-gears.md
├── glossary.md                         # Every key term, alphabetical, with chapter pointers
├── patterns.md                         # 13 actionable playbook patterns (When / How / Trade-offs)
└── cheatsheet.md                       # Single-page tables — TALC, channel ↔ customer, decision rules
```

The on-demand chapter files do not count against your context window until loaded. The agent reads only the files relevant to your question.

## Installation

### Claude Code
Clone or copy this repo into your Claude Code skills directory:

```bash
git clone https://github.com/andyzhuliai2026-byte/crossing-the-chasm-skill.git \
  ~/.claude/skills/crossing-the-chasm
```

Restart Claude Code or start a new session — the skill auto-loads when you mention chasm-crossing topics in either English or Chinese (`鸿沟`, `跨越鸿沟`, `立足点市场`, `务实主义者`, `市场战略`, etc.).

### Claude.ai (web/desktop)
1. Download this repo as a `.zip` (GitHub → Code → Download ZIP), or `git archive`:
   ```bash
   git archive --format=zip --output=crossing-the-chasm.zip HEAD
   ```
2. Open **claude.ai → Settings → Capabilities → Skills**
3. Click **Upload skill** and select the `.zip`

> Custom skill uploads on claude.ai require the **Skills** capability to be enabled on your account.

### Other agent runtimes
Any runtime that follows the Agent Skills convention (a folder with `SKILL.md` containing YAML frontmatter) should pick this up. Adjust the install path accordingly.

## How to invoke

| Prompt | What happens |
|---|---|
| *"Help me cross the chasm with our hardware product."* | Loads `SKILL.md` core frameworks |
| *"What's the beachhead scoring checklist?"* | Loads `ch04` for the Market Development Strategy Checklist |
| *"How should we price during the chasm?"* | Loads `ch07` for the pricing section |
| *"用跨越鸿沟模型诊断一下我们的销售卡点。"* | Triggers in Chinese; runs the diagnostic |
| *"What does Moore say about hockey-stick forecasts?"* | Loads `ch08` (Conclusion) |
| *"Show me the patterns for whole-product planning."* | Reads `patterns.md` |

## Generation provenance

This skill was generated using the [`book-to-skill`](https://github.com/anthropics/claude-skills) converter — a structured extraction tool that pulls frameworks, principles, techniques, and anti-patterns from books and turns them into reusable agent toolkits. The source was an EPUB of the 3rd edition (2014).

## Source

> Moore, Geoffrey A. *Crossing the Chasm: Marketing and Selling Disruptive Products to Mainstream Customers*. 3rd edition. HarperBusiness, 2014.

For the full post-chasm playbook, also read Moore's *Inside the Tornado* and *The Gorilla Game*.

## License

The skill files in this repository are derivative summaries created for personal study and agent use. The underlying frameworks, terminology, and case studies are the intellectual property of **Geoffrey A. Moore** and his publishers. This repository is **not** affiliated with or endorsed by the author or HarperBusiness.

If you have not already, **buy the book**. The full text is irreplaceable.
