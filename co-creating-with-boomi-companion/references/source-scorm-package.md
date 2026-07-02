---
type: Reference
title: Source SCORM Package
description: Provenance for the SCORM 1.2 package that this OKF bundle was converted from.
resource: co-creating-with-boomi-companion-scorm12-ur6fODAf
tags: [provenance, scorm, articulate-rise]
timestamp: 2026-07-01T00:00:00Z
---

# Package identity

- **Course title**: Co-Creating with Boomi Companion
- **SCORM version**: 1.2
- **Authoring tool**: Articulate Rise
- **Manifest identifier**: `zKpYwp69qrVzq47LGW4amcij4rde4x3Eur6fODAf`
- **Default organization**: `articulate_rise`
- **Launch page**: `scormdriver/indexAPI.html`

# Manifest structure

The SCORM manifest (`imsmanifest.xml`) declared a single organization with one SCO item ("Co-Creating with Boomi Companion"), referencing a single web content resource with the standard Rise runtime bundle:

- `scormdriver/` - SCORM runtime shim, bookmarking, and LMS communication
- `scormcontent/index.html` - Rise front-end bootstrapper
- `scormcontent/lib/rise/` - Rise front-end assets
- `scormcontent/lib/learn_dist/` - Rise learn distribution
- `scormcontent/lib/mondrian/` - Rise UI framework
- `scormcontent/assets/` - course-authored images, videos, audio, and captions

# Mapping between source and OKF concepts

| Source asset | OKF concept |
|--------------|-------------|
| `01_skill_folders.png` | [Skill Folders](/concepts/skill-folders.md) |
| `03_github.png` | Referenced in [Introduction](/modules/01-introduction.md) |
| `Conversational.BC.png` | [Conversational Mode](/concepts/conversational-mode.md) |
| `Canvas.BC.png` | [Canvas Mode](/concepts/canvas-mode.md) |
| `Conversational and Can.png` | [Conversational and Canvas](/modules/02-conversational-and-canvas.md) |
| `M3-B4_connector-registry-f.png` | [Connector Registry](/concepts/connector-registry.md) and [Module 3](/modules/03-connector-registry.md) |
| `4_planning_together.png` | [Planning Together](/modules/04-planning-together.md) |
| `5_stopping.png` | [Stopping](/modules/05-stopping.md) |
| `Habitsforstayingcurrent..png` | [Habits for Staying Current](/modules/06-habits-for-staying-current.md) |
| `boomi-companion-5.mp4` + `ai-captions-1782134631451.vtt` | [Developer Build Walkthrough](/scenarios/developer-build-walkthrough.md) |
| `Collaborating a Build-.mp4` + `ai-captions-1782154409521.vtt` | [Stakeholder Request Scoping](/scenarios/stakeholder-request-scoping.md) |
| `Boomi Companion - Ca.mp4` + `ai-captions-1782157398708.vtt` | [Reflection Checkpoint](/scenarios/reflection-checkpoint.md) |
| `Flipcard 1.png` through `Flipcard 5_1.png` | Summary flip-card review, embedded in module bodies where relevant |
| `Course end_no eval.svg` | Course wrap, referenced in [course.md](/course.md) |
| `Boomi Copyright 2025pt.svg` | Boomi copyright graphic — attribution, not knowledge content |

# Conversion notes

- Text narrative for the three embedded videos was extracted from the VTT caption files bundled with the SCORM package. The bulk of Rise course text is compressed inside `scormcontent/index.html` as an LZW-encoded blob; the OKF authoring here relies on the caption files, asset filenames, and manifest structure rather than decoding that blob byte-for-byte.
- Where the caption transcripts contain minor auto-caption artifacts (e.g., "Boomie Companion", "boomy companion"), the OKF concepts use the canonical spelling *Boomi Companion*.

# Original media

The original SCORM package should be retained alongside this bundle for anyone who wants to re-play the course inside an LMS. This bundle is the *knowledge* of the course; the SCORM package is the *experience*.
