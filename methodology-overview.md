> **Status: Living document** — updated as methodology evolves
> and portfolio projects are completed.

---

# Methodology Overview
> OHS risk assessment and GRC risk assessment are the same discipline
> with different vocabulary — and both succeed or fail based on how
> well they account for human behavior.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [The Core Argument](#the-core-argument)
- [The Two Disciplines](#the-two-disciplines)
- [How This Repository Is Organized](#how-this-repository-is-organized)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

A decade in Occupational Health & Safety taught me that unsafe
behavior is almost always a system design failure — not a human
failure. Years in UX product design taught me to observe how people
behave inside broken systems and redesign them around actual human
behavior. GRC study gave me the framework language to translate
both into auditable controls.

This repository documents what happened when I mapped my OHS risk
assessment practice onto GRC methodology — and discovered the
translation was almost entirely one-to-one.

The individual documents in this repository make the mapping
explicit, step by step. This overview tells you where to start.

---

## The Core Argument

**Three arguments. Each documented in depth in this repository.**

**1. OHS and GRC risk assessment are structurally identical.**
Same process. Same logic. Same failure modes. Different vocabulary
and different domain. The complete mapping is in
[`hazard-identification-to-threat-modeling.md`](hazard-identification-to-threat-modeling.md),
[`risk-scoring-crosswalk.md`](risk-scoring-crosswalk.md), and
[`corrective-action-to-remediation.md`](corrective-action-to-remediation.md).

**2. OHS risk scoring is more precise than NIST 800-30.**
The Fine-Kinney method uses three variables — Likelihood, Exposure,
and Consequence — where NIST 800-30 uses two. The missing variable
is Exposure: how frequently assets or people come into contact with
a threat source. Frequency of contact is an independent risk
multiplier that a two-variable model consistently underscores. The
full argument is in
[`risk-scoring-crosswalk.md`](risk-scoring-crosswalk.md).

**3. GRC is missing a human factors methodology that OHS has
always had.**
GRC acknowledges that humans introduce risk. OHS has systematic,
practiced methodology for designing controls around how humans
actually behave — not how procedures say they should. The
consequences of that gap are visible everywhere in security
practice. The full argument, with three case studies, is in
[`human-factors-in-risk.md`](human-factors-in-risk.md).

---

## The Two Disciplines

**Same process. Different domain. Different stakes.**

| | OHS | GRC |
|-|-----|-----|
| **Asset protected** | The human body | Information and systems |
| **Core question** | What could hurt someone here? | What could harm our information assets? |
| **Failure mode** | Controls that look right on paper but fail in practice | Controls that look right on paper but fail in practice |
| **Success condition** | Controls designed around actual human behavior | Controls designed around actual human behavior |
| **What's at stake** | Injury, disability, death | Data breach, regulatory penalty, reputational damage |

The difference is the domain. The methodology is identical.

---

## How This Repository Is Organized

**Start with the document most relevant to you.**

| Document | What it covers | Status |
|----------|---------------|--------|
| `methodology-overview.md` | The complete argument — start here | *This document* |
| [`hazard-identification-to-threat-modeling.md`](hazard-identification-to-threat-modeling.md) | OHS hazard ID → GRC threat identification | ✅ Complete |
| [`risk-scoring-crosswalk.md`](risk-scoring-crosswalk.md) | Fine-Kinney → NIST 800-30 risk scoring | ✅ Complete |
| [`corrective-action-to-remediation.md`](corrective-action-to-remediation.md) | OHS corrective action → GRC remediation | ✅ Complete |
| [`human-factors-in-risk.md`](human-factors-in-risk.md) | Where OHS and GRC most powerfully converge | ✅ Complete |
| [`applications.md`](applications.md) | How this methodology applies across the portfolio | ✅ Complete |

**Not sure where to start?**

- **GRC analyst or hiring manager** → [`human-factors-in-risk.md`](human-factors-in-risk.md)
- **OHS professional considering GRC** → [`hazard-identification-to-threat-modeling.md`](hazard-identification-to-threat-modeling.md)
- **UX designer or researcher** → [`human-factors-in-risk.md`](human-factors-in-risk.md)
- **Security researcher** → [`risk-scoring-crosswalk.md`](risk-scoring-crosswalk.md)
- **See methodology in practice** → [`applications.md`](applications.md)

---

## Key Takeaways

- OHS and GRC risk assessment are structurally identical —
  same process, different vocabulary
- Fine-Kinney's three-variable model is more precise than NIST
  800-30's two-variable model — Exposure is the missing variable
- GRC's primary gap is human factors methodology — OHS has it,
  GRC inconsistently applies it
- Controls designed without user input get routed around — always
- Unsafe behavior is almost always a system design failure —
  not a human failure
- Documentation is not evidence of effectiveness — behavior is

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)
