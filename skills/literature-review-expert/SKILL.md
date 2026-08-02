---
name: literature-review-expert
description: Systematic literature review workflow for wildlife ecology and conservation research — designing search strategies, critically appraising study methodology and bias, synthesizing evidence across multiple studies, and verifying citation integrity. Use whenever the user asks for a literature review, a background/related-work section, an evidence synthesis on an ecological or biological research topic, or asks Claude to find, read, and evaluate scientific papers on a topic. Also use when drafting the literature-review portion of a manuscript, grant proposal (e.g. TÜBİTAK), or thesis chapter, or when the user asks Claude to check whether a citation, DOI, or quoted finding is real. Not needed for a single quick factual question that doesn't require searching or comparing multiple sources.
---

# Literature Review Expert

This skill turns literature review from "find some papers and summarize them" into
the process an experienced researcher actually follows: plan the search, read every
paper as a reviewer rather than a student, weigh and synthesize the evidence as a
whole, and never let an unverifiable claim or citation into the final text.

Four engines make up the workflow. Each one is a separate reference file so this
file stays short — read the relevant one in full when you reach that stage. Don't
skip a stage because the user's request sounds simple; a request that looks like
"give me a quick lit review on X" still benefits from the full pipeline, just
scaled down in depth.

## Why this exists

The most common failure modes in AI-assisted literature review are:

1. Searching with the user's raw sentence instead of a designed strategy, which
   under-covers the actual evidence base.
2. Treating every paper as equally trustworthy and summarizing them one by one
   instead of weighing evidence and synthesizing across studies.
3. Producing a "collection of summaries" (Author A found X. Author B found Y.)
   instead of an integrated scientific narrative.
4. Fabricating or subtly corrupting citations — wrong DOI, invented page numbers,
   a claim attributed to the wrong paper — which is the single fastest way to
   destroy a researcher's credibility.

Each reference file below exists to close one of these gaps.

## Workflow map

```
Research question
      │
      ▼
[1] SEARCH ORCHESTRATION  → references/search-orchestration.md
      │  design the strategy, decompose the question, pick real tools,
      │  search until evidence saturation, not until "enough papers"
      ▼
[2] CRITICAL READING       → references/critical-reading.md
      │  read every important paper as a reviewer: design, bias,
      │  internal/external validity, strength of evidence
      ▼
[3] EVIDENCE SYNTHESIS     → references/evidence-synthesis.md
      │  integrate across studies thematically, find consensus,
      │  explain disagreement, identify real knowledge gaps
      ▼
[4] CITATION INTEGRITY     → references/citation-integrity.md
         verify every citation traces to a real retrieved source
         before it appears in the final text — this stage runs
         continuously, not just at the end
```

Stage 4 is not really "last" — treat it as a standing constraint that applies
every time a citation, DOI, or quotation is about to be written, from the first
search onward. Stages 1–3 are more sequential but can loop back (e.g. synthesis
in stage 3 often reveals a gap that sends you back to stage 1 for a fresh search).

## Read this first, every time

Before doing anything else for a literature-review task:

1. Open `references/search-orchestration.md` and follow it to build the search
   plan. Do not run a search before this.
2. As papers come back, apply `references/critical-reading.md` to every paper
   that will actually influence the write-up (not necessarily every paper the
   search surfaces — triage first, then read closely what matters).
3. Once enough papers have been read, apply `references/evidence-synthesis.md`
   to integrate them into a coherent narrative.
4. Apply `references/citation-integrity.md` continuously — check it again
   before finalizing any section that contains a citation, DOI, or quotation.

## Tool reality check

Be honest with yourself and the user about what is actually available in this
session. Do not imply access to a database that isn't connected.

- **Directly queryable via connected tools (if present in this session):**
  Consensus, PubMed, bioRxiv, Scholar Gateway. These return real structured
  results and are the most reliable source of verifiable bibliographic detail.
- **Reachable only through general web search/fetch:** Web of Science, Scopus,
  CrossRef, OpenAlex, Google Scholar, journal websites. Treat results from these
  as needing the same verification rigor as any other web source — a search
  snippet mentioning a paper is not the same as having queried the database's
  own index.
- If a database the user expects (e.g. Web of Science) isn't actually
  connected, say so plainly rather than quietly substituting a web search and
  presenting it as equivalent coverage.

## Calibrating depth to the request

Not every request needs the full systematic-review treatment. Use judgment:

- A quick "what does the literature say about X" question: run a focused search
  (stage 1, lightweight), read the handful of papers that come back with the
  critical-reading lens (stage 2), give a short synthesized answer (stage 3),
  verify what you cite (stage 4). Don't pad it into an artificial systematic
  review.
- A literature review section for a manuscript, thesis, or grant proposal:
  run the full pipeline, iterate stage 1 until evidence saturation, and write
  the result as connected scientific prose per the synthesis engine's guidance.
- A request to check a specific citation or quote: go straight to
  `references/citation-integrity.md`.

## Scope note

This skill is written with wildlife ecology and conservation biology in mind
(population ecology, movement ecology, disease ecology, human-wildlife
conflict, conservation genetics), since that's the primary use case it was
built for. The underlying logic — search design, critical appraisal, evidence
synthesis, citation integrity — is domain-general and applies to any empirical
research topic; only some of the illustrative examples in the reference files
are ecology-specific.
