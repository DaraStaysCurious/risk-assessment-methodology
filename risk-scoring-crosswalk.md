# Risk Scoring Crosswalk
> OHS and GRC risk scoring are the same underlying logic with
> different variables — and OHS got one of those variables right
> that GRC is still missing.

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

Risk scoring transforms qualitative observations into defensible,
prioritized decisions. Without a scoring model, findings are
opinions. With one, they are evidence.

This document maps the Fine-Kinney risk scoring method — used across
a decade of OHS practice on factory floors, oil rigs, and marine
environments — onto NIST 800-30 risk scoring. The two models share
the same underlying logic. Fine-Kinney is more precise because it
separates Exposure from Likelihood — capturing how frequently assets
or people contact a threat source as an independent risk multiplier.

**The argument:** GRC risk scoring should adopt a three-variable
model explicitly. Frequency of contact changes the risk profile in
ways a two-variable model consistently misses.

---

## The Fine-Kinney Method

**Risk = Likelihood × Exposure × Consequence**

### Likelihood (0.5 – 10)

| Score | Description |
|-------|-------------|
| 0.5 | Practically impossible |
| 1 | Conceivable but unlikely |
| 3 | Unusual but possible |
| 6 | Quite possible |
| 10 | To be expected |

### Exposure (0.5 – 10)

| Score | Description |
|-------|-------------|
| 0.5 | Very rarely — once a year or less |
| 1 | Rarely — monthly |
| 2 | Occasionally — weekly |
| 3 | Several times a week |
| 6 | Frequently — daily |
| 10 | Continuously — many times per day |

### Consequence (1 – 100)

| Score | Description |
|-------|-------------|
| 1 | Minor injury — first aid only |
| 3 | Significant injury — medical treatment |
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

---

## NIST 800-30 Risk Scoring

**Risk = Likelihood × Impact**

### Likelihood

| Level | Description |
|-------|-------------|
| Very Low | Threat source lacks capability or motivation |
| Low | Limited capability or motivation |
| Moderate | Some capability and motivation |
| High | Capable and motivated |
| Very High | Highly capable and highly motivated |

### Impact

| Level | Description |
|-------|-------------|
| Very Low | Negligible effect on operations |
| Low | Minor degradation — mission still performable |
| Moderate | Significant degradation — reduced effectiveness |
| High | Significant damage to assets or mission |
| Very High | Severe or catastrophic damage |

### Risk Matrix

| | Very Low Impact | Low | Moderate | High | Very High Impact |
|-|----------------|-----|----------|------|-----------------|
| **Very High Likelihood** | Low | Moderate | High | Very High | Very High |
| **High Likelihood** | Low | Moderate | High | High | Very High |
| **Moderate Likelihood** | Low | Low | Moderate | High | High |
| **Low Likelihood** | Very Low | Low | Low | Moderate | High |
| **Very Low Likelihood** | Very Low | Very Low | Low | Low | Moderate |

---

## The Complete Mapping

| Fine-Kinney | NIST 800-30 | Notes |
|-------------|-------------|-------|
| Likelihood (0.5–10) | Likelihood (Very Low–Very High) | Direct equivalent |
| Consequence (1–100) | Impact (Very Low–Very High) | Direct equivalent |
| Exposure (0.5–10) | **Not explicitly modeled** | **The gap** |
| Quantitative score | Qualitative matrix | Different output, same logic |
| Stop activity > 400 | Very High — immediate action | Equivalent escalation threshold |

**Where they align:** both assess probability and severity, produce
a risk level that drives prioritization, and escalate the highest
scores to immediate action.

**Where they diverge:** Fine-Kinney separates Exposure from
Likelihood. NIST collapses them together — losing precision for
risks involving frequent asset-threat contact.

---

## The Exposure Gap

**NIST 800-30's two-variable model systematically underscores
risks involving frequent contact between assets and threat sources.**

### The Problem

| | System A | System B |
|-|----------|----------|
| Vulnerability | Weak authentication | Weak authentication |
| Impact if exploited | High | High |
| Likelihood of exploit | High | High |
| Exposure | 2 admins, monthly access | 500 employees, daily access |
| **NIST 800-30 score** | **High** | **High** |
| **Fine-Kinney score** | **Substantial** | **Very High** |

NIST scores these identically. Fine-Kinney scores System B
dramatically higher — because 500 daily users create exponentially
more exploit opportunities than 2 monthly users.

### Where Exposure Matters Most in GRC

| High exposure scenario | Why it matters |
|-----------------------|---------------|
| Internet-facing login portals | Thousands of authentication attempts daily |
| Shared credentials across teams | Every user is a potential exploit vector |
| High-volume APIs | Millions of calls create millions of opportunities |
| Widely distributed sensitive data | More access = more exposure surface |
| Remote workforce on unmanaged devices | Daily exposure to uncontrolled environments |

### Proposed GRC Exposure Scale

| Score | Description |
|-------|-------------|
| 1 | Very low — accessed rarely, limited users |
| 2 | Low — accessed occasionally, small user group |
| 3 | Moderate — accessed regularly, defined user group |
| 6 | High — accessed frequently, large user group |
| 10 | Very high — internet-facing or accessed continuously |

**Proposed GRC formula:**
> **Risk = Likelihood × Exposure × Impact**

---

## Risk Scoring Governance

**A risk score is only as defensible as the process that produced it.**

### The Consensus Process

When assessors disagree on a risk score:

| Step | Action |
|------|--------|
| 1 | Two assessors score independently |
| 2 | If scores diverge, bring in a third assessor |
| 3 | Walk through the scenario together |
| 4 | Seek consensus through structured discussion |
| 5 | If no consensus — senior assessor decides, defaulting to the more conservative score |

### The Conservative Scoring Principle

**When uncertain, default to the higher risk score.**

The cost of underscoring a risk that materializes is almost always
higher than the cost of overscoring one that doesn't. In OHS,
underscoring means someone gets hurt. In GRC, underscoring means
an exploited vulnerability that a higher score would have prioritized
for remediation.

### Document the Rationale

| What to document | Why |
|-----------------|-----|
| Who scored the risk | Accountability |
| Scoring method used | Reproducibility |
| Variables assessed and why | Defensibility |
| Whether consensus was reached | Transparency |
| Final score and risk level | The decision that drives remediation |

**A score without rationale is an opinion.
A score with documented rationale is evidence.**

---

## Implications for GRC Practice

1. **Add Exposure as an explicit scoring variable** — frequency
   of asset-threat contact is an independent risk multiplier.
2. **Calibrate Exposure to your asset inventory** — internet-facing
   systems and widely distributed credentials carry high exposure
   scores regardless of likelihood or impact.
3. **Require peer review for high and very high scores** — build
   a consensus process into your scoring methodology.
4. **Default to the conservative score when assessors disagree** —
   the precautionary principle applies in GRC as much as in OHS.
5. **Document the rationale for every score** — who scored it,
   what method, what variables, whether consensus was reached.

---

## Key Takeaways

- Fine-Kinney and NIST 800-30 are the same underlying logic —
  probability × severity — with different levels of precision
- Fine-Kinney's three-variable model is more precise because it
  separates Exposure from Likelihood
- Exposure — frequency of asset-threat contact — is an independent
  risk multiplier a two-variable model misses
- GRC risk scoring should adopt: Likelihood × Exposure × Impact
- Risk scores are only as defensible as the process that produced
  them — consensus, conservative bias, documented rationale
- When assessors disagree, default to the more conservative score

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)

---

*Part of the [risk-assessment-methodology](../README.md) repository.*
*Next: [corrective-action-to-remediation.md](corrective-action-to-remediation.md)*
