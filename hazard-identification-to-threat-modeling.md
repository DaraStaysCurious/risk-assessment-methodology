# Hazard Identification to Threat Modeling
## How OHS Hazard Identification Practice Maps to GRC Threat Identification

---

> This document is part of the
> [risk-assessment-methodology](../README.md) repository.
> It expands on the mapping introduced in
> `methodology-overview.md`, providing a detailed examination
> of one specific phase of the risk assessment process:
> how threats and hazards are identified in the first place.

---

## Introduction

Every risk assessment begins with the same fundamental question:

**What could go wrong here?**

The quality of everything that follows — the likelihood ratings, the
impact assessments, the control recommendations, the remediation
roadmap — depends entirely on how well that question is answered.
A risk assessment that misses a significant hazard or threat source
at the identification stage will produce a control set with a gap
in it. That gap will persist through every subsequent phase of the
assessment, through audit, through remediation, and into production
— invisible until something exploits it.

Hazard identification in OHS and threat identification in GRC are
both attempts to answer that question as completely and accurately
as possible. They use different vocabulary, operate in different
environments, and draw on different bodies of knowledge — but the
underlying challenge is identical: systematically surfacing what
could cause harm before it does.

This document examines how OHS hazard identification practice —
developed across factory floors, oil rigs, and marine environments
over a decade of daily inspections, incident investigations, and
near miss analyses — maps onto GRC threat identification methodology.
It argues that OHS practice has developed several techniques for
comprehensive, accurate hazard identification that GRC practice
would benefit from adopting explicitly.

---

### What this document covers

- The OHS hazard identification process — what it is, how it works,
  and what makes it effective
- The GRC threat identification process — what it is, how it works,
  and where it frequently falls short
- A complete mapping between the two — every element of OHS hazard
  identification translated into GRC threat identification language
- Three principles from OHS practice that GRC threat identification
  is missing: real-time risk assessment, living assessment tools,
  and the two-person inspection principle
- Practical implications for GRC practitioners

---

### A note on terminology

Throughout this document, OHS and GRC terms are presented side by
side wherever they refer to the same underlying concept. The goal
is fluency in both vocabularies — because the ability to move
between them is itself a professional asset in a field that
increasingly needs practitioners who can bridge human factors and
technical security practice.

| OHS term | GRC equivalent |
|----------|---------------|
| Hazard | Threat source |
| Hazard event | Threat event |
| Risk assessment walkabout | Security assessment / audit |
| Inspection checklist | Assessment framework / audit checklist |
| Near miss | Security indicator / precursor event |
| Corrective action | Remediation / risk treatment |
| Interim control | Compensating control |
| Cordoning off an area | Containment |

## What Hazard Identification Actually Is

In OHS, hazard identification is the systematic process of finding
anything in a work environment that has the potential to cause harm
— before it does.

That definition sounds simple. The practice is not.

The challenge is not identifying obvious hazards. Obvious hazards
get identified. The challenge is identifying the hazards that have
become invisible — through familiarity, through normalization, through
the gradual drift of practice away from procedure that happens in
every workplace over time.

A machine guard that was removed six months ago "just temporarily"
and never replaced. A chemical stored in an unmarked container because
the label fell off and nobody got around to replacing it. A walkway
that everyone knows gets slippery when it rains but that nobody has
formally flagged because it hasn't caused an injury yet.

These are the hazards that hurt people. Not the obvious ones — the
ones that have become part of the background, accepted as normal,
invisible to the people who walk past them every day.

Effective hazard identification is the practice of making the
invisible visible — systematically, repeatedly, and with enough
rigor that familiarity bias doesn't determine what gets found.

---

### How it works in practice

Effective OHS hazard identification has three components that work
together:

**1. Structured systematic inspection**

A defined route, a versioned checklist, a consistent schedule —
not because creativity isn't valuable in hazard identification, but
because structure is what defeats familiarity bias. When the
inspection route is the same every time, the brain builds a baseline
of what normal looks like at each point on that route. Deviations
from that baseline become visible precisely because the baseline
is stable.

In practice: starting from the top floor and working down, twice
daily, with a checklist developed specifically for the environment
being assessed and versioned as that environment changes. Morning
and evening inspections — because conditions change between the
start and end of a working day, and a hazard that didn't exist at
7am can exist by 4pm.

