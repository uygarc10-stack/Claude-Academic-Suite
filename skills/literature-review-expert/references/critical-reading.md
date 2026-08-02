# Critical Reading Engine

Finding papers is only the beginning of a literature review. The real task is
evaluating scientific evidence, not summarizing publications. Not every paper
deserves equal trust, and treating them as if they do is how weak or biased
findings quietly end up shaping a review's conclusions.

Every publication that will actually influence the write-up should go through
structured critical appraisal before its findings are allowed to affect the
synthesis.

---

## Reading philosophy

Read as a reviewer, not as a student. A student's question is "what do the
authors claim?" A reviewer's questions are:

- Are the claims actually supported by the data presented?
- How strong is the evidence, really?
- What limitations exist, and how much do they matter?
- How transferable are the findings beyond this specific study?
- How does this study fit into the broader body of evidence?

## Structured paper analysis

For every important publication, work through the following, to whatever
extent the paper makes it possible:

**Bibliographic information** — authors, year, journal, DOI, PMID (if
applicable), country, institution. (This also feeds directly into the
citation-integrity check — see `citation-integrity.md`.)

**Research context** — the scientific question, objectives, hypotheses,
motivation, the knowledge gap the study claims to address, and why the study
was conducted in the first place.

**Study design** — experimental, observational, review, meta-analysis,
simulation, monitoring-based (camera trap, telemetry, genetic, disease
surveillance), laboratory, field, or mixed methods.

**Biological context** — species, taxonomic group, population, habitat,
geographic region, study period, sample size, spatial scale, temporal scale.

**Methodological assessment** — sampling strategy and effort, whether
detection probability was considered, replication, randomization, controls,
covariates, the statistical framework and software used, model assumptions,
validation approach, sensitivity analysis, uncertainty estimation.

**Statistical assessment** — response and predictor variables, effect sizes,
confidence or credible intervals, p-values where appropriate, information
criteria, model comparison, cross-validation, out-of-sample validation,
uncertainty estimation. Always distinguish statistical significance from
biological or practical importance — a significant effect can be trivially
small, and a non-significant one can still be biologically meaningful in an
underpowered study.

## Risk of bias

Actively look for, and be ready to name, sources of bias: selection bias,
sampling bias, spatial bias, temporal bias, publication bias, detection bias,
observer bias, measurement bias, reporting bias, confirmation bias, collider
bias, confounding, pseudoreplication, missing data, survivorship bias. Don't
just note that a bias "could exist" in the abstract — explain concretely how
it would push the paper's conclusions in a particular direction, if it does.

## Internal validity

Check whether the conclusions actually follow from the data presented. Watch
for: unsupported conclusions, overgeneralization beyond what the data show,
causal claims without evidence, correlation quietly reinterpreted as
causation, insufficient replication, weak controls, weak sampling designs,
overfitting, and underpowered analyses presented with unwarranted confidence.

## External validity

Assess whether the findings can reasonably generalize beyond the exact
conditions of the study: species, ecosystem, geographic region, sampling
design, study duration, level of human disturbance, climate, management
regime. Never assume a finding transfers automatically to a different
ecological system just because the underlying mechanism sounds general —
say explicitly when transferability is uncertain.

## Strength of evidence

For every major finding that will be used in the synthesis, form a view on
confidence — very high, high, moderate, low, or very low — and be prepared to
justify it. Confidence should track methodological quality (design, sample
size, replication, robustness of analysis), not journal prestige or how
confidently the paper's own abstract states its conclusions.

## Relationship to existing literature

For each paper, work out whether it: supports previous findings, contradicts
previous findings, extends previous work, introduces a new method, fills an
existing gap, opens a new question, or shifts current understanding. Never
evaluate a paper in isolation from the rest of what's been found — its value
is partly relational.

## Relevance to the user's actual question

Rate applicability as direct, partial, limited, or not applicable, and say
why. Consider species match, geographic similarity, methodological overlap,
ecological context, analytical framework, and whether the study's management
or research objectives resemble the user's.

## When a paper counts as "read"

Treat a paper as genuinely reviewed only once you understand its objectives,
have evaluated its methods, identified its limitations, assessed its evidence
strength, placed it relative to the literature, and worked out its relevance
to the user's question. Only then should its findings be allowed to feed into
the evidence synthesis stage (`evidence-synthesis.md`). A paper you've only
skimmed for its abstract hasn't cleared this bar — say so rather than citing
it as if it had.
