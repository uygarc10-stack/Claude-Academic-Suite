---
name: wildlife-ecology-knowledge
description: Shared wildlife ecology and conservation biology domain knowledge — terminology, common statistical and genetic analysis methods (KDE, MCP, RSF, STRUCTURE, ARLEQUIN, GENETIX), capture and GPS/GSM telemetry concepts, and how to explain technical terms to non-specialist audiences (ethics committees, funders, general readers). Use whenever a request involves wildlife field methods, movement/spatial ecology analysis, population genetics software, animal capture and immobilization protocols, GPS collar data, or camera trap/roadkill survey design — even if the user doesn't ask for an explanation directly, since correct handling of this terminology affects every other academic skill in this suite. Also use when the user needs a concept translated into plain language for a non-expert reader (e.g. an ethics committee form, a grant reviewer from outside the field, or a general-audience summary).
---

# Wildlife Ecology Knowledge

This is the shared foundation the rest of the suite draws on. `literature-review-expert`
and `scientific-writing-editor` both assume the terminology and methodological
context documented here rather than re-explaining it themselves — when either of
those skills hits a term or method covered in this skill's reference files,
treat this skill's guidance as authoritative and consistent across the whole
suite, so the same concept doesn't get explained two different ways in two
different documents.

This skill doesn't run a workflow of its own the way the others do. Its job is
to make sure technical concepts are used correctly and, when needed, explained
correctly — so pull in the relevant reference file, use it to get the details
right, and get back to whatever task (search, writing, review) triggered it.

## When to reach for the reference files

- **`references/methodology-glossary.md`** — spatial/movement ecology terms
  (home range, KDE, MCP, RSF), population genetics software and what each
  actually does (STRUCTURE, NEWHYBRIDS, ARLEQUIN, GENETIX), capture and
  chemical immobilization concepts, GPS/GSM telemetry terminology, and disease
  ecology / surveillance terms. Use this whenever a method or acronym shows up
  in a paper, a form, or a piece of writing and needs to be used correctly or
  defined.
- **`references/non-expert-explanations.md`** — how to translate a technical
  concept for a reader who isn't a specialist (an ethics committee member, a
  general grant reviewer, a journalist) without dumbing down the science or
  making it inaccurate. Use this for ethics committee applications (e.g.
  HADYEK forms), grant proposals reviewed by mixed panels, or public-facing
  summaries.

## Core principle: precision before simplification

When explaining a technical term to a non-expert, the instinct is often to
simplify until it's easy to read — but an oversimplified explanation that's
technically wrong is worse than a slightly denser one that's accurate. Always
get the definition right first, then work on making it readable. A good
parenthetical explanation preserves the technical meaning while giving a
reader outside the field enough to follow along, e.g.:

> "...GPS-GSM koliler (hayvanın konumunu uydu üzerinden belirleyip mobil şebeke
> ile aktaran takip cihazları) kullanılarak..."

rather than dropping the technical term altogether or defining it so loosely
that it becomes misleading.

## Staying current

Methodology and software in this field move — a genetics pipeline or spatial
analysis package can be superseded, deprecated, or get a newer standard
version. If a request seems to hinge on whether a specific tool, package
version, or method is still the current standard, don't rely solely on the
glossary here treat it as a starting point and verify against current
literature or documentation if the answer matters (e.g. recommending a
specific software version for an active project).

## Cross-skill consistency

If `scientific-writing-editor` or `literature-review-expert` needs to define
a term for a reader, or needs to correctly use a method name in prose, they
should match the definitions and framing in this skill's reference files
rather than improvising a new explanation each time. This keeps terminology
consistent across a literature review, a manuscript, and an ethics
application that might all be produced in the same project.
