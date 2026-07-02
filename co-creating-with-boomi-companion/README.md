---
type: Bundle README
title: Co-Creating with Boomi Companion — OKF Bundle
description: Repository readme for the OKF bundle representation of the Boomi L&D course Co-Creating with Boomi Companion.
tags: [readme, okf, boomi-companion]
timestamp: 2026-07-01T00:00:00Z
---

# Co-Creating with Boomi Companion — OKF Bundle

An [Open Knowledge Format (OKF)](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md) v0.1 bundle representing the Boomi L&D course *Co-Creating with Boomi Companion*, converted from a SCORM 1.2 (Articulate Rise) package.

## What is this

OKF is a specification from Google Cloud for representing knowledge as a directory of markdown files with YAML frontmatter. It is designed to be readable by humans without tooling, parseable by agents without SDKs, and diffable in version control. This bundle re-represents the course's concepts, scenarios, and modules as agent- and human-readable markdown so the content can live outside an LMS.

## Bundle contents

```
co-creating-with-boomi-companion/
├── index.md                                # OKF root, declares okf_version 0.1
├── log.md                                  # bundle change history
├── course.md                               # top-level course concept
├── modules/
│   ├── index.md
│   ├── 01-introduction.md
│   ├── 02-conversational-and-canvas.md
│   ├── 03-connector-registry.md
│   ├── 04-planning-together.md
│   ├── 05-stopping.md
│   └── 06-habits-for-staying-current.md
├── concepts/
│   ├── index.md
│   ├── boomi-companion.md
│   ├── conversational-mode.md
│   ├── canvas-mode.md
│   ├── skill-folders.md
│   └── connector-registry.md
├── scenarios/
│   ├── index.md
│   ├── stakeholder-request-scoping.md
│   ├── developer-build-walkthrough.md
│   └── reflection-checkpoint.md
└── references/
    ├── index.md
    └── source-scorm-package.md
```

Sixteen concept files plus six reserved index/log files. All concepts declare a `type` and cross-link with bundle-relative paths.

## Conformance

Validated against OKF v0.1 §9 with the spec's reference validator. No hard failures. Fifteen soft warnings, all `recommended-field-missing: resource`, which is expected since these are abstract course concepts (modules, scenarios, product concepts) with no single canonical URI.

## Provenance

Converted from the SCORM 1.2 package `co-creating-with-boomi-companion-scorm12-ur6fODAf` (Articulate Rise export). See [references/source-scorm-package.md](references/source-scorm-package.md) for the full mapping between original SCORM assets and OKF concepts.

Narrative content for the three embedded video segments was extracted from the VTT caption files bundled with the SCORM package. The remaining Rise course text is compressed as an LZW blob inside `scormcontent/index.html`; the conversion here relies on captions, asset filenames, and manifest structure rather than decoding the compressed content byte for byte. If a fuller extraction is needed later, the SCORM package itself should be retained as the source of truth.

## How to use

Clone the repo and read the markdown directly. If you're consuming this programmatically, the OKF spec appendix has a ~30-line Python parser that will walk the bundle and build a link graph.

```python
import pathlib, re, yaml

def load_bundle(root):
    concepts, links = {}, []
    for path in pathlib.Path(root).rglob("*.md"):
        text = path.read_text(encoding="utf-8")
        meta, body = {}, text
        if text.startswith("---"):
            try:
                _, fm, body = text.split("---", 2)
                meta = yaml.safe_load(fm) or {}
            except ValueError:
                pass
        concept_id = str(path.relative_to(root)).removesuffix(".md")
        concepts[concept_id] = {"meta": meta, "body": body, "path": str(path)}
        for target in set(re.findall(r"\]\((/[^)]+\.md)\)", body)):
            links.append((concept_id, target.removeprefix("/").removesuffix(".md")))
    return concepts, links
```

## Uploading to GitHub

1. Unzip this bundle into an empty repository directory.
2. `git init && git add . && git commit -m "Initial OKF bu