**2. Collaborative observation**

A single inspector is a single point of failure. Every observer
has blind spots — areas of familiarity where the brain stops
seeing and starts assuming. The practical solution is deliberate
collaborative observation: bringing a supervisor on every
inspection, rotating which supervisor attends each walkabout,
ensuring that a fresh pair of eyes is always present alongside
the trained eye of the safety professional.

This serves a second function: the supervisor present during the
inspection has immediate authority to act on findings. The path
from identification to remediation is as short as it can possibly
be — the person who can cordon off an area, stop a process, or
authorize an immediate fix is standing next to you when you find
the problem.

**3. Living documentation**

The inspection checklist is not a static document. It is a versioned
artifact that evolves with the environment it governs. New equipment
gets added to the checklist. Retired processes get removed. New
workflows create new hazard categories that require new checklist
items. Each version is numbered, dated, and stored — creating an
audit trail of how the assessment tool has evolved alongside the
environment.

Inspection findings are entered into a database after each walkabout
— not filed in a folder and forgotten, but recorded in a system
that allows patterns to be identified over time. A hazard that
appears in the database three times in two weeks is a different
risk than a hazard that appears once. The database makes that
difference visible.

---

### What makes hazard identification fail

Hazard identification fails in predictable ways. Recognizing these
failure modes is as important as understanding the methodology —
because they appear in GRC practice with the same regularity they
appear in OHS.

**Familiarity bias:** The longer an inspector has worked in an
environment, the more invisible its hazards become. What was once
noticed becomes assumed. The solution is structured routine combined
with fresh eyes — not relying on either alone.

**Checklist ossification:** A checklist that never changes becomes
a liability. It gives false confidence that everything is being
checked when the environment has evolved beyond what the checklist
covers. Version control and regular checklist reviews are the
practical solution.

**Single-point observation:** One inspector, no matter how skilled,
has blind spots. Collaborative inspection — rotating observers,
fresh eyes at every walkabout — is the structural solution to
individual perceptual limitation.

**Normalcy bias:** The hazard that hasn't caused an incident yet
gets treated as less urgent than the hazard that has. Near misses
get noted but not investigated with the same rigor as actual
incidents. Over time, the gap between "hasn't hurt anyone yet"
and "won't hurt anyone" collapses in the minds of the people
working around it — until it does.

**Scope drift:** Hazard identification that focuses only on the
most obvious risk categories misses the hazards that live at the
edges — the interactions between systems, the conditions that only
arise under specific combinations of circumstances, the risks that
emerge from workflow changes nobody thought to flag to the safety
manager.

## What Threat Identification Actually Is

In GRC, threat identification is the systematic process of finding
anything that has the potential to cause harm to an organization's
information assets, systems, or operations — before it does.

The parallel to OHS hazard identification is exact. The environment
is different. The assets being protected are different. The
vocabulary is different. The underlying challenge is identical:
systematically surfacing what could cause harm before it does,
in an environment where familiarity, normalization, and assumption
make the most significant threats the hardest to see.

---

### The vocabulary of GRC threat identification

Before mapping OHS practice onto GRC methodology, it helps to
understand precisely what GRC means by the terms it uses — because
the vocabulary is specific and the distinctions matter.

**Threat source**
Anything with the potential to trigger a threat event. NIST 800-30
identifies four categories:

- *Adversarial* — malicious actors: external attackers, insider
  threats, competitors, nation-state actors
- *Accidental* — unintentional actions by authorized users: a
  misconfigured server, an accidentally deleted database, a file
  sent to the wrong recipient
- *Structural* — failures of equipment or software: hardware
  failure, software bugs, aging infrastructure
- *Environmental* — natural or physical events: power outages,
  natural disasters, physical security failures

In OHS terms: a threat source is a hazard. The categories map
roughly to: deliberate sabotage, human error, equipment failure,
and environmental conditions.

**Threat event**
The specific way a threat source causes harm. A threat source is
the condition or actor; a threat event is the action or occurrence.

- Threat source: an external attacker
- Threat event: a phishing campaign that compromises employee
  credentials and provides unauthorized access to financial systems

In OHS terms: the threat source is the unguarded machine; the
threat event is the moment a sleeve catches and pulls someone in.

