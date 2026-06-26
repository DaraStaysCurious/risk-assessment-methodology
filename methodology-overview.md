> **Status: Draft v1 — in progress.** This document is being condensed.
> Full methodology content is distributed across individual documents
> in this repository. This overview will be updated once all individual
> documents are complete.

---

# Methodology Overview
> OHS risk assessment and GRC risk assessment are the same discipline
> with different vocabulary — and both succeed or fail based on how
> well they account for human behavior.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [The Two Disciplines](#the-two-disciplines)
- [How This Repository Is Organized](#how-this-repository-is-organized)
- [The Complete Mapping](#the-complete-mapping)
- [Where They Diverge](#where-they-diverge)
- [The Missing Layer](#the-missing-layer)
- [Implications for GRC Practice](#implications-for-grc-practice)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

A decade in Occupational Health & Safety taught me that unsafe
behavior is almost always a system design failure — not a human
failure. Years in UX product design taught me to observe how people
behave inside broken systems and redesign them around actual human
behavior. GRC and cloud security study gave me the framework language
to translate both into auditable controls.

This document argues that OHS and GRC risk assessment are structurally
identical — same process, same logic, different vocabulary. It maps
every step of OHS practice onto NIST 800-30, names where they diverge,
and identifies the one layer GRC is missing that OHS has always had:
a systematic methodology for designing controls around how humans
actually behave.

This is not theory. It is a decade of practice, translated.

---

## The Two Disciplines

### Occupational Health & Safety
**OHS risk assessment answers one question: what could hurt someone
here, and what are we going to do about it?**

The stakes are immediate and physical — a missed hazard can mean
injury, disability, or death. This forces OHS into a discipline
grounded in how humans actually behave, not how procedures say they
should.

### GRC
**GRC risk assessment answers a parallel question: what could harm
this organization's information assets, and what are we going to
do about it?**

The stakes are less immediately visible but no less real — a missed
vulnerability means data breach, regulatory penalty, or reputational
damage. Controls that exist on paper but fail in practice leave
organizations exposed without knowing it.

### The Parallel

| | OHS | GRC |
|-|-----|-----|
| **Asset protected** | The human body | Information and systems |
| **Core question** | What could hurt someone here? | What could harm our information assets? |
| **Failure mode** | Controls that look right on paper but fail in practice | Controls that look right on paper but fail in practice |
| **Success condition** | Controls designed around actual human behavior | Controls designed around actual human behavior |

The difference is the domain. Everything else — the methodology,
the judgment calls, the stakeholder dynamics — is functionally
identical.

---

## How This Repository Is Organized

| Document | What it covers | Status |
|----------|---------------|--------|
| `methodology-overview.md` | Complete methodology: OHS and GRC compared | *This document* |
| [`hazard-identification-to-threat-modeling.md`](hazard-identification-to-threat-modeling.md) | OHS hazard ID → GRC threat identification | ✅ Complete |
| [`risk-scoring-crosswalk.md`](risk-scoring-crosswalk.md) | OHS likelihood/severity → NIST 800-30 likelihood/impact | ✅ Complete |
| `corrective-action-to-remediation.md` | OHS corrective action → GRC remediation roadmaps | *Coming soon* |
| `human-factors-in-risk.md` | Where OHS and GRC most powerfully converge | *Coming soon* |
| `applications.md` | How this methodology applies across the portfolio | *Coming soon* |

---

## The Complete Mapping
### OHS Practice → NIST 800-30

NIST 800-30 defines four steps: Prepare, Assess, Communicate,
Maintain. Every step maps directly to OHS practice.

### Step 1: Prepare
**Before touching anything, establish why the assessment is happening.**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| "What brought this to my desk?" | Purpose of the assessment |
| Defining which task is being assessed | Scope definition |
| "Did something happen / almost happen?" | Prior incident information |
| Legislation and policy research | Applicable laws and policies |

> **What OHS adds:** NIST defines preparation as a documentation
> exercise. OHS adds a diagnostic conversation first — surfacing
> organizational history and unspoken concerns before a single
> framework requirement is reviewed.

---

### Step 2: Assess
**Identify threats, vulnerabilities, likelihood, and impact.**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Quiet observation of the task | Threat source identification |
| Employee task walkthrough | Threat event identification |
| Pain points and frustrations captured | Predisposing conditions |
| Prior incidents and near misses | Likelihood determination |
| Physical harm potential | Impact determination |

> **What OHS adds:** The most significant threats are often invisible
> in documentation but immediately visible to the people performing
> the task. Direct observation and structured interviews are primary
> identification methods — not optional supplements.

---

### Step 3: Communicate
**Present findings and develop controls collaboratively.**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Findings discussion with employees | Stakeholder communication |
| Collaborative control identification | Risk response development |
| Supervisor approval | Risk treatment authorization |
| SOP review and update | Policy and procedure development |
| Employee sign-off | Control acknowledgment and documentation |

> **What OHS adds:** NIST treats communication as a reporting
> exercise. OHS treats it as a collaborative design process —
> because controls designed without user input get routed around.
> Every time.

---

### Step 4: Maintain
**Verify that controls work in practice, not just on paper.**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Post-implementation monitoring period | Control effectiveness monitoring |
| Watching for workaround behavior | Control failure detection |
| Revisiting on incident or condition change | Assessment maintenance triggers |

> **What OHS adds:** A defined post-implementation observation period
> — physically verifying that the control is being used as intended.
> Documentation is not evidence of effectiveness. Behavior is.

---

## Where They Diverge

**GRC is more complex than OHS in four meaningful ways.**

| Dimension | OHS | GRC |
|-----------|-----|-----|
| **Asset** | Tangible, immediate, unambiguous | Abstract, delayed, distributed |
| **Threat landscape** | Bounded physical environment | Dynamic, intelligent, unbounded |
| **Regulatory environment** | Relatively unified (OSHA) | Fragmented, overlapping frameworks |
| **Pace of change** | Manageable, observable | Daily vulnerability discoveries, continuous adaptation |

OHS practitioners moving into GRC don't need to start over.
They need to expand — adding threat intelligence, multi-framework
fluency, and a continuous assessment mindset to a methodological
foundation that is already solid.

---

## The Missing Layer
### What GRC Can Learn from OHS

**GRC acknowledges human factors. OHS has methodology for them.**

Every security awareness training program acknowledges that humans
introduce risk. But acknowledgment is not methodology. OHS developed
systematic, practiced approaches to understanding how specific humans
behave inside specific systems — and designing controls around that
behavior. GRC largely has not.

The consequences are visible everywhere in security practice.

### The Five Principles

**1. The people closest to the risk know the most about it.**
Draw out their knowledge through deliberate structured conversation.
Treat it as primary evidence, not anecdote.

**2. Resistance is data.**
Classify it: convenience resistance signals a control design problem.
Substantive resistance signals a gap in your risk assessment. Neither
should be dismissed without examination.

**3. Friction kills controls.**
A control that requires significant extra effort will be routed around
— not occasionally, but reliably. Design controls so correct behavior
is always easier than the workaround.

**4. Absence of incident is not evidence of absence of risk.**
"We've never been breached" is not a risk assessment. Near misses,
failed logins, and caught phishing emails are likelihood data —
not reassurance.

**5. Co-design produces better controls than top-down design.**
Controls developed with the people who must use them are more
effective, more durable, and more practically intelligent than
controls handed down for implementation.

### Why This Layer Is Missing from GRC

GRC developed as a technical and legal discipline focused on
framework compliance and audit readiness. The question it was built
to answer is "are we compliant?" — not "do our controls actually
work?"

OHS never had that luxury. Controls that fail in practice have
immediate, visible consequences. The discipline was forced to develop
human factors methodology. GRC should adopt it — not as a replacement
for technical rigor, but as the layer underneath it.

---

## Implications for GRC Practice

**Seven changes that produce materially better risk assessments
without materially increasing scope.**

1. **Start with a diagnostic conversation** — before opening any
   framework document, find out why the assessment is really happening.

2. **Interview the people inside the system** — not a survey, a
   conversation. Ask what they actually do, not what policy says
   they should do.

3. **Treat resistance as diagnostic data** — classify it before
   dismissing it. It almost always contains information.

4. **Design controls collaboratively** — present options, not
   mandates. Co-design produces controls that work.

5. **Assess friction before finalizing recommendations** — ask what
   the easiest way to not do this is. If the workaround is easier
   than compliance, the control will fail.

6. **Treat near misses as high-signal likelihood data** — investigate
   them with the same rigor as actual incidents.

7. **Verify effectiveness through observation** — a control isn't
   implemented until it's been observed working in the environment
   where the risk lives.

---

## Key Takeaways

- OHS and GRC risk assessment are structurally identical — same
  process, different vocabulary
- The most significant difference is not methodology but domain
  complexity — GRC requires expanded threat intelligence and
  multi-framework fluency
- GRC's primary gap is human factors methodology — OHS has it,
  GRC inconsistently applies it
- Controls designed without user input get routed around — always
- Documentation is not evidence of effectiveness — behavior is
- The goal of risk assessment is not compliant documentation —
  it is actual risk reduction

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)
