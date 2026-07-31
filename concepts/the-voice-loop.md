---
title: Not dictation — why the voice loop closes
description: Dictation tools stop at text-in. SKI speaks the answer back, handles barge-in, and knows when your thought is finished. Here is why that matters.
---

# Not dictation. A conversation.

Dictation is one-directional. You talk, text appears, and you go back to reading. Your eyes are still the bottleneck, so you have not really left the keyboard, you have only changed how characters get into it.

SKI closes the loop. The agent's reply is synthesized on your machine and spoken aloud, which means the whole exchange can happen while you are looking at something else, or nothing at all.

## What closing the loop requires

**Speaking back.** A neural voice runs on-device, so a reply is spoken without a round trip to a server, and it works offline.

**Barge-in.** Full-duplex echo cancellation lets you interrupt the agent mid-sentence on open speakers. Without it you would be stuck with push-to-talk, waiting politely for a paragraph you already understood.

**Knowing when you are done.** Smart end-of-speech detection sends your thought whole rather than cutting it at the first breath.

**A voice per project.** When several repos are connected, each answers in its own voice. You can tell who is talking without checking the widget.

## What this changes in practice

You can pace the room while a build runs and hear what broke. You can be in a meeting and build live. You can be looking at a design in another window and ask why a component is misaligned, with a [screenshot riding along with your sentence](../guides/hotkeys-and-controls.md).

The agent stops being a window you have to visit and becomes something closer to a teammate at the next desk.

## Related

See [How SKI works](how-it-works.md) for the mechanics underneath, or [Your first conversation](../getting-started/first-conversation.md) to try it.
