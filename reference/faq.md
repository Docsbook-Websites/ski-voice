---
title: SKI FAQ — voice coding questions answered
description: What SKI is, which agents it works with, whether it needs internet, what it costs, and where your transcripts live. Short answers, in one place.
---

# FAQ

<!-- widget:accordion -->

### What is SKI?

A voice layer for your coding agent. You speak, your agent works, and it answers out loud in a natural voice generated on your machine. It runs on macOS and Windows and is free for life.

### How is this different from dictation tools?

Dictation stops at text-in. SKI speaks the reply back, supports barge-in over open speakers, and detects when your thought is finished. See [Not dictation, a conversation](../concepts/the-voice-loop.md).

### Which coding agents can I talk to?

Claude Code, Codex, Cursor, Gemini CLI, Windsurf, and OpenClaw. Most install with one click, and you can connect several projects from different agents at the same time. See [Supported agents](supported-agents.md).

### Does SKI type into my editor or terminal?

No. It talks to your agent through a skill and plain files inside your own project. Nothing is injected into windows or keystrokes, which is why it works with any terminal, editor, or IDE.

### Do I need an internet connection?

Not for voice coding or local meeting recording. Speech recognition and the voice both run on your own machine, so the loop works offline. A connection is needed for the free sign-in and for [sending your agent into a meeting](../guides/send-your-agent.md).

### Is my voice recorded or sent anywhere?

No. Audio, transcripts, code, file contents, and project paths from local use are never uploaded. Anonymous usage counts go to PostHog and can be turned off in **Preferences → About → Privacy**. See [On-device privacy](../concepts/on-device-privacy.md).

### Can I review what I said before it is sent?

Yes. Turn on [approve-before-send](../guides/approve-before-send.md) and every transcript waits in an editable bubble until you confirm it.

### Is there push-to-talk?

On macOS you can opt in to the globe or fn key: tap to mute or unmute, hold to talk. Custom bindings live in **Preferences → Hotkeys**.

### How much does it cost?

Free for life, no card. The only paid feature is sending your agent into a video meeting, billed per minute with free hours included. See [Pricing](pricing.md).

### Is meeting recording really unlimited?

Yes. Your machine does the recording and transcription, so there are no minutes to buy and no caps on length or retention.

### Does a bot join my call when I record?

No. Local recording captures audio on your machine only, and nothing changes for the other participants. Sending your agent is the mode where a visible participant joins.

### Where do my transcripts live?

On your disk, in SKI's Transcripts window. View, edit, copy, export as Markdown or plain text, or delete them at any time.

### What do I need to run it?

macOS 14.4 or newer on Apple Silicon, or Windows 10 or 11 on x64. See [System requirements](requirements.md).

<!-- /widget -->

## Still have a question

Email support@heyski.io, or start from the [documentation home](../README.md).
