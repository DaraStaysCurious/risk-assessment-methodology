# Risk Assessment Methodology
## A GRC Framework Derived from Occupational Health & Safety Practice

**Author:** Dara Thomas
**Status:** Living document — updated as methodology evolves
**Related projects:** [grc-trustpath-usable-security] · [secure-design-framework]

---

## What this is

This repository documents a risk assessment methodology built at the 
intersection of three disciplines:

- **Occupational Health & Safety** — a decade of workplace risk assessment,
hazard identification, incident investigation, and control implementation
- **UX Design & Research** — years of observing how people behave inside
complex systems, where they break down, and how to redesign them around
actual human behavior
- **Governance, Risk & Compliance** — the framework language that translates
both into auditable controls and defensible security programs

The central argument is simple:

**GRC risk assessment and OHS risk assessment are the same discipline
with different vocabulary. And both are made more effective — or fail
entirely — based on how well they account for human behavior.**

---

## Why this exists

Most GRC risk assessments are conducted by people who learned risk
management through security frameworks. This methodology was developed
by someone who learned risk management by standing on factory floors,
interviewing welders and machine operators, investigating near misses,
and figuring out why controls that looked perfect on paper kept failing
in practice.

That experience produced a set of convictions about how risk assessment
actually works — convictions that map cleanly onto GRC methodology once
you know where to look.

This document makes that mapping explicit.

---

## The core thesis

Unsafe behavior is almost always a system design failure, not a human
failure.

When a welder uses cardboard instead of a fire-rated welding blind, the
problem isn't the welder. The problem is that the welding blind was
stored three floors below where the work was being done — making the
wrong behavior easier than the right one.

When an employee shares their password, the problem usually isn't the
employee. The problem is a password policy so complex that writing it
down feels like the only rational option.

**Controls fail when they're designed around ideal human behavior.
Controls succeed when they're designed around actual human behavior.**

This methodology builds that principle into every phase of risk
assessment — from hazard/threat identification through control design,
implementation, and effectiveness monitoring.

---

## How this repository is organized

| Document | What it covers |
|----------|---------------|
| `methodology-overview.md` | The complete methodology: OHS and GRC compared |
| `hazard-identification-to-threat-modeling.md` | OHS hazard ID → GRC threat identification |
| `risk-scoring-crosswalk.md` | OHS likelihood/severity → NIST 800-30 likelihood/impact |
| `corrective-action-to-remediation.md` | OHS corrective action → GRC remediation roadmaps |
| `human-factors-in-risk.md` | Where OHS and GRC most powerfully converge |
| `applications.md` | How this methodology is applied across the portfolio |

---

## Who this is for

- **GRC analysts** looking for a risk assessment approach grounded in
human behavior, not just framework compliance
- **Security teams** whose controls keep failing in practice despite
looking correct on paper
- **OHS professionals** considering a transition into GRC who want to
understand how their existing skills translate
- **Researchers** interested in the intersection of human factors,
usable security, and governance

---

## A note on methodology vs. framework

Frameworks tell you *what* to assess. Methodology tells you *how* to
think about what you're assessing.

NIST 800-30 is a framework. ISO 27005 is a framework. This document is
a methodology — a way of thinking about risk that makes any framework
more effective when applied.

I'm not trying to replace existing GRC frameworks. I'm documenting how
I use them — in the hope that it's useful to others navigating the same
intersection of human behavior and risk management.

---

## Related work

This methodology informs every project in this portfolio. See
[applications.md] for specific examples of how it's applied across
the GRC audit projects and the secure-design-framework.

*Part of the [DaraStaysCurious](https://github.com/DaraStaysCurious)
GRC & Cloud Security portfolio.*
