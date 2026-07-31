---
title: On-device privacy — what never leaves your machine
description: SKI processes speech, code, and transcripts locally. See exactly what stays on disk, what anonymous data is collected, and how to turn it off.
---

# On-device privacy

The short version: your voice never leaves your machine. Speech-to-text and the synthesized voice both run on-device. Your audio, transcripts, code, and file contents are never uploaded.

## What stays local, always

- Spoken audio and its transcript
- The code and file contents your agent reads or writes
- Your project names and paths
- Locally recorded meetings and their transcripts

There is no upload path for any of it. Nothing to opt out of, because there is nothing to opt out from.

## What is collected

**Anonymous product analytics.** With your consent, a setting that is on by default and switchable in **Preferences → About → Privacy**, SKI sends anonymous usage statistics: counts and durations of features used, coarse device facts such as chip family and CPU cores, the app version, and a random install identifier. No account identity is attached. The vendor knows that an install exists, never whose it is.

In those analytics, "words" is a count. Never the text.

**Website analytics.** heyski.io uses Google Analytics 4 and the Google Ads tag for conversion measurement, and is served through Cloudflare, which processes standard request logs.

**Account data.** Continued use asks for a free sign-in through AgentCall, which creates an account from the email and sign-in identity you provide.

## The one cloud feature

Sending your agent into a video meeting runs in the cloud, because the call does. That mode processes meeting audio, transcripts, and chat in order to work. It is the only feature that does.

Recording a meeting locally is the opposite: audio is captured and transcribed entirely on your disk. See [Record a meeting locally](../guides/record-a-meeting.md) for the difference in practice.

## Approve before anything is sent

If you want a checkpoint between your mouth and the agent, turn on [approve-before-send](../guides/approve-before-send.md). Every transcript lands in an editable bubble and nothing moves until you confirm it.

## Related

[How SKI works](how-it-works.md) shows the file-based plumbing behind these guarantees.
