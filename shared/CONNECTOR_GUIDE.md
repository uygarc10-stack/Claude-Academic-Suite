# Connector Guide

## Purpose

This document defines how Claude Academic Suite prioritizes and uses connected external knowledge sources.

The objective is to maximize scientific accuracy while minimizing hallucinations, citation errors, and incomplete literature retrieval.

---

# General Principles

Scientific databases always take priority over general web search.

Never stop searching because one source produced relevant results.

Search multiple independent sources whenever the task requires comprehensive evidence synthesis.

Prefer peer-reviewed literature over preprints whenever both are available.

Use preprints primarily for identifying the newest developments.

General web search is supplementary, not primary.

---

# Priority Order

Tier 1

- Consensus
- PubMed
- Scholar Gateway

Tier 2

- CrossRef
- OpenAlex
- Web of Science
- Scopus

Tier 3

- bioRxiv
- medRxiv
- arXiv

Tier 4

- web_search
- web_fetch

---

# Evidence Saturation

Continue searching until additional searches provide little or no new information.

Do not terminate a search because a fixed number of papers has been found.

The stopping criterion is evidence saturation, not search count.

---

# Cross Validation

Whenever possible, verify important claims using more than one independent source.

Conflicting evidence should be investigated rather than ignored.

---

# Connector Roles

Consensus:
Primary evidence synthesis and rapid literature discovery.

PubMed:
Biomedical, veterinary, disease ecology, zoonoses, epidemiology.

Scholar Gateway:
Citation-level verification and source retrieval.

bioRxiv:
Recent but non-peer-reviewed research.

web_search:
Supplementary discovery.

web_fetch:
Retrieve full documents or additional context when necessary.
