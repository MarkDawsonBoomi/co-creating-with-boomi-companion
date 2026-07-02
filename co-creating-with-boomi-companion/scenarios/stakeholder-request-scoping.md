---
type: Scenario
title: Stakeholder Request Scoping
description: A vague stakeholder request becomes a buildable scope through the questions a senior developer asks before opening Boomi Companion.
tags: [scenario, planning, scoping, boomi-companion]
timestamp: 2026-07-01T00:00:00Z
source_video: Collaborating a Build-.mp4
source_captions: ai-captions-1782154409521.vtt
related_module: /modules/04-planning-together.md
---

# Setup

A stakeholder messages you:

> Can you help us build an integration that syncs orders from our store to our finance system?

The only problem is that is everything you have. Technically it is a request, but it's not really a buildable one yet, unless you are OK with spending a lot of tokens.

# The senior-developer questions

Before you open Boomi Companion, you ask the questions a senior developer would:

- Which store?
- Which finance system?
- Which environment?
- What does *sync* mean here? All orders, or only certain ones?
- In real time, or in batches?
- What happens when an order fails to sync? Who needs to know?
- Is there an existing integration we are looking at replacing, or is this net new?

Some of these you'll know. Some you'll ask the business. Some you'll ask your team.

# Opening Companion

Now you open Boomi Companion — not necessarily with a perfect prompt, but with a conversation:

> I need to sync new orders from System A to System B, batches every 15 minutes with email notification on failure. What would you do and what would you need from me to get started?

# The goal of the opening prompt

The goal at this point isn't a perfect prompt. It's a *shared understanding of what's being built and what each of you is responsible for.*

# Related

- Module: [Planning Together](/modules/04-planning-together.md)
- Concept: [Boomi Companion](/concepts/boomi-companion.md)
- Concept: [Conversational Mode](/concepts/conversational-mode.md)

# Citations

[1] Source captions: `scormcontent/assets/ai-captions-1782154409521.vtt` in the original SCORM package