**Vulnerability**
A weakness that a threat source can exploit to cause a threat event.
Vulnerabilities exist in systems, processes, and human behavior.

- Technical vulnerability: unpatched software, misconfigured access
  controls, weak encryption
- Process vulnerability: no formal change management process,
  inadequate separation of duties, missing incident response procedure
- Human vulnerability: untrained employees, password fatigue,
  susceptibility to social engineering

In OHS terms: a vulnerability is the condition that allows a hazard
to cause harm — the missing guard, the unmarked chemical container,
the wet floor without a warning sign.

**Predisposing condition**
An organizational or environmental characteristic that increases
the likelihood that a vulnerability will be exploited. Predisposing
conditions are frequently invisible in technical assessments because
they live in organizational culture, workflow pressure, and human
behavior rather than in systems.

- Deadline pressure that causes developers to skip security reviews
- Understaffing that leaves security tickets unresolved for weeks
- A culture where raising security concerns is seen as obstructing
  business objectives
- Remote work environments that reduce visibility into employee
  behavior and increase reliance on unmanaged devices

In OHS terms: predisposing conditions are the environmental factors
that make hazards more likely to cause harm — the noisy factory
floor that masks warning signals, the 12-hour shifts that increase
fatigue and error rates, the production pressure that makes
shortcuts feel necessary.

---

### How GRC threat identification works in practice

Standard GRC threat identification draws on several sources:

**Documentation review**
System architecture diagrams, network topology maps, data flow
diagrams, asset inventories, existing policies and procedures,
previous audit findings, incident logs. This establishes what
the organization says it has and how it says things work.

**Technical assessment**
Vulnerability scanning, penetration testing, configuration review,
access control analysis. This establishes what vulnerabilities
actually exist in the technical environment.

**Threat intelligence**
External information about the current threat landscape — known
attacker tactics, techniques, and procedures (TTPs); industry-
specific threat reports; regulatory guidance on emerging risks.
This establishes what threat sources are actively operating in
the environment relevant to the organization.

**Stakeholder interviews**
Conversations with system owners, IT staff, business process owners,
and end users about how systems are actually used, where pain points
exist, and what workarounds have developed. This is where GRC
practice most directly parallels OHS hazard identification — and
where it is most frequently underweighted relative to its value.

---

### Where GRC threat identification frequently falls short

GRC threat identification fails in ways that map almost exactly
onto OHS hazard identification failure modes — which is not a
coincidence. They are the same underlying challenge in different
environments.

**Over-reliance on documentation**
Documentation describes how systems are supposed to work. It rarely
describes how they actually work. The gap between documented
architecture and actual system behavior is where some of the most
significant vulnerabilities live — and documentation review alone
will not surface them.

**Underweighting human and organizational threat sources**
Technical vulnerability scanning finds technical vulnerabilities.
It does not find the developer who has been reusing the same
password across systems for three years, the business process that
requires employees to share credentials to meet a deadline, or the
culture that treats security tickets as low priority. These are
threat sources — and they are frequently invisible in assessments
that prioritize technical analysis over human and organizational
observation.

**Treating threat intelligence as a substitute for environmental
observation**
Knowing what threat actors are doing in the broader landscape is
valuable. It does not tell you how those threat actors would
interact with this specific organization's specific systems, culture,
and human behavior. Generic threat intelligence applied without
environmental observation produces generic risk assessments —
accurate about the landscape, inaccurate about the specific
terrain.

**Single-assessor observation**
A single assessor has blind spots. In GRC, unlike OHS, there is
rarely a structural requirement for collaborative observation during
threat identification. Assessments are frequently conducted by one
person reviewing documentation and running scans — with no
equivalent of the rotating supervisor who brings fresh eyes to
every inspection.

**Static assessment tools**
Assessment frameworks and checklists that don't evolve with the
environment they govern become liabilities — creating false
confidence that everything is being assessed when the environment
has moved on. Unlike OHS practice, GRC assessment tools are
frequently not version-controlled or regularly reviewed for
completeness against a changing asset and threat landscape.

**Normalcy bias**
"We've never been breached" functions in GRC exactly as "I haven't
gotten hurt doing this before" functions in OHS. It conflates the
absence of a realized incident with the absence of risk — and it
suppresses action on vulnerabilities that haven't yet been exploited.
Failed login attempts, caught phishing emails, and anomalous access
patterns are the GRC equivalent of near misses. They are likelihood
data, not reassurance.

