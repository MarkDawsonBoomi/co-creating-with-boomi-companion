---
type: Interaction Mode
title: Conversational Mode
description: Working with Boomi Companion through natural-language prompts to scope, plan, and iterate.
tags: [boomi-companion, interaction-mode, prompting]
timestamp: 2026-07-01T00:00:00Z
source_asset: Conversational.BC.png
---

# What it is

Conversational mode is the natural-language surface of [Boomi Companion](/concepts/boomi-companion.md). Developers describe intent, ask questions, provide inputs and outputs, and iterate through dialogue.

# What it's good for

- Framing a new integration request.
- Asking Companion to make a plan and check in on what it will need from you.
- Providing JSON/XML samples for mapping.
- Confirming assumptions before Companion commits work to the canvas.

# What it's not for

- Verifying the actual shape of what Companion built. That happens in [canvas mode](/concepts/canvas-mode.md).
- Running production tests. Companion's own test runs are visible in execution logs, but developers should also run their own tests from the canvas.

# The first prompt

A good first prompt is a *conversation opener*, not a spec. Example, from [planning together](/modules/04-planning-together.md):

> I need to sync new orders from System A to System B, batches every 15 minutes with email notification on failure. What would you do and what would you need from me to get started?

# Related

- [Canvas Mode](/concepts/canvas-mode.md)
- Module: [Conversational and Canvas](/modules/02-conversational-and-canvas.md)
