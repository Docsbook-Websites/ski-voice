---
title: SKI system requirements for macOS and Windows
description: Supported operating systems, chips, and what SKI needs from your microphone and speakers to run the full on-device voice loop.
---

# System requirements

Everything runs locally, so the requirements are about your machine rather than your connection.

## macOS

- macOS 14.4 Sonoma or newer
- Apple Silicon, M1 or later
- Builds are Developer-ID signed and notarized

## Windows

- Windows 10 or 11, x64
- Builds are not code-signed yet, so SmartScreen may warn on first install. Automatic updates after that are cryptographically signed and verified.

## Audio

Any microphone works. Open speakers are fine because full-duplex echo cancellation keeps the agent's own voice out of the transcript, which is what makes barge-in possible without a headset.

## Network

None required for the core loop. Speech recognition and the neural voice both run on-device, so voice coding and local meeting recording work fully offline.

A connection is needed for two things: the free sign-in after the trial, and [sending your agent into a video meeting](../guides/send-your-agent.md), which by definition happens in the cloud.

## Related

Go to [Install SKI](../getting-started/install.md), or check [Troubleshooting](troubleshooting.md) if an install already failed.
