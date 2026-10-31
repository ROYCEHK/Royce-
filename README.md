# Royce – Agent Skills & Consulting Practice

Skills and agents for Royce's agent hierarchy. This adds a consulting practice in the style of a strategy-consulting firm, with 21 skills, run by a Chief of Consultant who reports to the Chief of Commander.

The skills are original work built around common consulting topics. They are not affiliated with or endorsed by McKinsey & Company or Anthropic.

## Hierarchy
```
Chief of Commander (main go-to agent)
├── Chief of Staff – Second Brain      (existing skill: second-brain-chief-of-staff)
├── OCSiAl Command roster              (existing skill: ocsial-command)
├── INVEST001 Research Desk            (existing skill: invest001-research-desk)
├── Chief of Travel                    (existing skill: royce-travel-desk)
└── Chief of Consultant  ── MCKINSEY 003 practice
    ├── Strategy Partner                 01 Problem-Framing · 02 Situation Assessment · 03 Assumption Audit · 08 Strategic Options · 16 War-Gaming
    ├── Markets & Customers Partner      04 Market Mapping · 05 Competitive Intelligence · 06 Customer Segmentation · 07 Profit Pool · 09 Pricing Strategy
    ├── Corporate Finance Partner        10 Business Case · 11 Portfolio Review · 13 Initiative Prioritisation
    ├── Operations & Transformation      12 Operating Model · 14 Transformation Roadmap · 15 Risk Mitigation · 17 KPI Architecture
    ├── Communications & Decisions       18 Stakeholder Alignment · 19 Narrative Builder · 20 Decision Memo
    └── Engagement Sceptic (red team)
    21 Reusable Consulting Operating System → consult-operating-system (owned by the Chief of Consultant)
```

## Layout
- `.claude/skills/` holds one folder per skill (`SKILL.md`). Claude Code loads these automatically in this repo.
- `.claude/agents/` holds the subagent definitions with their roles and responsibilities.
- `dist/` holds one `.zip` per skill, for upload to claude.ai (Settings → Capabilities → Skills), so the skills work in the Claude apps as well.

## Google Drive: MCKINSEY 003
Folder id `1W2JP-je_oC_qB7vwP8RAUpRh80ivpMKc`. The subfolders and their ids are listed in `.claude/skills/consult-operating-system/SKILL.md`.

## Usage
- `Commander: <task>` lets the Commander route the task.
- `Chief of Consultant: should we enter the Korean dispersion market?` starts an engagement.
- `Pricing Partner / Markets Partner: <task>` goes straight to a practice.
