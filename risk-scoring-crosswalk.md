# Risk Scoring Crosswalk
> OHS and GRC risk scoring are the same underlying logic with different
> variables — and OHS got one of those variables right that GRC is
> still missing.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [The Fine-Kinney Method](#the-fine-kinney-method)
- [NIST 800-30 Risk Scoring](#nist-800-30-risk-scoring)
- [The Complete Mapping](#the-complete-mapping)
- [The Exposure Gap](#the-exposure-gap)
- [Risk Scoring Governance](#risk-scoring-governance)
- [Implications for GRC Practice](#implications-for-grc-practice)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

Risk scoring is how a risk assessment moves from qualitative
observation to defensible, prioritized decision-making. Without
a scoring model, findings are opinions. With one, they are evidence.

This document maps the Fine-Kinney risk scoring method — used across
a decade of OHS practice on factory floors, oil rigs, and marine
environments — onto NIST 800-30's risk scoring methodology. It shows
where the two models align, where they diverge, and where Fine-Kinney
captures a variable that NIST 800-30 systematically underweights:
**Exposure** — how frequently assets or people come into contact
with a threat source.

The argument: GRC risk scoring would be more accurate if it adopted
a three-variable model that explicitly separates Exposure from
Likelihood — because frequency of contact changes the risk profile
in ways a two-variable model consistently misses.

---

## The Fine-Kinney Method

**Fine-Kinney is a quantitative risk scoring model that calculates
risk as the product of three variables: Likelihood, Exposure, and
Consequence.**

> **Risk = Likelihood × Exposure × Consequence**

### The Three Variables

**Likelihood** — the probability that a hazard event will occur
if exposure happens.

| Score | Description |
|-------|-------------|
| 0.5 | Practically impossible |
| 1 | Conceivable but unlikely |
| 3 | Unusual but possible |
| 6 | Quite possible |
| 10 | To be expected |

**Exposure** — how frequently people or assets come into contact
with the hazard.

| Score | Description |
|-------|-------------|
| 0.5 | Very rarely — once a year or less |
| 1 | Rarely — monthly |
| 2 | Occasionally — weekly |
| 3 | Occasionally — several times a week |
| 6 | Frequently — daily |
| 10 | Continuously — many times per day |

**Consequence** — the severity of harm if the hazard event occurs.

| Score | Description |
|-------|-------------|
| 1 | Minor injury — first aid only |
| 3 | Significant injury — medical treatment required |
| 7 | Serious injury — hospitalization |
| 15 | One fatality |
| 40 | Multiple fatalities |
| 100 | Catastrophic — mass casualties |

### Risk Score Interpretation

| Score | Risk Level | Action Required |
|-------|-----------|----------------|
| < 20 | Acceptable | Monitor |
| 20–70 | Low | Attention needed |
| 70–200 | Substantial | Corrective action required |
| 200–400 | High | Immediate improvement needed |
| > 400 | Very High | Stop activity — remediate immediately |

### Why Fine-Kinney Works

**Three variables capture risk more accurately than two because
frequency of contact is an independent risk multiplier.**

A hazard with high consequence that workers encounter once a year
is categorically different from a hazard with the same consequence
that workers encounter twenty times a day. Fine-Kinney makes that
difference explicit and quantifiable. A two-variable model collapses
it into likelihood — losing precision in the process.

---

## NIST 800-30 Risk Scoring

**NIST 800-30 calculates risk as the product of two variables:
Likelihood and Impact.**

> **Risk = Likelihood × Impact**

### The Two Variables

**Likelihood** — the probability that a threat event will occur,
given the threat source characteristics, vulnerability severity,
existing controls, and historical data.

| Level | Description |
|-------|-------------|
| Very Low | Threat source lacks capability or motivation |
| Low | Threat source has limited capability or motivation |
| Moderate | Threat source has some capability and motivation |
| High | Threat source is capable and motivated |
| Very High | Threat source is highly capable and highly motivated |

**Impact** — the harm to the organization if the threat event occurs,
assessed across four dimensions:

| Dimension | Examples |
|-----------|---------|
| Confidentiality | Unauthorized disclosure of sensitive data |
| Integrity | Unauthorized modification of data or systems |
| Availability | Disruption of access to systems or data |
| Organizational | Financial loss, regulatory penalty, reputational damage |

| Level | Description |
|-------|-------------|
| Very Low | Negligible effect on operations or assets |
| Low | Minor degradation — mission still performable |
| Moderate | Significant degradation — reduced effectiveness |
| High | Significant damage to assets or mission capability |
| Very High | Severe or catastrophic damage |

### Risk Score Matrix

| | Very Low Impact | Low Impact | Moderate Impact | High Impact | Very High Impact |
|-|----------------|-----------|----------------|-------------|-----------------|
| **Very High Likelihood** | Low | Moderate | High | Very High | Very High |
| **High Likelihood** | Low | Moderate | High | High | Very High |
| **Moderate Likelihood** | Low | Low | Moderate | High | High |
| **Low Likelihood** | Very Low | Low | Low | Moderate | High |
| **Very Low Likelihood** | Very Low | Very Low | Low | Low | Moderate |

---

## The Complete Mapping

**Fine-Kinney and NIST 800-30 are solving the same problem with
different levels of precision.**

| Fine-Kinney | NIST 800-30 | Notes |
|-------------|-------------|-------|
| Likelihood (0.5–10) | Likelihood (Very Low–Very High) | Direct equivalent — probability of harm occurring |
| Consequence (1–100) | Impact (Very Low–Very High) | Direct equivalent — severity if harm occurs |
| Exposure (0.5–10) | **Not explicitly modeled** | **The gap — see below** |
| Quantitative score | Qualitative matrix | Different output format, same underlying logic |
| Stop activity > 400 | Very High risk — immediate action | Equivalent escalation threshold |
| Corrective action required | Risk treatment required | Equivalent remediation trigger |

### Where They Align

Both models:
- Assess probability of harm occurring
- Assess severity of harm if it occurs
- Produce a risk level that drives prioritization
- Escalate the highest scores to immediate action
- Treat lower scores as monitor or accept

### Where They Diverge

**Fine-Kinney separates Exposure from Likelihood. NIST collapses
them together.**

This is not a minor difference. It is a precision gap that
systematically underscores risks involving frequent asset-threat
contact — which in modern GRC environments includes almost every
internet-facing system, every shared credential, and every
high-volume data processing workflow.

---

## The Exposure Gap

**NIST 800-30's two-variable model systematically underscores
risks that involve frequent contact between assets and threat
sources.**

### The Problem in Plain Language

Imagine two systems with identical vulnerabilities and identical
impact if exploited:

| | System A | System B |
|-|----------|----------|
| **Vulnerability** | Weak authentication | Weak authentication |
| **Impact if exploited** | High | High |
| **Likelihood of exploit if attempted** | High | High |
| **Exposure** | Accessed by 2 admins, monthly | Accessed by 500 employees, daily |
| **NIST 800-30 score** | High | High |
| **Fine-Kinney score** | Substantial | Very High |

NIST 800-30 scores these identically. Fine-Kinney scores System B
dramatically higher — because 500 people accessing a vulnerable
system daily creates exponentially more opportunities for the
vulnerability to be exploited than 2 people accessing it monthly.

### Where Exposure Matters Most in GRC

| High exposure scenario | Why it matters |
|-----------------------|---------------|
| Internet-facing login portals | Thousands of authentication attempts daily |
| Shared credentials across teams | Every user is a potential exploit vector |
| High-volume APIs | Millions of calls create millions of exploit opportunities |
| Widely distributed sensitive data | More people with access = more exposure surface |
| Remote workforce on unmanaged devices | Daily exposure to uncontrolled environments |

### The Proposed Addition

**GRC risk scoring should explicitly model Exposure as an
independent variable — separate from Likelihood — using a scale
calibrated to digital asset contact frequency.**

A proposed GRC Exposure scale:

| Score | Description |
|-------|-------------|
| 1 | Very low — asset accessed rarely, limited users |
| 2 | Low — asset accessed occasionally, small user group |
| 3 | Moderate — asset accessed regularly, defined user group |
| 6 | High — asset accessed frequently, large user group |
| 10 | Very high — asset internet-facing or accessed continuously |

**Adjusted GRC formula:**

> **Risk = Likelihood × Exposure × Impact**

This produces a more precise risk score that reflects not just
whether a vulnerability could be exploited, but how many
opportunities exist for it to be exploited in practice.

---

## Risk Scoring Governance

**A risk score is only as defensible as the process that produced it.**

### The Consensus Process

In OHS practice, disputed risk scores were resolved through a
structured consensus process:

1. Two assessors score independently
2. If scores diverge significantly, a third assessor is called in
3. All assessors walk through the scenario together
4. Consensus is sought through structured discussion
5. If consensus isn't reached, the senior assessor makes the final
   call — defaulting to the more conservative score

This process produces three things that matter in GRC as much as
in OHS: **accuracy, defensibility, and documented rationale.**

### The Conservative Scoring Principle

**When assessors disagree, default to the higher risk score.**

This is not risk aversion. It is professional discipline — the
recognition that the cost of underscoring a risk that materializes
is almost always higher than the cost of overscoring a risk that
doesn't.

In OHS: underscoring a risk means someone gets hurt.
In GRC: underscoring a risk means an exploited vulnerability that
a higher score would have prioritized for remediation.

The precautionary principle — when uncertain, err on the side of
caution — is as applicable to GRC risk scoring as it is to
workplace safety.

### Documented Rationale

**Every risk score should have a record of how it was reached.**

| What to document | Why it matters |
|-----------------|---------------|
| Who scored the risk | Accountability and expertise validation |
| What scoring method was used | Reproducibility and consistency |
| What variables were assessed and why | Defensibility if score is challenged |
| Whether consensus was reached | Transparency about scoring confidence |
| Final score and risk level | The decision that drives remediation priority |

A score without rationale is an opinion. A score with documented
rationale is evidence.

---

## Implications for GRC Practice

**Five changes to risk scoring practice derived from OHS methodology.**

1. **Add Exposure as an explicit scoring variable** — don't collapse
   frequency of asset-threat contact into Likelihood. Score it
   separately. It changes the risk profile in ways a two-variable
   model misses.

2. **Calibrate Exposure to your asset inventory** — internet-facing
   systems, widely distributed credentials, and high-volume data
   processing workflows all carry high exposure scores regardless
   of likelihood or impact.

3. **Require peer review for high and very high risk scores** —
   don't let consequential scores rest on a single assessor's
   judgment. Build a consensus process into your scoring methodology.

4. **Default to the conservative score when assessors disagree** —
   the precautionary principle applies. Underscoring a risk that
   materializes is almost always more costly than overscoring one
   that doesn't.

5. **Document the rationale for every risk score** — who scored it,
   what method was used, what variables were considered, whether
   consensus was reached. A score without rationale is an opinion.
   A score with documented rationale is evidence.

---

## Key Takeaways

- Fine-Kinney and NIST 800-30 are the same underlying logic —
  probability × severity — with different levels of precision
- Fine-Kinney's three-variable model is more precise than NIST's
  two-variable model because it separates Exposure from Likelihood
- Exposure — frequency of asset-threat contact — is an independent
  risk multiplier that changes the risk profile in ways Likelihood
  alone doesn't capture
- GRC risk scoring should adopt a three-variable model: Likelihood
  × Exposure × Impact
- Risk scores are only as defensible as the process that produced
  them — consensus, conservative bias, and documented rationale
  are the structural safeguards
- When assessors disagree, default to the more conservative score —
  the precautionary principle applies in GRC as much as in OHS

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)

---

*Part of the [risk-assessment-methodology](../README.md) repository.*
*Next: [corrective-action-to-remediation.md](corrective-action-to-remediation.md) — coming soon*
