---
type: Concept
title: Connector Registry
description: The Boomi catalog of connectors, operations, and credentials that defines what Boomi Companion can plan integrations against.
tags: [boomi-companion, connectors, registry]
timestamp: 2026-07-01T00:00:00Z
source_asset: M3-B4_connector-registry-f.png
---

# What it is

The connector registry is the Boomi catalog of connectors available in your tenant. It defines the surface area [Boomi Companion](/concepts/boomi-companion.md) can plan against.

# Why it matters

Companion's plans are grounded in what actually exists. A connector missing from the registry cannot appear in a Companion-authored process. A connector present but not credentialed can appear in a plan but not execute at test time. Understanding the registry helps developers pre-empt scope questions before they blow up mid-session.

# Practical checks before you build

- Is the connector for the system your stakeholder mentioned in the registry?
- Is it credentialed for the environment you plan to test in?
- If not, do you need to raise that as blocking scope before opening Companion?

# Related

- Module: [Connector Registry](/modules/03-connector-registry.md)
- Concept: [Boomi Companion](/concepts/boomi-companion.md)