## The Complete Mapping
### OHS Hazard Identification → GRC Threat Identification

The two disciplines have been introduced separately. Now the mapping
becomes explicit.

What follows is a complete translation of OHS hazard identification
practice into GRC threat identification language — not as a metaphor,
but as a structural parallel. Every element of OHS practice described
in Section 2 has a direct GRC equivalent. Every failure mode
described in Section 3 has a direct OHS parallel.

The table below provides the high-level mapping. The sections that
follow examine each element in depth.

---

### High-level mapping table

| OHS hazard identification | GRC threat identification |
|--------------------------|--------------------------|
| Hazard | Threat source |
| Hazard event | Threat event |
| Unsafe condition | Vulnerability |
| Environmental/organizational factor | Predisposing condition |
| Inspection checklist | Assessment framework / audit checklist |
| Daily walkabout | Continuous monitoring / assessment cycle |
| Twice-daily inspection schedule | Dual assessment cadence |
| Top-down systematic route | Structured scope traversal |
| Rotating supervisor companion | Collaborative assessment / peer review |
| Database of inspection findings | Risk register |
| Version-controlled checklist | Living assessment framework |
| Near miss | Security indicator / precursor event |
| Cordoning off an area | Interim compensating control / containment |
| Incident investigation | Security incident response |
| Photographic evidence | Digital forensic documentation |
| Witness interviews | Stakeholder interviews / incident debrief |

---

### Element 1: The inspection route → Structured scope traversal

**In OHS:**
Starting from the top floor and working down — every time, without
exception. The consistency of the route is not a constraint on
thoroughness. It is the mechanism that produces thoroughness. A
consistent route builds a mental baseline of what normal looks like
at every point in the environment. Deviations from that baseline
become visible precisely because the baseline is stable.

**In GRC:**
Structured scope traversal is the practice of defining the boundaries
of an assessment and working through them systematically — asset
by asset, system by system, domain by domain — rather than following
attention or intuition.

In practice this means: define the asset inventory before beginning
the assessment, establish a consistent order for reviewing assets
and systems, and follow that order every time. The consistency
builds the same baseline effect as the OHS inspection route —
making deviations, changes, and anomalies visible against a stable
reference point.

**What OHS practice adds:**
The physical discipline of a defined inspection route makes the
baseline-building mechanism explicit and non-negotiable. GRC
assessments frequently lack this discipline — assessors follow
their attention, which means familiar systems get reviewed
thoroughly and unfamiliar ones get reviewed superficially. Structured
scope traversal corrects this by making the route, not the assessor's
attention, the determinant of coverage.

---

### Element 2: Twice-daily inspections → Dual assessment cadence

**In OHS:**
Morning and evening inspections — not because the checklist changes
between them, but because conditions change. A hazard that didn't
exist at the start of the day can exist by its end. New equipment
gets moved onto the floor. A spill happens. A guard gets removed
for maintenance and not replaced. The twice-daily cadence catches
these changes before they cause harm.

**In GRC:**
A dual assessment cadence applies the same logic to continuous
monitoring — recognizing that the threat landscape and the
organizational environment both change within assessment cycles,
not just between them.

In practice this means building monitoring checkpoints at multiple
points within a defined period — not just at the start and end of
an audit cycle, but at regular intervals that catch changes as they
occur. Automated monitoring tools, security information and event
management (SIEM) systems, and regular log reviews are the GRC
equivalents of the twice-daily walkabout.

**What OHS practice adds:**
The twice-daily inspection instills a continuous monitoring mindset
that point-in-time assessments don't develop. The question is not
"is everything safe right now?" but "what has changed since the
last time I looked?" That question — asked twice daily, every day
— produces a fundamentally different relationship with risk than
an annual assessment produces.

---

### Element 3: The rotating supervisor companion →
### Collaborative assessment and peer review

**In OHS:**
A different supervisor on every walkabout — one for the morning
inspection, another for the evening. This serves two functions
simultaneously: fresh eyes that catch what familiarity has made
invisible to the trained inspector, and immediate authority to
act on findings without escalation delay.

The rotation matters as much as the collaboration. The same
supervisor every day would develop the same familiarity bias as
the inspector. Rotating ensures that a genuinely fresh perspective
is present at every inspection.

