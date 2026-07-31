---
title: How SKI works — widget, skill, and plain files
description: SKI has three moving parts and no daemon or cloud. See how your voice reaches the agent and how its answer gets spoken back to you.
---

# How SKI works

There are three moving parts and none of them is a server.

## The widget

A small floating window on your desktop. On a Mac it docks into the notch, black and flush with the menu bar, or draws its own notch on machines without one. On Windows it floats as a pill wherever you park it.

It rests as a quiet bar, springs open when there is something to say, then folds back. That is the whole interface. There is no main window to manage.

## The skill

A small set of instructions your coding agent already knows how to read. You install it once per agent. It tells the agent to check for what you said and to write back the text it wants spoken aloud.

## The files

The widget and the agent talk through plain files inside your own project. No daemon, no socket to a cloud service, no injected keystrokes. You can open those files, read every byte, and delete them whenever you want.

This is also why SKI is agent-agnostic. Anything that can read and write a file in your repo can be given a voice.

## What runs where

| Step | Where it runs |
|---|---|
| Speech recognition | Your machine |
| The agent doing work | Your machine, in your agent |
| Voice synthesis | Your machine |
| Anonymous usage counts | Sent to PostHog, and you can turn it off |
| Sending an agent into a video call | The cloud, and only if you use it |

## Live agent status

The green dot is not a guess. It reflects whether the agent is actually connected and listening right now, so a dead session cannot look alive.

## Related

Read [Not dictation, a conversation](the-voice-loop.md) for why the return path matters, or [On-device privacy](on-device-privacy.md) for the exact boundary of what leaves your machine. Back to the [documentation home](../README.md).
