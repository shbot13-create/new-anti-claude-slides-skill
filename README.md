# New Anti-Claude Slides Skill (V2)

A Claude Code skill for building dense, institutional, fact-card slide decks:
Montserrat only, single-line titles, no em-dashes, facts-only with flagged opinions,
optional named palettes (ODA), sanctioned real vendor logos, an entity-profile card
template, and an airy logo-row variant for overloaded slides.
Outputs self-contained 1280x720 HTML per slide, a merged PDF, and (on request)
a fully native, editable PPTX.

V2 of the original anti-claude-slides skill: the base hard rules plus ten
user-added rules (see the "V2 RULES" section in `SKILL.md`) and a matching
audit gate in `checklist.md` section 9.

## Install on another computer

```bash
git clone https://github.com/sadaalfan/new-anti-claude-slides-skill.git \
  ~/.claude/skills/New-anti-claude-slides-skill
```

Restart Claude Code (or start a new session) and the skill appears in the skill
list as `New-anti-claude-slides-skill`.

## Contents

- `SKILL.md` — the binding spec: base hard rules + V2 rules
- `checklist.md` — the per-slide audit gate (run on every slide before delivery)
- `assets/tokens.css` — palette + type scale + flat primitives (inlined into every slide)
- `assets/cover.html` — the one sanctioned starter (deck cover); everything else is composed fresh