**In GRC:**
Collaborative assessment is the practice of involving more than
one assessor in threat identification — not as a quality check
after the assessment is complete, but as a structural feature of
the assessment itself.

In practice this means: involving subject matter experts from
different domains in the assessment process, rotating who reviews
which systems and domains, and building peer review into threat
identification rather than treating it as a solo activity followed
by an optional review.

The immediate authority principle maps to **escalation pathway
design** — ensuring that the person with authority to act on a
finding is as close to the finding as possible. In GRC terms:
threat identification findings should reach the person with
authority to authorize remediation through the shortest possible
path, not through a chain of reports and meetings that introduces
delay between identification and action.

**What OHS practice adds:**
GRC assessments are frequently single-assessor activities. The
structural requirement for collaborative observation — built into
the daily inspection routine rather than treated as optional peer
review — is something GRC practice could adopt explicitly. A
finding that two people with different perspectives have both
examined is a more reliable finding than one that a single assessor
identified alone.

---

### Element 4: The versioned checklist → Living assessment framework

**In OHS:**
The inspection checklist is a versioned document — updated when
new equipment arrives, when workflows change, when new hazard
categories emerge from incident investigation. Each version is
numbered, dated, and stored. The checklist is never treated as
complete or final. It is treated as a current best approximation
of what needs to be assessed, subject to revision as the
environment evolves.

Findings from each inspection are entered into a database —
creating a longitudinal record that makes patterns visible over
time. A hazard that appears three times in two weeks is a different
risk than a hazard that appears once. The database makes that
difference visible and actionable.

**In GRC:**
A living assessment framework applies the same version control
discipline to GRC assessment tools — treating audit checklists,
assessment frameworks, and risk registers as versioned artifacts
that evolve with the environment they govern.

In practice this means:
- Maintaining version history for all assessment tools and
  frameworks
- Establishing triggers for checklist review: new systems deployed,
  new regulations enacted, new threat intelligence received,
  post-incident review completed
- Storing assessment findings in a risk register that allows
  longitudinal pattern analysis — not just point-in-time snapshots
- Treating the risk register as a living document, updated
  continuously rather than refreshed at assessment intervals

**What OHS practice adds:**
Version control on assessment tools is standard practice in software
development and document management but inconsistently applied in
GRC. The OHS model — where the checklist is explicitly versioned,
the version history is maintained, and the triggers for revision
are defined — provides a practical template for living GRC
documentation that most assessment frameworks don't prescribe
explicitly.

---

### Element 5: The ad-hoc finding → Real-time risk assessment

**In OHS:**
When a new hazard is identified during a walkabout — something not
on the checklist, something unexpected — the response is immediate
and structured:

1. Notate the finding on the spot
2. Discuss with the supervisor companion — walk through possible
   scenarios, assess potential fallout, determine risk level
3. Contain immediately if risk is medium to high — cordon off the
   area, stop the process, remove the hazard if possible
4. Develop a list of possible solutions before escalating
5. Bring the finding and solution options to management — present
   constraints alongside options, not just the problem
6. Obtain authorization for the selected treatment
7. Procure and implement the approved remediation
8. Hand off to supervisors for operational implementation

This is a complete risk treatment lifecycle — conducted informally,
in real time, in the environment where the hazard was found.

**In GRC:**
Real-time risk assessment is the capacity to identify, triage, and
initiate treatment for new threats as they emerge — between formal
assessment cycles, without waiting for the next scheduled audit.

In practice this means:
- Defining a clear process for ad-hoc threat identification that
  mirrors the structured response of the OHS walkabout finding
- Establishing risk triage criteria that allow rapid classification
  of new findings as low, medium, or high priority
- Defining immediate containment actions for high-priority findings
  — the GRC equivalent of cordoning off the area
- Maintaining a defined escalation pathway that gets findings to
  the right decision-maker quickly
- Documenting ad-hoc findings in the risk register with the same
  rigor as formally scheduled assessment findings

**What OHS practice adds:**
The structured informality of the OHS ad-hoc finding response —
rigorous enough to produce a complete risk treatment lifecycle,
flexible enough to execute in real time on a factory floor — is
a model for continuous risk management that GRC practice frequently
lacks. Most GRC programs handle scheduled assessments well and
ad-hoc findings inconsistently. The OHS model provides a practical
template for closing that gap.

