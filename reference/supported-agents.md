---
title: Coding agents supported by SKI
description: Claude Code, Codex, Cursor, Gemini CLI, Windsurf and OpenClaw, with the install scope for each and what one-click setup covers.
---

# Supported agents

SKI installs a small skill per agent. Most are one click. The scope column says where the skill lands: at the user level, per project, or both.

| Agent | Install scope | Setup |
|---|---|---|
| Claude Code | User and project | One click |
| Codex | User and project | One click |
| Cursor | Project | One click |
| Gemini CLI | User | One click |
| Windsurf | Manual | Manual install |
| OpenClaw | User | One click |

## Running several at once

You are not limited to one agent. Connect a Claude Code session in one repo and a Codex session in another and both stay live, each answering in its own voice. See [Multi-project routing](../concepts/multi-project.md).

## What the skill actually does

It teaches the agent two things: check for what the user just said, and write back the text you want spoken. Everything moves through plain files in your project, which is why the same small skill works across agents that share almost no internals. See [How SKI works](../concepts/how-it-works.md).

## Related

Start at [Connect your agent](../getting-started/connect-your-agent.md) for the step-by-step.
