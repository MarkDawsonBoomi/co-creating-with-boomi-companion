---
type: Scenario
title: Developer Build Walkthrough
description: A developer's end-to-end session with Boomi Companion — prompt, plan, generated process, canvas inspection of the map step, groovy scripting, and a test run.
tags: [scenario, boomi-companion, canvas, mapping, testing]
timestamp: 2026-07-01T00:00:00Z
source_video: boomi-companion-5.mp4
source_captions: ai-captions-1782134631451.vtt
related_module: /modules/02-conversational-and-canvas.md
---

# Setup

The developer has been hearing about [Boomi Companion](/concepts/boomi-companion.md) and wants to give it a try.

# The prompt

With Boomi Companion loaded, the developer puts in a prompt with a basic outline of what they will be working on, asking Companion to make a plan and check in with what the developer will need to provide.

# The clarifying questions

Boomi Companion asks a number of questions, and the developer is able to answer them fairly quickly. Once Companion has made some considerations, it also comes up with other things it might need. The developer is asked for the JSON input and XML output needed for the mapping. While collecting those, they notice some other pieces that will be important in this build and include them in their next prompt.

# The build

The prompt gets pasted in and Boomi Companion gets to work. The developer can see it plan as it is working, and all is looking good. Companion will need more information to build the integration outright, but the developer decides they want to see it as a test process first.

# Inspecting the canvas

They navigate to the integration canvas and open up the process Companion has created. They are most interested in how the mapping is being handled, so opening the map step on the canvas is where they go first.

Once inside the map, they can see that groovy script has been developed and incorporated into the mapping function. They take note of the *department to cost center* function as something that might be worth another look, and they check that the date is changed as requested.

# Testing

They then return to the canvas and decide to run a test from here.

Boomi Companion also runs its own tests, visible in the execution logs, but the developer wants to see it for themselves and check there. Once the test has been completed, they check the output to make certain that it is what was requested, and then check the input passed from the message step in this test was also correct.

All in all, it was a very impressive test.

# Wrap

As the developer thinks of things they're going to try next, the message to the learner is clear: you can get started on your own journey with Boomi Companion.

# Related

- Concept: [Boomi Companion](/concepts/boomi-companion.md)
- Concept: [Canvas Mode](/concepts/canvas-mode.md)
- Concept: [Conversational Mode](/concepts/conversational-mode.md)
- Module: [Conversational and Canvas](/modules/02-conversational-and-canvas.md)

# Citations

[1] Source captions: `scormcontent/assets/ai-captions-1782134631451.vtt` in the original SCORM package
