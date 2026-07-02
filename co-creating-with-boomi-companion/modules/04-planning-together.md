---
type: Module
title: Planning Together
description: Teaches the scoping questions a senior developer asks before opening Boomi Companion, so the first prompt is a conversation rather than a guess.
module_number: 4
tags: [module, planning, scoping, boomi-companion]
timestamp: 2026-07-01T00:00:00Z
source_asset: 4_planning_together.png
---

# What this module covers

Before opening Boomi Companion, developers should ask the questions a senior developer would. Vague stakeholder requests, however well-intentioned, are not buildable and burn tokens when handed straight to an AI.

# The stakeholder scenario

A stakeholder messages you: "Can you help us build an integration that syncs orders from our store to our finance system?" That is technically a request. It is not yet a buildable one.

The [stakeholder request scoping](/scenarios/stakeholder-request-scoping.md) scenario walks through the questions you ask before you open Companion:

- Which store, specifically?
- Which finance system?
- Which environment?
- What does *sync* mean here? All orders, or only certain ones?
- Real time, or batches?
- What happens when an order fails to sync? Who needs to know?
- Is there an existing integration you're looking at replacing, or is this net new?

Some of these you already know. Some you ask the business. Some you ask your team. All of them should be at least attempted before Companion enters the picture.

# The first prompt is a conversation

The goal of the opening prompt is not perfection. It is a *shared understanding of what's being built and what each of you is responsible for.* A first prompt might look like:

> I need to sync new orders from System A to System B, batches every 15 minutes with email notification on failure. What would you do and what would you need from me to get started?

# Related

- Scenario: [stakeholder request scoping](/scenarios/stakeholder-request-scoping.md)
- Concept: [Boomi Companion](/concepts/boomi-companion.md)
- Module: [Stopping](/modules/05-stopping.md) is the bookend to Planning Together
