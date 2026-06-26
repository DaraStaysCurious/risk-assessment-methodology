# Hazard Identification to Threat Modeling
> OHS hazard identification and GRC threat identification are the same
> process in different environments — and OHS has developed techniques
> for comprehensive, accurate identification that GRC would benefit
> from adopting explicitly.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [Vocabulary Guide](#vocabulary-guide)
- [What Hazard Identification Actually Is](#what-hazard-identification-actually-is)
- [What Threat Identification Actually Is](#what-threat-identification-actually-is)
- [The Complete Mapping](#the-complete-mapping)
- [The Real-Time Risk Assessment](#the-real-time-risk-assessment)
- [Living Assessment Tools](#living-assessment-tools)
- [Implications for GRC Practice](#implications-for-grc-practice)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

Every risk assessment begins with the same question: what could go
wrong here? The quality of everything that follows — likelihood
ratings, impact assessments, control recommendations — depends
entirely on how completely that question is answered.

This document maps OHS hazard identification practice onto GRC threat
identification methodology. It draws on a decade of daily inspections
across factory floors, oil rigs, and marine environments to show
where the two disciplines are structurally identical — and where OHS
practice has developed techniques that GRC consistently underuses:
real-time risk assessment, version-controlled living assessment tools,
and collaborative two-person inspection.

---

## Vocabulary Guide

**The two fields use different words for identical concepts.**

| OHS term | GRC equivalent |
|----------|---------------|
| Hazard | Threat source |
| Hazard event | Threat event |
| Unsafe condition | Vulnerability |
| Environmental/organizational factor | Predisposing condition |
| Inspection checklist | Assessment framework / audit checklist |
| Daily walkabout | Continuous monitoring / assessment cycle |
| Twice-daily inspection | Dual assessment cadence |
| Top-down systematic route | Structured scope traversal |
| Rotating supervisor companion | Collaborative assessment / peer review |
| Database of inspection findings | Risk register |
| Version-controlled checklist | Living assessment framework |
| Near miss | Security indicator / precursor event |
| Cordoning off an area | Interim compensating control |
| Incident investigation | Security incident response |
| Photographic evidence | Digital forensic documentation |
| Witness interviews | Stakeholder interviews / incident debrief |

---

## What Hazard Identification Actually Is

**Effective hazard identification makes the invisible visible —
systematically, repeatedly, and with enough rigor that familiarity
bias doesn't determine what gets found.**

The challenge is not identifying obvious hazards. The challenge is
identifying hazards that have become invisible through familiarity
and normalization — the machine guard removed six months ago "just
temporarily," the chemical in an unmarked container, the walkway
everyone knows gets slippery but nobody has formally flagged.

### Three Components of Effective OHS Hazard Identification

**1. Structured systematic inspection**
A defined route, a versioned checklist, a consistent schedule.
Structure defeats familiarity bias — when the route is the same
every time, the brain builds a baseline of normal. Deviations become
visible precisely because the baseline is stable.

**2. Collaborative observation**
A single inspector is a single point of failure. Bringing a
supervisor on every inspection — rotating who attends each walkabout
— ensures a fresh perspective is always present alongside the trained
eye. The supervisor also has immediate authority to act on findings,
making the path from identification to remediation as short as
possible.

**3. Living documentation**
The inspection checklist is never finished. It is a versioned
artifact updated when new equipment arrives, workflows change, or
new hazard categories emerge. Findings are entered into a database
after each walkabout — creating a longitudinal record that makes
patterns visible over time.

### How Hazard Identification Fails

| Failure mode | What it looks like |
|--------------|-------------------|
| Familiarity bias | The longer you've worked somewhere, the more invisible its hazards become |
| Checklist ossification | A checklist that never changes creates false confidence |
| Single-point observation | One inspector has blind spots — collaborative inspection is the fix |
| Normalcy bias | "Nothing has happened yet" mistaken for "nothing will happen" |
| Scope drift | Hazards at the edges — interactions between systems, specific conditions — get missed |

---

## What Threat Identification Actually Is

**GRC threat identification faces the same challenge as OHS hazard
identification: systematically surfacing what could cause harm before
it does, in an environment where familiarity makes the most
significant threats hardest to see.**

### GRC Vocabulary

**Threat source** — anything with potential to trigger a threat event.
NIST 800-30 identifies four categories:

| Category | Examples |
|----------|---------|
| Adversarial | External attackers, insider threats, nation-state actors |
| Accidental | Misconfigured servers, accidentally deleted databases |
| Structural | Hardware failure, software bugs, aging infrastructure |
| Environmental | Power outages, natural disasters, physical security failures |

**Threat event** — the specific way a threat source causes harm.
The misconfigured server is the threat source. The exposed customer
database is the threat event.

**Vulnerability** — a weakness a threat source can exploit:
- Technical: unpatched software, weak access controls
- Process: no change management, inadequate separation of duties
- Human: untrained employees, password fatigue, social engineering

**Predisposing condition** — organizational factors that increase
likelihood: deadline pressure, understaffing, a culture that treats
security as an obstacle.

### How GRC Threat Identification Fails

| Failure mode | GRC equivalent of OHS failure |
|--------------|-------------------------------|
| Over-reliance on documentation | Describes how systems should work, not how they do |
| Underweighting human threat sources | Technical scans don't find behavioral vulnerabilities |
| Generic threat intelligence | Accurate about the landscape, inaccurate about specific terrain |
| Single-assessor observation | No structural requirement for fresh eyes |
| Static assessment tools | Frameworks that don't evolve with the environment |
| Normalcy bias | "We've never been breached" treated as evidence of safety |

---

## The Complete Mapping

**Every element of OHS hazard identification has a direct GRC
equivalent.**

### Inspection Route → Structured Scope Traversal

**Consistency of route produces consistency of coverage.**

In OHS: starting from the top floor and working down — every time.
The consistent route builds a mental baseline; deviations become
visible because the baseline is stable.

In GRC: define the asset inventory before beginning, establish a
consistent order for reviewing assets and systems, follow that order
every time. Let the route, not attention, determine coverage.

---

### Twice-Daily Inspections → Dual Assessment Cadence

**Conditions change within assessment cycles, not just between them.**

In OHS: morning and evening inspections catch hazards that emerge
during the working day — a spill, a removed guard, new equipment
moved onto the floor.

In GRC: monitoring checkpoints at multiple intervals within a defined
period — SIEM reviews, log analysis, automated alerts — catch changes
as they occur rather than at the next audit cycle.

---

### Rotating Supervisor Companion → Collaborative Assessment

**A single assessor is a single point of failure.**

In OHS: a different supervisor on every walkabout — fresh eyes that
catch what familiarity has made invisible, plus immediate authority
to act on findings without escalation delay.

In GRC: involve subject matter experts from different domains,
rotate who reviews which systems, build peer review into threat
identification as a structural feature — not optional quality check.

| OHS principle | GRC application |
|---------------|----------------|
| Fresh eyes on every inspection | Rotate assessors across domains |
| Supervisor has immediate authority | Escalation pathway built into assessment structure |
| Rotation prevents familiarity bias | Different reviewers for different system areas |

---

### Versioned Checklist → Living Assessment Framework

**An assessment tool that doesn't evolve becomes a liability.**

In OHS: checklist updated when new equipment arrives, workflows
change, or incidents reveal new hazard categories. Each version
numbered, dated, stored. Findings entered into a database for
longitudinal pattern analysis.

In GRC:

| OHS practice | GRC equivalent |
|--------------|---------------|
| Version-numbered checklist | Version-controlled assessment framework |
| Revision triggers: new equipment, workflow changes | Revision triggers: new systems, regulations, threat intel |
| Findings database | Risk register with longitudinal analysis |
| Pattern identification over time | Emerging risk detection across assessment cycles |

---

### Ad-Hoc Finding → Real-Time Risk Assessment

**When an unexpected hazard appears, the response is immediate
and structured.**

In OHS, a new finding during a walkabout triggers a consistent
sequence regardless of environment — factory floor, oil rig, or
cruise ship:

| Step | OHS action | GRC equivalent |
|------|-----------|----------------|
| 1 | Notate immediately | Document the finding on the spot |
| 2 | Rapid collaborative triage | Assess with a second perspective |
| 3 | Cordon off if medium/high risk | Implement interim compensating control |
| 4 | Develop solution options | Prepare remediation options before escalating |
| 5 | Escalate with constraints noted | Present finding, triage, and options to decision-maker |
| 6 | Obtain authorization | Formal risk treatment authorization |
| 7 | Procure remediation resources | Acquire and deploy remediation |
| 8 | Hand off to supervisors | Transfer to operational owner for implementation |

**The two-speed principle:**
- **Fast:** Identify, triage, contain — minutes to hours, within
  the assessor's authority
- **Deliberate:** Develop options, authorize, remediate, verify —
  hours to weeks, requires stakeholder involvement

The interim control buys time for deliberate remediation without
leaving the organization exposed.

---

### Near Misses → Security Indicators

**A near miss is evidence that the probability exists and is
actively materializing.**

In OHS: near misses investigated with almost the same rigor as
actual incidents. A workplace that tracks near misses seriously
learns from them before they become incidents.

In GRC:

| Near miss equivalent | What it signals |
|---------------------|----------------|
| Failed login attempts | Credential compromise being attempted |
| Caught phishing emails | Social engineering actively targeting the org |
| Anomalous access patterns | Authorized credentials may be compromised |
| Blocked malware | Malicious code being delivered to the environment |

These are not reassuring indicators. They are likelihood data.
The difference between a near miss and an incident is frequently
a control that worked once — but may not work again.

---

## The Real-Time Risk Assessment

**The structured informality of the OHS ad-hoc finding response
is a model for continuous risk management that GRC frequently lacks.**

Most GRC programs handle scheduled assessments well and ad-hoc
findings inconsistently. The OHS model — rigorous enough to produce
defensible risk decisions, flexible enough to execute in the middle
of a working day — closes that gap.

### Designing for Real-Time Response

For continuous risk management to work, three things must be defined
before they're needed:

**1. Triage criteria**
What makes a finding low, medium, or high priority? Define this
in advance so classification happens in seconds, not meetings.

**2. Compensating control authority**
Who can implement an interim control without waiting for full
escalation? That person should be as close to the identification
process as possible. Define the authority. Document it. Ensure
people have it before they need it.

**3. Escalation pathway**
How does a finding get from identification to the decision-maker
with authority to authorize remediation — and how fast? Every
layer of distance is a delay. Every delay is exposure.

---

## Living Assessment Tools

**An assessment tool that doesn't evolve with its environment
creates false confidence.**

### Version Control as Risk Management Discipline

| Practice | Why it matters |
|----------|---------------|
| Number and date every version | Creates audit trail of how the tool evolved |
| Define revision triggers in advance | New systems, regulations, threat intel, post-incident review |
| Store version history | Shows how assessment evolved alongside the environment |
| Enter every finding into a longitudinal record | Turns individual findings into systemic insight |

**A risk register updated continuously is a fundamentally different
tool than one refreshed at audit intervals.** The first tells you
what your risk landscape looks like right now. The second tells you
what it looked like last time someone checked.

---

## Implications for GRC Practice

**Seven structural changes derived from OHS hazard identification
practice.**

1. **Define and follow a structured scope traversal route** — let
   the route, not attention, determine coverage.

2. **Build collaborative observation into the assessment structure**
   — rotate reviewers, ensure fresh eyes at every significant
   assessment activity.

3. **Design immediate escalation pathways** — define who can implement
   compensating controls without waiting for full escalation, and
   make sure that person is close to the identification process.

4. **Treat near misses as seriously as incidents** — investigate,
   document, and use them to calibrate likelihood upward.

5. **Establish a real-time finding process** — define triage criteria,
   compensating control authority, and escalation pathways before
   they're needed.

6. **Version control your assessment tools** — define revision
   triggers, maintain version history, update after every significant
   environmental change.

7. **Enter every finding into a longitudinal record** — patterns
   reveal systemic vulnerabilities that point-in-time assessments
   miss.

---

## Key Takeaways

- OHS hazard identification and GRC threat identification are
  structurally identical — different vocabulary, same challenge
- The most significant threats are often invisible in documentation
  but immediately visible to the people doing the work
- Collaborative observation — rotating fresh eyes — catches what
  familiarity makes invisible to a single assessor
- Near misses are likelihood data, not reassurance
- Assessment tools that don't evolve with their environment create
  false confidence
- Real-time risk assessment requires defined triage criteria,
  compensating control authority, and escalation pathways — defined
  before they're needed
- Documentation is not evidence of effectiveness — behavior is

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)

---

*Part of the [risk-assessment-methodology](../README.md) repository.*
*Next: [risk-scoring-crosswalk.md](risk-scoring-crosswalk.md) — coming soon*
