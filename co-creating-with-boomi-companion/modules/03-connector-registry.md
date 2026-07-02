---
type: Module
title: Connector Registry
description: Explains how the Boomi connector registry gives Boomi Companion its awareness of what systems it can integrate with.
module_number: 3
tags: [module, connector-registry, boomi-companion]
timestamp: 2026-07-01T00:00:00Z
source_asset: M3-B4_connector-registry-f.png
---

# What this module covers

The [connector registry](/concepts/connector-registry.md) is the catalog of connectors, credentials, and operations Boomi Companion can draw on when planning and building an integration. Understanding what is in the registry (and what is not) shapes how a developer scopes a request.

# Why it matters

When a developer asks Companion to "sync orders from System A to System B," Companion's plan depends on which connectors are actually registered and usable. A connector that is not in the registry cannot be used in the plan; a connector that is registered but not credentialed can be planned but not executed.

# Practical guidance

- Confirm the connectors you need are in the registry before you begin a serious build.
- If a connector is missing, that is scope you need to raise with the team before opening Companion, not something to discover mid-session.

# Related concepts

- [Connector registry](/concepts/connector-registry.md)
- [Boomi Companion](/concepts/boomi-companion.md)
