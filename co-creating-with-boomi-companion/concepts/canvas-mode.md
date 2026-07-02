---
type: Interaction Mode
title: Canvas Mode
description: Working with Boomi Companion directly on the integration canvas — inspecting steps, opening maps, and running tests.
tags: [boomi-companion, interaction-mode, canvas, testing]
timestamp: 2026-07-01T00:00:00Z
source_asset: Canvas.BC.png
---

# What it is

Canvas mode is the direct-manipulation surface of the Boomi platform. Developers use it to inspect what [Boomi Companion](/concepts/boomi-companion.md) has built, edit steps, and run tests.

# Typical canvas workflow

1. Companion produces a plan and, when the developer is ready, builds a test process.
2. The developer navigates to the integration canvas and opens the process Companion created.
3. The developer opens the map step to see how mapping is handled. If Companion incorporated groovy script, it is visible inside the mapping function.
4. The developer sanity-checks specific transformations. In the walkthrough, this includes a *department to cost center* mapping function and a date transformation.
5. The developer returns to the canvas and runs a test from there.
6. The developer inspects both the message step input and the final output to confirm the run matches the request.

# Why go to the canvas at all

Companion runs its own tests, and the results are visible in the execution logs. Developers should still run tests themselves from the canvas because:

- Reading the canvas is how you *see* what was built, not just what was reported.
- Running the test yourself confirms the message step input and the final output separately.

# Related

- [Conversational Mode](/concepts/conversational-mode.md)
- Scenario: [developer build walkthrough](/scenarios/developer-build-walkthrough.md)
- Module: [Conversational and Canvas](/modules/02-conversational-and-canvas.md)