---

### Element 6: Near misses → Security indicators and precursor events

**In OHS:**
A near miss is an event that could have caused harm but didn't —
through luck, timing, or a control that worked when it needed to.
Near misses are investigated with almost the same rigor as actual
incidents, because they are evidence that the probability exists
and is actively materializing. A workplace that tracks near misses
seriously is a workplace that learns from them before they become
incidents.

**In GRC:**
Security indicators and precursor events are the GRC equivalent
of near misses — signals that a threat event is being attempted
or is in progress, even if it hasn't caused material harm yet.

- Failed login attempts — evidence that credential compromise is
  being attempted
- Caught phishing emails — evidence that social engineering is
  being targeted at the organization
- Anomalous access patterns — evidence that authorized credentials
  may be compromised or misused
- Blocked malware — evidence that malicious code is being delivered
  to the environment

These are not reassuring indicators. They are likelihood data.
They tell you that the probability exists and is materializing —
and that the difference between a near miss and an incident may
be a control that worked once but may not work again.

**What OHS practice adds:**
The cultural discipline of treating near misses as seriously as
incidents — investigating them, documenting them, using them to
calibrate likelihood assessments — is something GRC practice
acknowledges in theory but inconsistently applies. Organizations
that track caught phishing attempts and failed login attempts as
seriously as actual breaches develop a materially more accurate
picture of their likelihood exposure than organizations that treat
these indicators as evidence that their controls are working.

They are not evidence that controls are working. They are evidence
that threat actors are trying — and that the controls have worked
so far.

## The Real-Time Risk Assessment
### Ad-Hoc Finding to Continuous Risk Management

Formal risk assessments operate on a schedule. Reality does not.

New equipment gets deployed between assessment cycles. Workflows
change. Employees develop workarounds. Threat actors don't wait
for the next annual audit before probing for vulnerabilities. The
environment that was assessed six months ago is not the environment
that exists today — and the gap between them is where unmanaged
risk accumulates.

OHS practice developed a solution to this problem not through
formal methodology but through operational necessity. When you're
responsible for safety on an oil rig or a cruise ship, you cannot
wait for the next scheduled assessment to address a hazard you
found this morning. You need a structured, repeatable process for
handling unplanned findings in real time — rigorous enough to
produce defensible risk decisions, flexible enough to execute
in the middle of a working day without stopping everything else.

That process, developed through a decade of daily inspections
across factory floors, oil rigs, and marine environments, is
documented here — and translated into a model for continuous
risk management in GRC.

---

### The OHS real-time finding process

When an unexpected hazard is identified during a routine inspection
— something not on the checklist, something that wasn't there
yesterday — the response follows a consistent sequence:

**Step 1: Notate immediately**
Document the finding on the spot. Location, description, time,
conditions. Don't rely on memory. The documentation starts at
the moment of identification, not after the walkabout is complete.

**Step 2: Rapid collaborative triage**
Discuss the finding with the supervisor companion immediately.
Walk through possible scenarios: what could this hazard cause?
Under what conditions? How likely? How severe? This is a real-time
risk assessment — informal in setting, rigorous in logic. Two
people with different perspectives and different knowledge of the
environment produce a more reliable triage than one person alone.

**Step 3: Immediate containment if warranted**
If the rapid triage produces a medium or high risk determination,
contain immediately. Cordon off the area. Stop the process. Remove
the hazard if possible. Don't wait for management authorization
to implement an interim control — the supervisor companion present
during the inspection has the authority to act, and acting
immediately is the point of having them there.

**Step 4: Solution development before escalation**
Before bringing the finding to management, develop a list of
possible solutions — at least two or three options, with the
constraints of each noted. Budget implications. Time requirements.
Operational disruption. The escalation conversation is more
productive when it presents options rather than problems — giving
decision-makers what they need to make an informed authorization
decision rather than putting them in the position of solving a
problem they've just been handed.

**Step 5: Structured escalation**
Bring the finding, the triage assessment, and the solution options
to the relevant manager. Present constraints alongside options.
Be specific about what each option addresses and what it leaves
unaddressed. Give the decision-maker a clear recommendation while
preserving their authority to choose differently.

