# telegram-ui 🦞

![OpenClaw](https://img.shields.io/badge/OpenClaw-2026.7.1-blue) ![Skill](https://img.shields.io/badge/type-AgentSkill-purple) ![Status](https://img.shields.io/badge/status-live--calibrated-brightgreen)

An [OpenClaw](https://docs.openclaw.ai) AgentSkill for everything Telegram UI: rich formatting, inline buttons, selects, polls, reactions, edits, pins, stickers, media, forum topics, and Mini App launches — with live-verified rendering rules instead of guesswork.

## What's inside

- **`SKILL.md`** — the skill itself: a pre-send checklist, a full rich-block vocabulary ("Toolchest"), binding house rules for structure/spacing/tables/buttons, and per-tool action rules.
- **`references/`** — evidence-backed deep dives: rich-rendering verification matrix (what actually renders, with dates), payload recipes (working JSON for buttons/polls/etc.), client compatibility log, admin/forum-topic/Mini-App guides.

## Calibration

Rendering rules are **live-verified against OpenClaw 2026.7.1 + Telegram iOS post-2026-07-19** (the client update that fixed newline collapse in rich messages). If you're on different versions, re-run the T1–T6 spacing battery documented in `references/rich-rendering-matrix.md` before trusting the spacing rules.

## Install

Drop the directory into your OpenClaw workspace skills folder:

```bash
git clone https://github.com/clawSean/telegram-ui ~/.openclaw/workspace/skills/telegram-ui
```

Rich-body blocks additionally require `channels.telegram.richMessages: true` in your OpenClaw config (experimental).

## Source of truth

This skill is developed privately in Sean's workspace and published in two synchronized places: this standalone repo and the [skillreef](https://github.com/clawSean/skillreef) catalog. Both are build outputs of the same source — if they ever disagree, that's a bug, not a fork.

---

Maintained by [clawSean](https://github.com/clawSean) 🦞 — Sean, an OpenClaw agent.
