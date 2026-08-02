---
name: grant-proposal-assistant
description: Drafts and reviews grant proposal sections (including TÜBİTAK and other bilateral/international research cooperation calls) by answering the questions a reviewer actually scores against — why it matters, why now, why this method, why this team, what the risks are, what the alternative plan is, what the expected output and impact are. Use whenever the user is writing or revising a grant proposal, project justification, or funding application section, or asks Claude to review a draft from a reviewer's perspective. Not for the ethics-committee/animal-welfare forms specifically — see wildlife-ecology-knowledge for the non-expert explanation approach those need.
---

# Grant Proposal Assistant

A grant proposal is scored by a reviewer against specific criteria, not read
the way a paper is read. The most common way a technically strong proposal
scores poorly is by describing the science well but never explicitly
answering the questions the reviewer is instructed to check for. This skill
exists to make sure those questions get answered directly, not left implicit.

---

## The core reviewer questions

Every major proposal section should, directly or indirectly, answer:

- **Why is this important?** — not just "this is an interesting question,"
  but why it matters to the field, to conservation practice, or to policy,
  stated concretely rather than generically.
- **Why now?** — what has changed (new method available, new gap identified,
  new collaboration possible, urgent conservation need) that makes this the
  right moment, as opposed to this being askable at any point in the past
  decade.
- **Why this method?** — justify the chosen approach against plausible
  alternatives, the way `statistical-consultant` justifies a model choice
  against the data — a method choice stated without justification reads as
  arbitrary to a reviewer.
- **Why this team?** — what expertise, prior work, access (field sites,
  permits, existing collaborations), or infrastructure makes this team
  positioned to actually deliver this project, stated with specifics rather
  than general claims of competence.
- **What is the risk?** — name the realistic ways the project could
  under-deliver (e.g. low capture rates, permit delays, collar failure
  rates) rather than presenting the plan as risk-free, which reviewers tend
  to read as a sign the risks weren't seriously considered.
- **What is the alternative plan?** — for each named risk, what's the
  contingency, stated concretely enough that a reviewer can see the project
  survives a setback rather than collapsing.
- **What is the expected output?** — concrete deliverables (papers, datasets,
  policy briefs, trained personnel, deposited genetic samples) rather than
  vague statements of contribution to knowledge.
- **What is the impact?** — who uses the output and how, distinguishing
  scientific impact (advances a specific gap) from broader impact
  (conservation policy, capacity building, international cooperation) where
  the call asks for both.

## Writing with the reviewer's eye

Draft or revise text as if scoring it against a rubric, not as if telling the
story of why the work is exciting. Concretely, this means:

- Front-load the answer to "why does this matter" rather than building up to
  it after several paragraphs of background.
- State the specific gap being filled, ideally traceable to an actual
  literature synthesis (`literature-review-expert`) rather than an assertion
  that a gap exists.
- Make risk and contingency sections genuinely informative rather than
  perfunctory — a one-line "risks are minimal" answers none of the reviewer's
  actual concern.
- Keep claims about team capability specific and verifiable (named prior
  projects, named infrastructure, named collaborators) rather than general
  self-description.

## International and bilateral cooperation specifics

For calls involving cross-border cooperation (e.g. a bilateral project with a
partner institution in another country), reviewers typically also want to see:

- a clear division of labor between the institutions/countries involved,
  stated specifically rather than as generic "collaboration,"
- how data, samples, or materials will move between countries where
  relevant (e.g. specimen transport, permit and regulatory considerations),
  and
- what each side specifically contributes that the other side couldn't
  provide alone — this is often what distinguishes a genuine bilateral
  project from a domestic project with an added international partner for
  the sake of eligibility.

## A caution on program-specific requirements

Funding call structures, required sections, page limits, and evaluation
criteria change between calls and over time — including for recurring
programs like TÜBİTAK's bilateral cooperation calls. Don't rely on memory of
a program's structure from a previous cycle as if it were guaranteed current;
check the current call text for the specific program and cycle being applied
to, and flag this explicitly if a specific structural requirement is being
assumed rather than confirmed.

## What to avoid

- Don't let enthusiasm for the science substitute for explicitly answering
  the reviewer's actual questions above.
- Don't present a project as risk-free — an honest risk section reads as
  more credible, not less.
- Don't claim broader impact in vague terms ("will benefit conservation")
  without naming who specifically benefits and how.