**Step 6: Authorization and procurement**
Once a treatment is selected, obtain formal authorization and
initiate procurement of whatever resources are needed. Document
the authorization — who approved what, when, and on what basis.

**Step 7: Operational handoff**
Transfer implementation responsibility to the supervisors with
operational authority over the affected area. Brief them on what
was found, what was decided, and what they need to do. Follow up
to verify implementation.

---

### Why this process works

The OHS real-time finding process works because it resolves the
central tension of ad-hoc risk management: the tension between
the need for immediate action and the need for rigorous process.

It resolves it by separating the process into two phases with
different speeds:

**Phase 1 is fast:** Notate, triage, contain. This happens in
minutes, on the spot, with the people present. It doesn't require
management approval because containment — reducing immediate
exposure — is within the authority of the safety manager and
supervisor companion. Speed here is the point.

**Phase 2 is deliberate:** Solution development, escalation,
authorization, procurement, handoff. This happens at the pace
appropriate to the decision — fast enough to close the gap left
by containment, deliberate enough to produce a good decision
rather than a rushed one.

The interim control — the cordoned area, the stopped process —
buys the time needed for Phase 2 to happen properly. It transforms
an urgent problem into a managed one.

---

### The GRC equivalent: Continuous risk management

In GRC, continuous risk management is the practice of maintaining
risk assessment as an ongoing activity rather than a periodic one
— identifying, triaging, and initiating treatment for new risks
as they emerge, between formal assessment cycles.

The OHS real-time finding process translates directly into a
continuous risk management workflow:

**Step 1: Identification and immediate documentation**
New threat identified — through monitoring alerts, employee report,
vendor notification, threat intelligence feed, or direct observation.
Document immediately: what was identified, when, by whom, under
what circumstances.

**Step 2: Rapid collaborative triage**
Assess the finding against defined triage criteria: threat source
category, affected assets, potential impact, likelihood given
current controls. Involve a second perspective — a peer, a subject
matter expert, a supervisor. Produce a risk classification: low,
medium, or high priority.

**Step 3: Immediate compensating control if warranted**
For medium or high priority findings: implement an interim
compensating control immediately, without waiting for the full
remediation cycle. Block the suspicious IP. Revoke the compromised
credential. Isolate the affected system. Disable the vulnerable
feature. The compensating control buys time for deliberate
remediation — it is the GRC equivalent of cordoning off the area.

**Step 4: Solution development**
Develop remediation options before escalating to decision-makers.
Document the constraints of each option: cost, implementation
time, operational impact, residual risk. Give leadership options,
not just problems.

**Step 5: Escalation and authorization**
Present the finding, triage assessment, compensating control
status, and remediation options to the appropriate decision-maker.
Obtain formal authorization for the selected treatment. Document
the authorization.

**Step 6: Remediation and verification**
Implement the approved remediation. Verify its effectiveness
through observation, not just documentation. Update the risk
register with the finding, the treatment, and the verification
outcome.

**Step 7: Risk register update and pattern analysis**
Add the finding to the risk register. Review whether it reveals
a pattern — is this the third finding of this type in two months?
Does it suggest a gap in the assessment framework that needs to
be addressed? Update the assessment checklist if a new threat
category has been identified.

---

### The two-speed principle in GRC

The same two-speed logic that makes the OHS real-time finding
process effective applies directly to GRC continuous risk
management:

**Fast:** Identification, triage, compensating control.
Minutes to hours. Within the authority of the security or GRC
practitioner. Speed is the point — every hour between identification
and containment is an hour of unmanaged exposure.

**Deliberate:** Solution development, authorization, remediation,
verification. Hours to weeks depending on complexity. Requires
stakeholder involvement and formal authorization. Deliberateness
is the point — a rushed remediation that introduces new
vulnerabilities is worse than a contained risk being managed
carefully.

The compensating control is what makes the two-speed approach
possible. It reduces immediate exposure to a manageable level,
transforming an urgent problem into a managed one — and buying
the time needed for deliberate remediation without leaving the
organization exposed in the interim.

---

### A note on authority and escalation design

The OHS real-time finding process works in part because the
authority to implement immediate containment is built into the
inspection structure itself. The supervisor companion isn't there
just for fresh eyes. They're there because immediate action
sometimes requires immediate authority — and waiting for an
escalation chain to authorize a cordon while a hazard is actively
present defeats the purpose of finding it.

