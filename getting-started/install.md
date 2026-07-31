---
title: Install SKI on macOS or Windows
description: Download the SKI installer, get past the first-launch security prompt, and confirm the version. Takes about two minutes, no credit card.
---

# Install SKI

One installer, one setup wizard, and you are done. SKI asks for your microphone, a voice, and a hotkey, then gets out of the way.

<!-- widget:stepper -->

### Download the installer

Get the newest build from the [SKI releases page](https://github.com/pattern-ai-labs/ski-releases/releases/latest) or straight from [heyski.io](https://heyski.io).

| Platform | File | Requirements |
|---|---|---|
| macOS (Apple Silicon) | `SKI_<version>_aarch64.dmg` | macOS 14.4 Sonoma or newer, M1 or later |
| Windows | `SKI_<version>_x64-setup.exe` | Windows 10 or 11, x64 |

### Install on macOS

If a previous copy of SKI exists, delete `/Applications/SKI.app` first. Old copies can stay Gatekeeper-blocked, and a fresh download will not heal them.

Open the DMG and drag SKI into Applications. The first launch shows the standard "downloaded from the Internet" prompt, so click **Open**.

### Install on Windows

Run the installer. Windows may show a SmartScreen notice because the build is not code-signed yet. Click **More info**, then **Run anyway**, and follow the prompts.

Every automatic update after this is cryptographically signed and verified before it is applied, so a compromised download host cannot push a tampered build to you.

### Verify the download

Each release prints its expected hash in the release notes. Compare it:

```bash
shasum -a 256 SKI_<version>_aarch64.dmg
```

### Confirm the version

Open **SKI → Preferences → About**. The version shown there should match the release you downloaded.

<!-- /widget -->

## Registration

After a short trial, continued use asks for a free sign-in. No card, no subscription. Voice coding, the local meeting recorder, and everything else on-device stay free for life.

## Automatic updates

Once installed, SKI checks for new releases on its own. On macOS the update downloads in the background and applies when you relaunch. On Windows you click **Restart now** in Preferences → About and the installer runs.

## Next

The app is installed but it cannot hear your agent yet. Continue with [Connect your agent](connect-your-agent.md), or read [System requirements](../reference/requirements.md) if the install did not go through.
