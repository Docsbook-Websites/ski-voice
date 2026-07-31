---
title: SKI troubleshooting — install, mic and connection fixes
description: Fixes for a Gatekeeper-blocked install, a SmartScreen warning, a dot that will not turn green, and an agent that hears you but stays silent.
---

# Troubleshooting

<!-- widget:accordion -->

### macOS refuses to open the app

An older copy of SKI can stay Gatekeeper-blocked, and a fresh download does not heal it. Delete `/Applications/SKI.app`, then install again from the DMG. On first launch, the standard "downloaded from the Internet" prompt appears, so click **Open**.

### Windows shows "Windows protected your PC"

The Windows build is not code-signed yet, so SmartScreen warns on first install. Click **More info**, then **Run anyway**. Every automatic update after this is cryptographically signed and verified before it is applied.

### The dot never turns green

The green dot means a live agent session is connected. Check that you installed the skill for that specific agent, that you typed `ski` inside the session, and that the session is still running. The indicator is real-time, so a stale session shows as disconnected rather than green.

### The agent hears me but never speaks

Check whether silent mode is on. In silent mode the agent still receives what you say but replies as text only. Turn it off from the widget hover controls or with its hotkey.

### It sends before I finish my sentence

SKI uses end-of-speech detection to send a thought whole. If it is cutting you off in a noisy room, turn on [approve-before-send](../guides/approve-before-send.md) so every transcript waits in an editable bubble until you confirm it.

### A colleague's voice ends up in my session

Use mute to cut the mic at the source when someone comes over, and consider approve-before-send in shared spaces so nothing reaches the agent unreviewed.

### The recording has no per-person names

Local recordings capture two tracks, your mic and the meeting audio. For a transcript tagged by individual speaker name, [send your agent into the call](../guides/send-your-agent.md) instead.

### I want to check the download is genuine

Run `shasum -a 256` on the downloaded file and compare it against the hash printed in that release's notes.

<!-- /widget -->

## Still stuck

Email support@heyski.io. For what SKI needs from your machine in the first place, see [System requirements](requirements.md).
