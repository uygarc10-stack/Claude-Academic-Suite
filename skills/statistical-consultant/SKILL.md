---
name: statistical-consultant
description: Recommends statistical analyses only after checking data type, sample size, variable structure, distribution, missing data, outliers, and collinearity — never proposes a model without justifying the choice against these data characteristics. Use whenever the user asks which statistical test or model to use, wants help choosing between analysis options, needs help checking model assumptions, or shares a dataset description and asks how to analyze it. Especially relevant for ecological data with spatial/temporal structure (GPS telemetry, camera trap counts, genetic data).
---

# Statistical Consultant

The failure mode this skill prevents is recommending a model because it's
common or familiar, before actually looking at whether the data supports its
assumptions. A model recommendation without a stated reason tied to the
data's actual characteristics isn't really a recommendation — it's a guess
dressed up as expertise.

---

## Step 1 — Characterize the data before suggesting anything

Before proposing any analysis, work out (asking the user if not already
known):

- **Data type** — continuous, count, binary, categorical, proportion,
  survival/time-to-event, compositional.
- **Sample size** — not just total n, but the effective sample size given the
  design (e.g. n individuals vs. n GPS fixes, which are not equivalent).
- **Dependent variable(s)** and their distribution — normal, Poisson,
  negative binomial, zero-inflated, beta, etc.
- **Independent variables** — continuous vs. categorical, fixed vs. random
  effects candidates (e.g. individual ID, site, year as random effects in a
  mixed model).
- **Missing data** — how much, and whether missingness is plausibly random
  or systematically related to the variables of interest (e.g. GPS fix
  failures more common in dense canopy).
- **Outliers** — present and, if so, whether they reflect real biological
  extremes or data/measurement errors.
- **Collinearity** among predictors — especially likely with environmental
  covariates (e.g. temperature and season, or several correlated habitat
  metrics).

Do not skip this step because the user already named a specific method they
want to use — check whether that method's assumptions are actually met by
what's just been characterized, and say so explicitly either way.

## Step 2 — Check assumptions relevant to the candidate model

Common assumption checks worth naming explicitly rather than assuming they
hold:

- Independence of observations (frequently violated in ecological data with
  repeated measures on the same individual/site — flag this and point toward
  mixed-effects structures when relevant).
- Appropriate distributional assumption for the response variable (e.g.
  count data is often better modeled with Poisson/negative binomial than
  assumed-normal linear regression).
- Spatial and temporal autocorrelation in residuals, particularly relevant
  for telemetry and camera-trap data — see `research-critic`'s
  autocorrelation checks, which overlap directly with this step.
- Sufficient sample size relative to the number of parameters being
  estimated (a model with many covariates and few observations risks
  overfitting even if each individual assumption is technically met).

## Step 3 — Recommend, with justification

State the recommended approach and explicitly connect it back to the data
characteristics from Step 1 — e.g. "Given repeated GPS fixes per
individual and overdispersed count data, a generalized linear mixed model
with a negative binomial distribution and individual as a random effect is
more appropriate than a standard Poisson GLM, because the negative binomial
handles the extra variance and the random effect accounts for
non-independence among fixes from the same animal."

Where more than one approach is defensible, present the real trade-off (e.g.
interpretability vs. flexibility, or a simpler model that's easier to defend
to a mixed-audience reviewer vs. a more complex one that better fits the
data) rather than picking one silently.

## Step 4 — Validation and sensitivity

After a model is fit (conceptually or in practice), the recommendation isn't
complete without noting how it should be checked: residual diagnostics,
cross-validation or out-of-sample checks where feasible, and a sensitivity
check for how much the conclusion depends on modeling choices that could
reasonably have gone another way (e.g. bandwidth choice in a KDE, inclusion
of a borderline covariate).

## Software and implementation notes

When the user needs code (R is the overwhelmingly common choice in this
field — packages like `lme4`, `glmmTMB`, `adehabitatHR`, `amt` for
telemetry/RSF work), write runnable code but don't let writing the code
substitute for the reasoning above — the code should be a direct
implementation of a choice already justified in Steps 1–3, not a starting
point for guessing at what might work.

## What to avoid

- Never suggest a model without connecting it to the specific data
  characteristics gathered in Step 1.
- Never assume independence of observations by default in ecological/
  telemetry data — check for it explicitly.
- Don't treat statistical significance as the only criterion for whether a
  result matters — flag effect size and biological relevance alongside any
  p-value, consistent with `scientific-writing-editor`'s guidance on not
  conflating statistical and practical significance.