GRC programs should design the same principle into their continuous
risk management process: define clearly who has authority to
implement compensating controls without waiting for full escalation,
and make sure that person is as close to the identification process
as possible.

A security operations center analyst who identifies a suspicious
access pattern should not have to wait three approval layers to
block a compromised credential. The authority to act should be
commensurate with the speed the situation requires.

Define the authority. Document it. Make sure the people who need
it have it before they need it.

## Living Assessment Tools
### Version Control as a Risk Management Discipline

The inspection checklist is never finished. It is always a current
best approximation of what needs to be assessed — subject to revision
as the environment changes.

This is not a minor operational detail. It is a fundamental
methodological principle: an assessment tool that doesn't evolve
with the environment it governs becomes a liability. It creates
false confidence that everything is being checked when the
environment has moved on without the checklist.

In OHS practice, checklist version control is driven by specific
triggers:
- New equipment or systems introduced
- Workflows modified by management
- New hazard categories identified through incident or near miss
  investigation
- Regulatory changes that introduce new requirements

Each version is numbered, dated, and stored. The version history
is maintained — creating an audit trail of how the assessment tool
has evolved alongside the environment it governs.

Inspection findings are entered into a database after each walkabout
— not filed and forgotten, but recorded in a system that makes
patterns visible over time. A hazard that appears three times in
two weeks is a different risk than a hazard that appears once.
Longitudinal pattern analysis turns individual findings into
systemic insight.

**In GRC terms:**
- Treat assessment frameworks and audit checklists as versioned
  documents with defined revision triggers
- Maintain version history for all assessment tools
- Store findings in a risk register that supports longitudinal
  analysis, not just point-in-time snapshots
- Review and update assessment tools after every significant
  environmental change — new systems, new regulations, new threat
  intelligence, post-incident review

A risk register that is updated continuously is a fundamentally
different tool than one that is refreshed at audit intervals.
The first tells you what your risk landscape looks like right now.
The second tells you what it looked like last time someone checked.

---

## Implications for GRC Practice
### What to Do Differently

The argument this document has made is that OHS hazard identification
practice contains methodology that GRC threat identification would
benefit from adopting explicitly. This final section translates
that argument into specific, actionable changes.

These are not additions that require significant extra resources.
They are changes in posture and process that produce materially
more accurate threat identification without materially increasing
assessment scope.

**1. Define and follow a structured scope traversal route**
Before beginning any assessment, define the asset inventory and
establish a consistent order for working through it. Follow that
order every time. Let the route, not your attention, determine
coverage.

**2. Build collaborative observation into the assessment structure**
Involve a second perspective in threat identification — not as
optional peer review after the fact, but as a structural feature
of the assessment itself. Rotate who reviews which domains.
Ensure that fresh eyes are present at every significant assessment
activity.

**3. Design immediate escalation pathways**
Define who has authority to implement compensating controls without
waiting for full escalation. Make sure that person is as close to
the identification process as possible. Document the authority
before it's needed.

**4. Treat near misses as seriously as incidents**
Failed login attempts, caught phishing emails, blocked malware,
and anomalous access patterns are likelihood data — not reassurance.
Investigate them. Document them. Use them to calibrate likelihood
assessments upward from what incident history alone would suggest.

**5. Establish a real-time finding process**
Define a structured, repeatable process for handling unplanned
findings between formal assessment cycles. Fast phase: identify,
triage, contain. Deliberate phase: develop options, escalate,
authorize, remediate, verify. Don't leave ad-hoc findings to
improvisation.

**6. Version control your assessment tools**
Define revision triggers for all assessment frameworks and
checklists. Maintain version history. Update after every significant
environmental change. Treat your assessment tools as living
documents, not static templates.

**7. Enter every finding into a longitudinal record**
A single finding is a data point. Multiple findings over time are
a pattern. Patterns reveal systemic vulnerabilities that point-in-
time assessments miss. Maintain a risk register that supports
longitudinal analysis and review it regularly for emerging patterns.

---

*This document is part of the
[risk-assessment-methodology](../README.md) repository.
Next: [risk-scoring-crosswalk.md] — how OHS likelihood and severity
matrices map to NIST 800-30 likelihood and impact scoring.*
