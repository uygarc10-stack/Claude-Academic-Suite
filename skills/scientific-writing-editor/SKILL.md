---
name: scientific-writing-editor
description: Edits and drafts scientific writing to match the register of top ecology and conservation journals (Nature Ecology & Evolution, Ecology Letters, Journal of Applied Ecology, Biological Conservation) — active voice, one idea per paragraph, restrained claims, minimal speculation in Discussion sections, no unnecessary adjectives. Use whenever the user asks to write, tighten, or edit a manuscript section, abstract, cover letter, or any academic prose destined for a journal, thesis, or grant proposal, or asks Claude to make writing sound more like a specific journal's style. Also use for general polishing of scientific paragraphs even outside a full manuscript context. Works together with literature-review-expert (which supplies the evidence) and citation-integrity (which the writing must never violate when citing sources).
---

# Scientific Writing Editor

This skill governs how scientific prose gets written or edited, independent of
whether a full literature review is in progress. A user asking to "tighten this
paragraph" or "make my abstract sound like Ecology Letters" should trigger this
skill directly, without needing to go through a literature search first.

Any citation that appears in text produced by this skill still has to satisfy
`citation-integrity.md` from the `literature-review-expert` skill — writing
quality is never a reason to relax that requirement. Terminology should stay
consistent with `wildlife-ecology-knowledge` when a technical term appears.

---

## Core writing principles

These apply regardless of target journal:

- **Keep scientific accuracy ahead of fluency.** A clean sentence that
  slightly overstates a finding is a worse outcome than a slightly denser one
  that's precisely correct. Never smooth out a hedge (e.g. "may be
  associated with") into a stronger claim (e.g. "causes") just because it
  reads better.
- **Prefer active voice.** "We tested whether..." over "It was tested
  whether..." Passive voice has a place in Methods sections where the actor
  is genuinely irrelevant, but shouldn't be the default throughout a
  manuscript.
- **Cut adjectives that aren't doing scientific work.** Words like
  "remarkable," "dramatic," "significant" (used loosely rather than
  statistically), "robust," or "compelling" often substitute for actually
  quantifying how large or reliable an effect is. Replace them with the
  actual number, effect size, or specific qualifier where possible.
- **One main idea per paragraph.** If a paragraph is doing two jobs (e.g.
  describing a method and also justifying why it was chosen), consider
  whether it should split, or at least make sure the topic sentence signals
  which idea is primary.
- **Don't let Results become Discussion.** Results should report what was
  found; interpretation, mechanism, and implications belong in Discussion.
  Watch for interpretive language creeping into a Results section ("this
  demonstrates that..." belongs later, not next to the numbers).
- **Restrain speculation in Discussion.** It's appropriate to propose
  mechanisms and implications, but each speculative claim should be flagged
  as such ("one possible explanation is...", "this may reflect...") rather
  than stated with the same confidence as a directly supported finding.
- **Don't overstate results.** A moderate effect described as "strong," a
  single-site study generalized as if it applied broadly, or a correlational
  finding framed causally are the most common ways manuscripts overstate
  their own findings — watch for all three specifically.

## Journal style calibration

Before editing toward a specific journal's voice, check
`references/journal-style-profiles.md` for the target journal's typical
register (some are more concise and mechanism-focused, others allow more
narrative framing) — don't apply a single generic "scientific style" and
call it journal-specific without checking what actually differs.

If the user hasn't specified a target journal, default to a register similar
to Journal of Applied Ecology / Biological Conservation (clear, applied,
moderately narrative) rather than the terser Ecology Letters house style,
since it's a safer default for a broader range of submission targets — but
ask if precision matters for that specific piece (e.g. the user is actually
about to submit somewhere specific).

## Section-specific guidance

- **Abstract** — every sentence should carry information a reader would use
  to decide whether to read further: the gap, the approach, the key result
  with a number or direction, and the implication. Avoid abstract sentences
  that only describe the paper's structure ("We discuss the implications of
  our findings") without stating what the findings actually were.
- **Introduction** — build the argument for why the study matters
  (broad context → specific gap → this study's contribution), not a
  loosely-connected literature summary. This should draw on
  `literature-review-expert`'s synthesis output rather than restating a
  list of prior studies.
- **Methods** — precise enough that the study could be replicated; passive
  voice is more acceptable here than elsewhere, but specificity (sample
  sizes, exact software/versions, parameter choices) still matters more than
  smooth prose.
- **Results** — report findings without interpreting them; use exact
  statistics, not vague magnitude words.
- **Discussion** — interpret findings, compare to existing literature
  (flagging agreement/disagreement per `evidence-synthesis.md`), state
  limitations honestly, and only then discuss broader implications. Avoid
  ending on inflated claims about significance to the field.

## Sentence-level rules and journal profiles

See `references/sentence-level-rules.md` for concrete before/after rewriting
examples covering hedging language, adjective removal, and active-voice
conversion, and `references/journal-style-profiles.md` for per-journal style
notes on the four journals named above.

## When editing existing text rather than drafting new text

State clearly which changes are stylistic (word choice, sentence structure)
versus substantive (changed a claim's strength, added a hedge, removed an
unsupported statement) — a substantive change to what's being claimed should
never happen silently as a side effect of a style pass. If tightening a
sentence would require softening or strengthening a claim, flag that
explicitly to the user rather than deciding unilaterally.
