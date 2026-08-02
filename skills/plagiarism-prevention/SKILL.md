---
name: plagiarism-prevention
description: Prevents plagiarism at the writing-process level — full conceptual rewriting instead of sentence-reordering, structural independence from source material, synthesis across multiple sources instead of paraphrasing one at a time, and flagging accidental self-plagiarism (reused text across a thesis, papers, or grant proposals). Use whenever text is being drafted from source material (papers, reports, a prior draft, another document) for a manuscript, thesis, proposal, or summary — even when citations are already correctly attached, since correct citation alone does not prevent plagiarism if the wording or structure too closely mirrors the source. Works alongside citation-integrity (in literature-review-expert), which governs whether citations are real, not whether the surrounding prose is independently written.
---

# Plagiarism Prevention

This skill is not about whether a citation is real — that's
`citation-integrity.md`'s job, inside `literature-review-expert`. This skill
is about something that can go wrong even when every citation is completely
correct: text that too closely mirrors a source's wording or structure,
which is still plagiarism regardless of whether it's properly attributed.

Correct attribution and independent expression are two separate
requirements. A paragraph can cite its source perfectly and still be
plagiarized if it was produced by lightly rewording the original rather than
by understanding it and expressing it independently.

---

## Core principle: paraphrase is not reordering

The single most common mistake in AI-assisted or human academic writing is
treating paraphrase as a word-substitution exercise — swapping a few words
for synonyms, or reordering clauses, while keeping the original sentence
structure and argument flow intact. This is not paraphrasing. It's
disguised copying, and plagiarism-detection software is generally good at
catching exactly this pattern.

Genuine paraphrase requires:

1. **Reading for meaning first.** Understand what the source is actually
   claiming and why, completely separate from its specific wording.
2. **Writing from that understanding, not from the source text.** Once the
   meaning is understood, write the sentence as if explaining the idea to
   someone else from memory — don't keep the source document open and
   rephrase it line by line.
3. **Changing the structure, not just the words.** If the source presents
   evidence then conclusion, and the rewrite presents evidence then
   conclusion in the same order with the same emphasis, that's still too
   close even if every word is different. Consider leading with the
   conclusion instead, or reorganizing around a different logical thread.

## Synthesize across sources rather than paraphrasing one at a time

The safest and most academically valuable way to avoid mirroring any single
source is to synthesize several sources into one statement, which is also
exactly what `evidence-synthesis.md` (in `literature-review-expert`) already
asks for. A sentence that integrates findings from three papers is
structurally very different from any one of them individually — it can't
closely mirror a single source because it isn't built from a single source.
When drafting from literature, default to this synthesis-first approach
rather than summarizing papers one by one and then citing each summary.

## Direct quotation: the deliberate exception

Occasionally, exact wording matters enough to justify a direct quotation —
a legal or regulatory definition, a precisely stated hypothesis, specific
survey/interview wording being analyzed. When that's the case:

- Mark it unambiguously as a quotation (quotation marks, block quote
  formatting) — never present quoted text as paraphrase or vice versa.
- Attach the source directly to the quotation, not just somewhere in the
  paragraph.
- Keep quotations short and used sparingly — see `citation-integrity.md`'s
  quotation discipline rules, which apply here identically.

Outside of these deliberate cases, default to full paraphrase.

## Self-check before finalizing text drawn from sources

Before treating a paragraph as done, check it against the source(s) it was
drawn from:

- Does any sentence share five or more consecutive words with the source
  (excluding necessary technical terms, species names, or short quoted
  phrases that are properly marked)?
- Does the paragraph's structure — the order ideas appear in, which idea is
  emphasized, the logical connectors used — closely track the source's
  structure, even though the wording differs?
- Could this paragraph have been produced without actually understanding the
  source's argument, just by following its shape? If yes, it likely needs a
  more substantial rewrite.

If any of these checks fail, rewrite from the underlying meaning again
rather than making surface edits to the existing draft.

## Watch for accidental self-plagiarism

Plagiarism isn't only about other people's text. Reusing substantial passages
of one's own previously published or submitted text — an introduction
paragraph reused across two grant proposals, a methods section copied
between a thesis chapter and a paper drawn from it — is treated as
self-plagiarism by most journals and funding bodies unless explicitly
disclosed and permitted. When drafting a new document that covers similar
ground to something the user has written before (visible earlier in this
conversation or provided as a reference document), flag this explicitly
rather than silently reusing the earlier phrasing, and default to writing it
fresh unless the user confirms reuse is acceptable for that specific venue.

## Every claim needs a traceable source

A claim presented as established fact should be traceable either to a source
retrieved in this session or to something the user has explicitly stated.
Don't let a claim drift from "the literature suggests" into an unqualified
statement of fact during the rewriting process — this is the same discipline
`citation-integrity.md` requires, extended to the paraphrasing process
itself: rewording a hedged claim into an unhedged one is a factual error, not
just a style choice, even when no citation is technically broken by doing it.
