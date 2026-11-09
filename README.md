# telegram-ui 🦞

![OpenClaw](https://img.shields.io/badge/OpenClaw-AgentSkill-blue) ![Skill](https://img.shields.io/badge/type-AgentSkill-purple) ![Plugin](https://img.shields.io/badge/plugin-optional-orange)

An OpenClaw skill for Telegram rich formatting, spacing, controls, media, and
client-specific rendering. The skill works by itself; an optional, fail-open
plugin provides narrow last-mile checks.

## Skill-only install

Clone this repository into your OpenClaw workspace's `skills/telegram-ui`
directory. Tell your agent to use the `telegram-ui` skill for Telegram output.
Check your selected Telegram account's rich-message setting and run a client
canary before relying on break tags or advanced blocks.

## Optional plugin

The same checkout contains an OpenClaw plugin. See [PLUGIN.md](PLUGIN.md) for
the opt-in install command, modes, and exact repair scope. Its default `warn`
mode never changes or cancels a message. The `repair` mode addresses only a
proven heading boundary; it does not automatically add spacing to every line.

## Evidence and source

The [rendering matrix](references/rich-rendering-matrix.md) records what was
actually observed on specific Telegram clients. This repository and the
[skillreef catalog](https://github.com/clawSean/skillreef) are synchronized
public outputs of Sean's canonical workspace skill.
