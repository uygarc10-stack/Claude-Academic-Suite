---
name: research-idea-generator
description: Generates publishable research ideas and testable hypotheses from identified literature gaps — checks each idea for scientific importance, feasibility (data, permits, time), and journal fit before proposing it. Use when the user asks for research ideas, project directions, hypotheses to test, or "what should I study next," especially in wildlife ecology and conservation. Not for general brainstorming unrelated to a research program — this is specifically about ideas that could become a fundable, publishable study.
---

# Research Idea Generator

The goal here is a publishable idea, not just an interesting one. Plenty of
questions are interesting but untestable, already answered, or impossible to
resource — the job of this skill is to filter those out before they're
proposed, not to generate the largest possible list of things that sound
novel.

If `literature-review-expert` has already run in this conversation and
surfaced knowledge gaps (via `evidence-synthesis.md`'s gap analysis), start
from those gaps rather than inventing new ones from scratch — a gap that's
already been evidence-checked against the literature is a stronger starting
point than a fresh guess. If no literature review has been done yet, say so
and offer to run one first, since an idea generated without checking the
literature risks proposing something already answered.

---

## Step 1 — Confirm the gap is real

Before building on a knowledge gap, ask:

- Is this actually a gap, or just an area with less-searched literature?
- Has it been addressed by a study using a different term or approach that a
  narrow search might have missed?

If unsure, this is worth a quick additional search rather than assuming the
gap is real because it wasn't mentioned in the papers already reviewed.

## Step 2 — Test whether the gap matters

A gap being unaddressed isn't enough by itself. Check:

- Would filling this gap change scientific understanding, management practice,
  or policy in a meaningful way?
- Is it a gap because no one has asked the question, or because the question
  turned out not to be very informative?

Be willing to say a gap isn't worth pursuing if it doesn't clear this bar,
even if it's technically novel.

## Step 3 — Check feasibility honestly

For each candidate idea, work through:

- Can the necessary data actually be collected, given realistic constraints
  (field access, permits, ethics approval, funding, time)?
- Does it require capture, collaring, genetic sampling, or other logistically
  heavy methods, and is that proportionate to the question?
- Is the timeline compatible with the funding mechanism or degree timeline in
  question (e.g. a TÜBİTAK project cycle, a PhD chapter deadline)?
- Could the result plausibly be publishable regardless of which way the data
  comes out (a design that only "works" if the hypothesis is confirmed is a
  weak design)?

An idea that fails feasibility should be flagged as such rather than
presented as equally viable to one that's clearly resourceable.

## Step 4 — Formulate a testable hypothesis

Turn the idea into a hypothesis that is specific, falsifiable, and tied to
measurable variables — not a vague direction of interest. Compare:

**Too vague:** "Investigate how urbanization affects jackal ecology."
**Testable:** "Jackal home range size increases with distance from urban
edge, mediated by prey availability, as measured via GPS telemetry and camera
trap indices across a rural-urban gradient."

State what result would support the hypothesis and what result would refute
it — if neither is clear, the hypothesis isn't specific enough yet.

## Step 5 — Match to realistic outlets

Suggest which journals or venues would plausibly fit the resulting study,
based on scope and scale (a single-population field study fits differently
than a multi-region synthesis) — see `scientific-writing-editor`'s journal
profiles for the register each venue expects, which also hints at what scale
and framing of study each one tends to publish.

## What to avoid

- Don't just repeat what the existing literature already found dressed up as
  new — check this explicitly against the literature-review-expert synthesis
  if one exists.
- Don't generate ideas divorced from what's actually feasible for this
  specific researcher's context (available field sites, permits, current
  collaborations) — ask about constraints if they're not already known
  rather than proposing something that assumes unlimited resources.
- Don't present every generated idea as equally strong. Rank them, and say
  plainly which one you'd pursue first and why.
