---
type: Concept
title: Skill Folders
description: The mechanism by which Boomi Companion is grounded in Boomi platform knowledge — a folder of skill definitions the agent draws on.
tags: [boomi-companion, skills, agent-architecture]
timestamp: 2026-07-01T00:00:00Z
source_asset: 01_skill_folders.png
---

# What they are

Skill folders are the mechanism that grounds [Boomi Companion](/concepts/boomi-companion.md) in Boomi-specific platform knowledge. Rather than relying on a general model's guesses about Boomi, Companion consults skill definitions that describe how the platform actually works.

# Why they matter

The course frames this as "the agent skill closes the gap." A raw language model may know that Boomi exists and roughly what an integration looks like, but it will make assumptions that do not survive contact with your tenant. Skill folders fill that gap by giving Companion a concrete, up-to-date model of the platform.

# Related

- [Boomi Companion](/concepts/boomi-companion.md)
- Module: [Introduction](/modules/01-introduction.md)
