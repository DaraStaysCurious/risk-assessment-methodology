> **Status: Draft v1 — in progress.** This document is currently being
> condensed. Full methodology content is being distributed across
> individual documents in this repository. This overview will be
> updated once all individual documents are complete.

---

# Methodology Overview
## OHS Risk Assessment Practice as a Foundation for GRC

---

## Introduction

This document makes a single argument:

Occupational Health and Safety risk assessment and Governance, Risk,
and Compliance risk assessment are the same discipline with different
vocabulary. And both are made more effective — or fail entirely —
based on how well they account for human behavior.

That argument is not theoretical. It's drawn from a decade of
conducting workplace risk assessments — standing on factory floors,
interviewing machine operators and welders, investigating near misses,
and figuring out why controls that looked perfect on paper kept failing
in practice. Then translating that experience into GRC methodology and
discovering that the translation was almost entirely one-to-one.

This document is the record of that translation.

---

### How to use this document

If you're a **GRC analyst**, read this document as a methodology
supplement — a way of thinking about risk assessment that makes NIST
800-30 and ISO 27005 more effective when you apply them. The framework
tells you what to do. This document tells you how to think while
you're doing it.

If you're an **OHS professional considering a transition into GRC**,
read this document as a bridge. Everything you know about risk
assessment translates. The vocabulary changes. The underlying logic
doesn't. This document shows you exactly where your existing skills
map to GRC practice — and where the field needs what you already know.

If you're a **UX designer or researcher transitioning into GRC or
cybersecurity**, read this document as proof of concept. The research
skills, systems thinking, and human behavior expertise you've built
in design practice are not adjacent to GRC — they're directly
applicable to it. This document shows you exactly where your existing
lens maps onto risk assessment methodology, and why the field needs
it.

If you're a **UX designer or researcher working on secure-by-design
projects**, read this document as a methodology bridge. Understanding
how GRC analysts think about risk, threat, and control design will
make your secure-by-design work more rigorous — and understanding how
design thinking can inform control design will make you a more
effective collaborator with the security teams you work alongside.

If you're a **security researcher or practitioner** interested in
human factors and usable security, read this document as a case study
in what GRC practice looks like when it's built on a human-systems
foundation rather than a framework-compliance foundation.

---

### How this repository is organized

| Document | What it covers |
|----------|---------------|
| `methodology-overview.md` | The complete methodology: OHS and GRC compared — *this document* |
| [`hazard-identification-to-threat-modeling.md`](hazard-identification-to-threat-modeling.md) | OHS hazard ID → GRC threat identification |
| `risk-scoring-crosswalk.md` | OHS likelihood/severity → NIST 800-30 likelihood/impact — *coming soon* |
| `corrective-action-to-remediation.md` | OHS corrective action → GRC remediation roadmaps — *coming soon* |
| `human-factors-in-risk.md` | Where OHS and GRC most powerfully converge — *coming soon* |
| `applications.md` | How this methodology is applied across the portfolio — *coming soon* |

---

### A note on framework vs. methodology

NIST 800-30 is a framework. ISO 27005 is a framework. Frameworks tell
you *what* to assess and *what to produce*. They are essential —
they provide structure, defensibility, and a common language across
the industry.

But frameworks don't tell you how to think. They don't tell you what
to listen for when an employee says "the machine works fine without
the guard." They don't tell you how to distinguish between resistance
that signals a control design problem and resistance that signals
convenience avoidance. They don't tell you what to do when the right
control and the available budget are not the same number.

Methodology fills that gap. It's the thinking that happens inside the
framework — the judgment, the diagnostic listening, the human factors
awareness that determines whether a technically correct risk assessment
produces controls that actually work in practice.

This document is a methodology. It's designed to be used alongside
frameworks, not instead of them.

---

## The Two Disciplines

Before mapping one to the other, it helps to understand what each
discipline is trying to do at its core — stripped of framework
language and industry jargon.

---

### Occupational Health & Safety Risk Assessment

OHS risk assessment exists to answer one question:

**What could hurt someone here, and what are we going to do about it?**

In practice this means:
- Identifying the conditions, equipment, materials, and human behaviors
  present in a work environment
- Determining which of those elements could cause harm, and under what
  circumstances
- Estimating how likely that harm is to occur, and how severe it would
  be if it did
- Selecting and implementing controls to reduce that likelihood or
  severity to an acceptable level
- Monitoring those controls over time to make sure they continue to
  work as intended

The stakes in OHS are immediate and physical. A missed hazard can
result in injury, disability, or death. Controls that fail in practice
— not just on paper — have direct consequences for real people.

This creates a discipline that is, by necessity, grounded in how
humans actually behave inside systems. You cannot conduct a credible
OHS risk assessment from behind a desk. You have to go where the work
happens, watch how it's done, and talk to the people doing it —
because the gap between how a task is supposed to be performed and how
it's actually performed is almost always where the risk lives.

---

### GRC Risk Assessment

GRC risk assessment exists to answer a parallel question:

**What could harm this organization's information assets, and what are
we going to do about it?**

In practice this means:
- Identifying the systems, data, processes, and human behaviors present
  in an organization's information environment
- Determining which of those elements could cause harm — data breach,
  system failure, regulatory penalty, reputational damage — and under
  what circumstances
- Estimating how likely that harm is to occur, and how severe it would
  be if it did
- Selecting and implementing controls to reduce that likelihood or
  severity to an acceptable level
- Monitoring those controls over time to make sure they continue to
  work as intended

The stakes in GRC are less immediately physical but no less real. A
missed vulnerability can result in data breach, regulatory fine, loss
of customer trust, or business disruption. Controls that exist on
paper but fail in practice leave organizations exposed — often without
knowing it.

---

### The Parallel

Read those two descriptions again side by side.

The question is the same. The process is the same. The failure mode
is the same — controls that look correct on paper but fail in
practice. The success condition is the same — controls that work
because they were designed around how people actually behave, not how
we wish they would.

The difference is the domain. In OHS the asset being protected is the
human body. In GRC the asset being protected is information. Everything
else — the methodology, the thinking, the judgment calls, the
stakeholder dynamics — is functionally identical.

This is not a metaphor. It is a structural parallel. And the
implications for how GRC risk assessments should be conducted are
significant — which is what the rest of this document explores.

---

### A word on vocabulary

One of the biggest barriers for OHS professionals moving into GRC —
and for GRC professionals trying to understand human factors research
— is vocabulary. The two fields use different words for the same
concepts, which makes them look more different than they are.

Throughout this document, OHS terms and GRC terms will be presented
side by side wherever they refer to the same underlying concept. By
the end of this document you should be able to move fluidly between
both vocabularies — which is itself a professional asset in a field
that increasingly needs practitioners who can bridge human factors
and technical security.

---

## The Complete Mapping
### OHS Risk Assessment Practice → NIST 800-30

NIST Special Publication 800-30, "Guide for Conducting Risk
Assessments," is one of the foundational documents in GRC risk
management. It defines a four-step risk assessment process:

1. Prepare for the Assessment
2. Conduct the Assessment
3. Communicate Results
4. Maintain the Assessment

What follows is a complete mapping of OHS risk assessment practice
onto those four steps — showing not just that the steps correspond,
but how the thinking, judgment, and human factors awareness developed
in OHS practice enriches each step of the GRC process.

---

### Step 1: Prepare for the Assessment

**In NIST 800-30:**
Before conducting a risk assessment, establish the context. Define the
purpose of the assessment, the scope of what's being assessed, the
assumptions and constraints that apply, and the sources of information
that will inform the assessment. Identify applicable laws, regulations,
and organizational policies.

**In OHS practice:**
Before touching anything, establish why this assessment is happening.
Ask: what brought this task to my desk? Did something happen? Did
something almost happen? Is someone afraid or alarmed by something
about this task? Then identify which legislation and company policies
apply to the task being assessed.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| "What brought this to my desk?" | Purpose of the assessment |
| Defining which task is being assessed | Scope definition |
| "Did something happen / almost happen?" | Information sources — prior incidents |
| Legislation and policy research | Applicable laws and organizational policies |

**What OHS practice adds:**
NIST 800-30 defines preparation as a documentation and scoping
exercise. OHS practice adds a diagnostic front end — the assessment
begins not with paperwork but with a conversation about what prompted
the assessment in the first place. That conversation establishes
context that no document can provide: the organizational history,
the interpersonal dynamics, the unspoken concerns that sit behind
the formal request.

In GRC terms: before you open a framework document, find out why
you're really there.

---

### Step 2a: Identify Threat Sources and Threat Events

**In NIST 800-30:**
Identify threat sources — anything with the potential to trigger a
threat event. Identify threat events — the specific ways those sources
could cause harm to the system or organization being assessed.

**GRC vocabulary:**
- Threat source — a person, condition, or situation with the potential
  to cause harm (a malicious actor, a misconfigured system, a
  disgruntled employee, a natural disaster)
- Threat event — the specific way that source causes harm (a phishing
  attack that compromises credentials, a misconfiguration that exposes
  data, an insider who exfiltrates intellectual property)

**In OHS practice:**
Go observe the task quietly, taking notes. Then ask the employees
performing the task to walk through it step by step, talking aloud
about what they're doing at each step and why. Encourage them to be
as critical as possible — to name every pain point and frustration
as they experience it. Capture anonymized quotes.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Quiet observation of the task | Threat source identification — conditions and equipment |
| Employee task walkthrough | Threat event identification — how things could go wrong |
| Pain points and frustrations captured | Predisposing conditions — factors that increase likelihood |
| Anonymized quotes documented | Evidence collection for risk assessment record |

**What OHS practice adds:**
NIST 800-30 identifies threat sources and events primarily through
documentation review and technical analysis. OHS practice adds
direct observation and structured employee interviews as primary
identification methods — because the most significant threats are
often invisible in documentation but immediately visible to the
people performing the task every day.

The employee who says "this step always feels unstable" is handing
you a threat event. The equipment that "makes a weird noise sometimes"
is a threat source. Neither of these appears in a system diagram or
a policy document. They appear in conversations — if you know how
to have them.

---

### Step 2b: Identify Vulnerabilities and Predisposing Conditions

**In NIST 800-30:**
Identify vulnerabilities — weaknesses in the system that could be
exploited by a threat source. Identify predisposing conditions —
characteristics of the environment that increase the likelihood of
a threat event occurring.

**GRC vocabulary:**
- Vulnerability — an unpatched system, a weak password policy, an
  untrained employee, a misconfigured access control
- Predisposing condition — deadline pressure that causes security
  steps to be skipped, understaffing that leaves tickets unresolved,
  a culture that treats security as an obstacle rather than a practice

**In OHS practice:**
Through observation and employee interviews, identify the specific
conditions that create risk — missing guards, incorrect storage,
inadequate training, environmental factors like noise or fatigue
that increase error rates. Document both the physical vulnerabilities
and the organizational conditions that allow them to persist.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Missing guards, incorrect storage, inadequate training | Vulnerabilities |
| Noise, fatigue, production pressure | Predisposing conditions |
| "This step is always rushed" | Predisposing condition — time pressure |
| "We haven't had training on this in two years" | Vulnerability — inadequate awareness |

**What OHS practice adds:**
OHS practice makes predisposing conditions — particularly
organizational and human factors — a primary focus of vulnerability
identification. GRC assessments frequently identify technical
vulnerabilities thoroughly while underweighting the organizational
conditions that allow those vulnerabilities to persist or that
prevent controls from being implemented effectively.

A vulnerability exists in a context. That context determines whether
the vulnerability will be exploited, whether the control will be
accepted, and whether the remediation will stick. OHS practice treats
context as data. GRC practice should do the same.

---

### Step 2c: Determine Likelihood

**In NIST 800-30:**
Determine the likelihood that a threat event will occur, given the
identified threat sources, vulnerabilities, and predisposing
conditions. NIST uses a five-point scale: Very Low, Low, Moderate,
High, Very High. Likelihood is informed by threat source
characteristics, vulnerability severity, existing controls, and
historical data.

**In OHS practice:**
Determine how probable it is that a hazard will result in harm.
Draw on prior incidents, near misses, employee historical knowledge,
and observation of actual task performance. Weight recent incidents
more heavily than distant ones. Treat near misses as high-signal
likelihood indicators — they are evidence that the probability is
materializing, even if harm hasn't occurred yet.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Prior incidents | Historical threat data |
| Near misses | Indicators — likelihood signals |
| Employee historical knowledge | Threat intelligence — domain expertise |
| Observation of actual task performance | Current state assessment |
| "Nothing has happened yet" | Absence of incident ≠ absence of risk |

**What OHS practice adds:**
The treatment of near misses as high-signal likelihood data is one
of the most important contributions OHS practice makes to GRC
methodology. In OHS, a near miss is investigated with almost the
same rigor as an actual incident — because it is evidence that the
probability exists and is materializing.

In GRC, the equivalent of a near miss is a failed login attempt, an
anomalous access pattern, a phishing email that was caught by a
filter rather than a human. These are indicators — signals that a
threat event is being attempted, even if it hasn't succeeded yet.
They should inform likelihood assessment with the same weight that
near misses carry in OHS.

The other critical contribution: the explicit rejection of "nothing
has happened yet" as evidence of low likelihood. Absence of incident
is evidence of luck, not safety. This distinction — between the
absence of harm and the absence of risk — is one of the most
important judgment calls in risk assessment, in any field.

---

### Step 2d: Determine Impact

**In NIST 800-30:**
Determine the impact if the threat event occurs — the harm to the
organization in terms of loss of confidentiality, integrity, or
availability of information assets. NIST uses the same five-point
scale. Impact is assessed across multiple dimensions: financial,
reputational, operational, legal and regulatory.

**In OHS practice:**
Determine the severity of harm if the hazard materializes — ranging
from minor injury requiring first aid through permanent disability
to fatality. Consider both the immediate physical harm and the
organizational consequences: workers' compensation liability,
regulatory penalties, reputational damage, operational disruption.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Minor injury | Very Low impact |
| Lost time injury | Low — Moderate impact |
| Permanent disability | High impact |
| Fatality | Very High impact |
| Regulatory penalty (OSHA) | Legal and regulatory impact |
| Reputational damage | Reputational impact |
| Operational disruption | Availability impact |

**What OHS practice adds:**
OHS impact assessment is anchored in physical harm to human beings
— which creates an inherent clarity about what matters most. When
the worst case is death, impact prioritization is unambiguous.

GRC impact assessment operates across more abstract dimensions —
data confidentiality, system availability, regulatory compliance —
which can make prioritization feel less urgent than it should be.
OHS practice is a useful corrective: it trains risk assessors to
think concretely about the worst case, to name it plainly, and to
let that clarity drive prioritization decisions.

---

### Step 3: Communicate Results

**In NIST 800-30:**
Document and communicate the findings of the risk assessment to
relevant stakeholders. Produce a risk assessment report that includes
identified threats and vulnerabilities, likelihood and impact ratings,
and recommended risk responses. Tailor communication to the audience
— technical findings for technical teams, business impact framing
for leadership.

**In OHS practice:**
Present findings to employees and supervisors. Discuss pain points
and potential controls collaboratively with the people who will have
to implement and live with them. Seek employee input on at least
two to three possible solutions before selecting a control. Review
and update the relevant Standard Operating Procedure. Obtain
supervisor approval. Conduct employee sign-off to document awareness
and understanding.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Findings discussion with employees | Stakeholder communication — operational level |
| Collaborative control identification | Risk response development |
| Supervisor approval | Risk treatment authorization |
| SOP review and update | Policy and procedure development |
| Employee sign-off | Control acknowledgment and awareness documentation |
| Tailoring language for supervisors vs. employees | Audience-appropriate communication |

**What OHS practice adds:**
This is where OHS practice diverges most significantly from standard
GRC practice — and where it has the most to contribute.

NIST 800-30 treats communication as a documentation and reporting
exercise. OHS practice treats it as a collaborative design process.
Controls are not selected by the assessor and handed down to the
people who must implement them. They are developed in dialogue with
those people — because the people closest to the risk have contextual
knowledge the assessor doesn't have, and because controls designed
without user input get routed around.

This is not a soft preference. It is a practical observation backed
by experience: the welding blind stored three floors below where the
work happens will be replaced by cardboard. The password policy
employees had no input on will be written on a sticky note. The
security awareness training nobody was consulted about will be
clicked through in four minutes.

Co-design is not optional. It is the difference between a control
that exists and a control that works.

---

### Step 4: Maintain the Assessment

**In NIST 800-30:**
Risk assessments are not one-time events. Monitor implemented controls
for effectiveness over time. Update the assessment when significant
changes occur — new systems, new threats, organizational changes,
security incidents. Establish a review cadence appropriate to the
risk environment.

**In OHS practice:**
After implementing a control, monitor employees performing the
modified task for a defined period — typically one to two weeks —
to verify that the change has been adopted in practice, not just
acknowledged on paper. Follow up to identify whether the control
is creating new friction or unintended consequences. Revisit the
assessment if conditions change or incidents occur.

**The mapping:**

| OHS practice | NIST 800-30 |
|--------------|-------------|
| Post-implementation monitoring period | Control effectiveness monitoring |
| Watching for workaround behavior | Control failure detection |
| Following up on friction and unintended consequences | Continuous improvement |
| Revisiting on incident or condition change | Assessment maintenance triggers |

**What OHS practice adds:**
The specific practice of a defined post-implementation monitoring
period — physically going back to observe whether the control is
working as intended — is something GRC practice frequently skips.
Controls get implemented, documented, and checked off. Whether they
work in practice is often not verified until the next audit cycle,
or until an incident occurs.

OHS practice treats the post-implementation period as part of the
assessment itself, not as a separate activity. The assessment isn't
complete until you've seen the control working in the environment
where the risk lives — with the people who have to use it, under
the conditions they actually work in.

In GRC terms: a control isn't implemented until it's been observed
working. Documentation is not evidence of effectiveness. Behavior is.

---

## Where They Diverge

The mapping between OHS and GRC risk assessment is strong — but it
is not perfect. There are meaningful differences between the two
disciplines that are worth naming honestly, both because they matter
for practitioners moving between fields and because they reveal where
each discipline has something genuine to learn from the other.

---

### 1. The nature of the asset being protected

In OHS, the asset is the human body. It is tangible, irreplaceable,
and the harm that can come to it is immediate and visible. A fatality
is unambiguous. An injury is undeniable. This creates a clarity of
purpose that cuts through organizational politics, budget debates,
and risk appetite negotiations in a way that abstract harm rarely
can.

In GRC, the assets are information, systems, and organizational
reputation. The harm that can come to them is frequently delayed,
distributed, and difficult to attribute directly to a specific control
failure. A data breach may not be discovered for months. Its full
impact — regulatory penalty, customer attrition, reputational damage
— may take years to materialize fully.

This difference has practical consequences. In OHS it is easier to
make the case for a control because the worst case is viscerally
imaginable. In GRC the worst case is often abstract enough that
leadership can rationalize accepting more risk than they should.

OHS practitioners moving into GRC should be aware of this dynamic
— and should develop the ability to make abstract harm concrete for
non-technical stakeholders. The skill of translating risk into human
terms, developed in OHS, is directly applicable here.

---

### 2. The scale and complexity of the threat landscape

In OHS, threat sources are primarily physical and environmental —
equipment, materials, conditions, and human behavior within a defined
physical space. The threat landscape is bounded. A factory floor has
finite hazards that can be systematically identified and assessed.

In GRC, the threat landscape is significantly more complex and less
bounded. Threat sources include malicious external actors with
sophisticated capabilities, insider threats, supply chain
vulnerabilities, zero-day exploits, and the entire surface area of
an organization's digital infrastructure — which may span multiple
cloud environments, third-party integrations, remote workforces, and
legacy systems simultaneously.

This complexity means GRC risk assessment requires a broader threat
intelligence function than OHS — staying current on the evolving
threat landscape, understanding attacker motivations and
capabilities, and assessing risk against a threat environment that
is actively and intelligently adapting to defenses.

OHS practitioners moving into GRC need to expand their threat
identification practice beyond observable physical conditions to
include this dynamic, intelligence-driven threat landscape.

---

### 3. The regulatory environment

Both OHS and GRC operate within regulatory frameworks — OSHA in
occupational safety, and a complex landscape of frameworks and
regulations in GRC (NIST, ISO, SOC 2, HIPAA, GDPR, PCI DSS, and
others depending on industry and jurisdiction).

The difference is in complexity and overlap. OSHA provides a
relatively unified regulatory framework for workplace safety in the
United States. GRC operates across a fragmented landscape of
overlapping frameworks, each with different requirements, different
audit mechanisms, and different consequences for non-compliance —
often simultaneously within a single organization.

Managing multi-framework compliance — understanding where frameworks
overlap, where they conflict, and how to build a unified control set
that satisfies multiple requirements without duplicating effort — is
a GRC-specific skill that has no direct OHS equivalent. It requires
a different kind of systems thinking: not the systems thinking of
how humans behave inside processes, but the systems thinking of how
regulatory requirements interact across a compliance landscape.

---

### 4. The pace of change

Workplace hazards change — new equipment gets introduced, processes
get modified, new materials get used. But the rate of change in a
physical work environment is generally manageable and observable.

The GRC threat landscape changes at a fundamentally different pace.
New vulnerabilities are discovered daily. Threat actors adapt their
techniques continuously. Regulatory requirements evolve. Cloud
infrastructure changes with every deployment. A risk assessment that
was accurate six months ago may be materially incomplete today.

This requires GRC practitioners to maintain a continuous assessment
mindset rather than a periodic assessment mindset — building
monitoring, detection, and response capabilities that can identify
emerging risks between formal assessment cycles.

---

### What this means in practice

These divergences are real and should not be minimized. GRC is a
more complex threat environment than OHS, operating at greater scale,
with a more dynamic threat landscape, across a more fragmented
regulatory environment, and with assets whose harm is frequently
less immediately visible.

But none of these differences invalidate the methodological parallel.
They extend it. The core discipline — identify what could cause harm,
assess how likely and severe that harm would be, design controls that
work in the environment where humans actually operate, monitor those
controls over time — is the same in both fields.

The OHS practitioner moving into GRC doesn't need to start over.
They need to expand — adding threat intelligence, multi-framework
fluency, and a continuous assessment mindset to a methodological
foundation that is already solid.

---

## The Missing Layer
### What GRC Can Learn from OHS Practice

The mapping in Section 3 shows that OHS and GRC risk assessment are
structurally parallel. The divergences in Section 4 show where GRC
operates at greater complexity than OHS. This section argues something
different:

There is a layer of practice that OHS has developed over decades —
through hard experience on factory floors, in incident investigations,
and in the difficult conversations between safety managers and
production supervisors — that GRC has not yet fully integrated.

That layer is human factors methodology.

Not human factors as a concept. GRC acknowledges human factors. Every
security awareness training program, every acceptable use policy,
every phishing simulation is an acknowledgment that humans are a
risk variable.

But acknowledgment is not methodology. Knowing that humans introduce
risk is different from having a systematic, practiced approach to
understanding how specific humans behave inside specific systems —
and designing controls around that behavior rather than around
idealized behavior that doesn't exist in practice.

OHS has that methodology. GRC largely does not. And the consequences
are visible everywhere in security practice.

---

### What human factors methodology actually means in practice

It means starting every risk assessment with the assumption that the
humans inside the system are rational actors making reasonable
decisions given the constraints and incentives they face — not
irrational actors who need to be trained into compliance.

The welder who used cardboard instead of a welding blind was not
being reckless. They were solving a real problem — the welding blind
was stored three floors below where the work was being done — in the
most efficient way available to them. The solution to that problem
was not retraining the welder. It was building a storage closet on
the correct floor.

The employee who writes their password on a sticky note is not being
careless. They are responding rationally to a password policy so
complex that memorization is genuinely difficult — and the
consequences of being locked out of their system feel more immediate
than the abstract risk of a credential compromise. The solution to
that problem is not another security awareness training. It is a
password policy designed around how human memory actually works.

**This is the core of human factors methodology: treat control failure
as a design problem, not a compliance problem.**

When a control fails in practice — when people route around it,
ignore it, or find workarounds — the first question should not be
"how do we enforce compliance?" It should be "what does this failure
tell us about the design of the control?"

---

### The five human factors principles OHS practice taught me

These are not derived from a textbook. They are observations from a
decade of conducting risk assessments with real people in real
environments — and they apply with equal force in GRC contexts.

---

**Principle 1: The people closest to the risk know the most about it**

In every risk assessment I conducted, the employees performing the
task had more accurate, more detailed, and more practically useful
knowledge about the risk than any document, policy, or outside expert
— including me. They lived with the risk every day. They had
developed an intimate understanding of where it was likely to
materialize, under what conditions, and what made it better or worse.

That knowledge is not automatically offered. It has to be drawn out
through deliberate, structured conversation — with questions designed
to elicit critical thinking rather than reassurance, and with enough
psychological safety that people feel comfortable naming problems
rather than defending the status quo.

In GRC terms: the employees who use the systems you're assessing
know more about how those systems actually work — and where they
actually break down — than any technical audit will reveal. Talk
to them. Listen diagnostically. Treat what they tell you as primary
evidence, not anecdote.

---

**Principle 2: Resistance is data**

When employees pushed back on a control I proposed, my first instinct
was never to override the resistance. It was to understand it.

Resistance falls into two categories. The first is convenience
resistance — pushback rooted in friction, inconvenience, or the
disruption of established habit. This tells you something about the
design of the control: it may be creating more friction than
necessary, and friction is a control killer.

The second is substantive resistance — pushback that contains real
information about the risk, the environment, or the feasibility of
the proposed control. This tells you something about your risk
assessment: there is contextual knowledge in the room that your
assessment hasn't captured yet.

The signals that distinguish them:
- Convenience resistance sounds like: "who has time for this," "this
  will slow me down," impatient tone, rushing to end the conversation
- Substantive resistance sounds like: "the machine works fine without
  the guard," "I haven't gotten hurt doing this before" — statements
  that contain a theory about the risk that deserves examination

Both types of resistance deserve a response. Convenience resistance
tells you to examine the friction cost of your control design.
Substantive resistance tells you to steelman the objection — to find
the strongest possible version of the argument and examine it
seriously before dismissing it.

In GRC terms: when employees push back on security controls, listen
before you enforce. The resistance may be telling you something your
risk assessment missed.

---

**Principle 3: Friction kills controls**

A control that requires significant extra effort from the people who
must use it will be routed around. Not occasionally. Reliably.

This is not a statement about human laziness or carelessness. It is
a statement about rational behavior under real-world constraints.
People operating under time pressure, cognitive load, and competing
priorities will consistently choose the path of least resistance —
and if that path bypasses your control, your control will fail.

The practical implication: control design must account for the
friction cost of implementation. A technically correct control with
high friction cost will consistently underperform a technically
imperfect control with low friction cost.

The goal is not to eliminate friction entirely — some friction is
appropriate and intentional, functioning as a speed bump that prompts
deliberate decision-making. The goal is to ensure that the friction
cost of the correct behavior is always lower than the friction cost
of the workaround.

In GRC terms: before finalizing any control recommendation, ask —
what is the easiest way for someone to not do this? Then design the
control so that doing it correctly is easier than not doing it.

---

**Principle 4: Absence of incident is not evidence of absence of risk**

"I haven't gotten hurt doing this before" is one of the most
dangerous statements in risk management.

It conflates two things that are not the same: the probability that
harm will occur, and whether harm has occurred yet. A hazard that
hasn't caused injury in two years is not a safe hazard. It is a
hazard whose probability hasn't materialized yet — which is a
different thing entirely.

This cognitive pattern — called normalcy bias — is one of the most
reliable failure modes in risk assessment across every domain. It
is the reason organizations are consistently surprised by incidents
that, in retrospect, were entirely predictable. The signals were
there. The near misses were there. But the absence of a major
incident created a false sense of security that suppressed action.

In GRC terms: "we've never been breached" is not a risk assessment.
It is an absence of evidence being mistaken for evidence of absence.
Near misses, failed login attempts, anomalous access patterns, and
caught phishing emails are not reassuring indicators. They are
likelihood data — signals that the probability exists and is
actively materializing.

---

**Principle 5: Co-design produces better controls than top-down design**

In my experience, controls developed collaboratively with the people
who must implement and live with them were more effective, more
durable, and more practically intelligent than controls I developed
independently and handed down for implementation.

This is not a surprising finding. The people performing the task
have contextual knowledge I don't have. They know the environmental
constraints, the workflow pressures, the equipment quirks, and the
organizational dynamics that determine whether a control will work
in practice. That knowledge produces better control design when it's
incorporated — and produces workarounds when it's ignored.

The co-design process also serves a second function: it creates
ownership. People are more likely to comply with controls they
helped design — not because of psychological manipulation, but
because the controls are more likely to actually fit the reality
they work in.

The practical process:
1. Present the risk and its assessment — share what you found and
   why it matters, in plain language
2. Ask for input before proposing solutions — what do they think
   should be done? What have they tried before? What do they know
   about this risk that you don't?
3. Propose options, not mandates — present two or three possible
   controls and discuss tradeoffs openly
4. Listen for the kernel of truth in resistance — even objections
   rooted in convenience often contain real information about
   feasibility or friction
5. Document the conversation — who was involved, what was discussed,
   what was decided, and why

In GRC terms: security controls designed with end users are more
effective than security controls designed for end users. This is
not a principle unique to OHS — it is foundational to UX research,
human factors engineering, and usable security research. It is
simply underimplemented in standard GRC practice.

---

### Why this layer is missing from GRC

GRC developed primarily as a technical and legal discipline — focused
on framework compliance, audit readiness, and the documentation of
controls. The question it was built to answer is "are we compliant?"
not "do our controls actually work?"

That framing produces a discipline that is very good at producing
evidence of compliance and not always as good at producing security
that works in practice. Controls get designed, documented, and
audited. Whether they work in the environments where humans actually
operate — whether people use them, route around them, or find
workarounds that introduce new risks — is frequently outside the
scope of the formal assessment.

OHS never had that luxury. A workplace safety control that looks
correct on paper but fails in practice has immediate, visible
consequences. The discipline was forced, by the nature of its
stakes, to develop methodology for understanding how humans actually
behave inside systems — not how they're supposed to behave.

That methodology is what this document is proposing GRC adopt —
not as a replacement for technical rigor, but as a layer underneath
it. The technical assessment tells you what the vulnerabilities are.
The human factors layer tells you whether the controls you design
to address them will actually work.

Both are necessary. Currently, GRC practice does one well and the
other inconsistently.

---

## Implications for GRC Practice
### What This Methodology Looks Like in Action

The argument this document has made is structural and theoretical.
This final section makes it practical — translating the methodology
into specific changes to how GRC risk assessments are conducted,
from scoping through control implementation and monitoring.

These are not additions to standard GRC practice that require
significant extra time or resources. They are adjustments to how
existing steps are approached — changes in posture, questioning
technique, and interpretive framework that produce materially better
risk assessments without materially increasing assessment scope.

---

### 1. Start every assessment with a diagnostic conversation

Before opening a framework document, before reviewing system
architecture diagrams, before touching a single policy — have a
conversation with the person who requested the assessment.

Ask:
- What brought this assessment to the table right now?
- Has something happened, or almost happened?
- What are you most worried about that you haven't been able to
  articulate formally yet?
- What have previous assessments missed?

This conversation establishes context that no document can provide.
It surfaces the organizational history, the interpersonal dynamics,
and the unspoken concerns that sit behind the formal request — and
it calibrates the entire assessment before a single framework
requirement has been reviewed.

In NIST 800-30 terms: this is preparation. In practice, it is
frequently skipped in favor of jumping directly to scope definition
and documentation review. Don't skip it.

---

### 2. Conduct structured interviews with the people inside the system

After the diagnostic conversation with the requestor, before
conducting technical assessment, interview the people who use the
systems being assessed.

Not a survey. Not a questionnaire. A conversation — structured
enough to cover the necessary ground, open enough to surface what
you don't know to ask about.

Ask them to walk you through what they actually do — not what the
policy says they should do, but what they actually do. Ask them
where the process feels slow, confusing, or frustrating. Ask them
what workarounds they've developed. Ask them what they'd fix if
they could fix anything.

Document what they tell you. Treat it as primary evidence. The gap
between documented procedure and actual practice is almost always
where the most significant vulnerabilities live.

---

### 3. Treat resistance as diagnostic data

When people push back on findings or proposed controls during an
assessment, resist the instinct to override or dismiss the
resistance. Instead, classify it:

**Is this convenience resistance?**
- Does it sound like friction avoidance — "this will slow us down,"
  "nobody has time for this," impatience or disengagement?
- If so: examine the friction cost of the proposed control. Is there
  a lower-friction alternative that achieves the same risk reduction?
  Friction is a control killer — a technically correct control with
  high friction cost will consistently underperform.

**Is this substantive resistance?**
- Does it contain a theory about the risk — "we've never had a
  problem with this," "that's not how this system actually works,"
  "that control won't work here because..."?
- If so: steelman the objection. Find the strongest possible version
  of the argument and examine it seriously. There may be contextual
  knowledge in the room that your assessment hasn't captured yet.

Both types of resistance contain information. Neither should be
dismissed without examination.

---

### 4. Design controls collaboratively

Before finalizing any control recommendation, bring proposed controls
back to the people who will implement and live with them. Present
the risk and its assessment in plain language. Ask for input before
proposing solutions. Present options rather than mandates. Listen
for the kernel of truth in objections.

This is not a soft preference or a courtesy. It is a practical
methodology for producing controls that work in practice rather than
on paper — because the people closest to the risk have contextual
knowledge that produces better control design when it's incorporated,
and produces workarounds when it's ignored.

The co-design process does not require consensus. There will be
situations where the correct control is non-negotiable regardless
of employee preference — and those situations should be handled
directly and honestly. But even in those cases, the conversation
produces better implementation: people who understand why a control
exists are more likely to comply with it than people who received
it as a mandate.

---

### 5. Assess friction before finalizing recommendations

Before any control recommendation is finalized, ask:

**What is the easiest way for someone to not do this?**

Then examine whether that path is easier than doing it correctly.
If it is — if the workaround is genuinely more convenient than
compliance — the control will fail in practice regardless of how
technically correct it is.

The goal is not to eliminate all friction. Some friction is
intentional — a deliberate speed bump that prompts conscious
decision-making before a consequential action. The goal is to ensure
that the friction cost of correct behavior is always lower than the
friction cost of the workaround.

Where high friction is unavoidable, document it explicitly in the
risk assessment. Note that the control's effectiveness depends on
sustained compliance with a high-friction requirement, and recommend
compensating monitoring controls that can detect when workarounds
are occurring.

---

### 6. Treat near misses as high-signal likelihood data

In the assessment of likelihood, weight near misses — failed attacks,
caught phishing attempts, anomalous access patterns, security
incidents that were contained before causing material harm — with
the same rigor applied to actual incidents.

A near miss is not a reassuring indicator. It is evidence that the
probability exists and is actively materializing. The difference
between a near miss and an incident is frequently luck, timing, or
a control that worked once but may not work again.

Document near misses in the risk assessment record. Use them to
calibrate likelihood ratings upward from what a purely incident-based
analysis would suggest. And resist the organizational pressure to
treat "nothing bad actually happened" as evidence that the risk
is under control.

---

### 7. Verify control effectiveness through observation, not just documentation

After controls are implemented, verify their effectiveness through
direct observation — not just through documentation review or
self-reported compliance.

This does not require a formal audit. It requires going to where
the work happens and watching whether the control is being used
as intended. Are people following the new procedure? Is the
authentication step being completed or bypassed? Is the documented
process what actually happens?

A control isn't implemented until it's been observed working in
the environment where the risk lives — with the people who have
to use it, under the conditions they actually work in.

Documentation is not evidence of effectiveness. Behavior is.

---

### Putting it together: what this methodology looks like end to end

A risk assessment conducted with this methodology follows the
standard NIST 800-30 structure — prepare, assess, communicate,
maintain — with the following additions at each stage:

**Prepare:**
- Diagnostic conversation with the requestor before any documentation
  review
- Identification of prior incidents AND near misses as primary
  likelihood inputs
- Structured interviews with system users before technical assessment

**Assess:**
- Threat and vulnerability identification informed by user interviews,
  not just technical analysis
- Predisposing conditions assessed explicitly — organizational
  pressures, workflow constraints, cultural factors that affect
  control effectiveness
- Likelihood calibrated against near miss data, not just incident
  history
- Impact assessed in concrete, human terms wherever possible

**Communicate:**
- Findings presented in plain language to the people affected,
  not just to leadership
- Control recommendations developed collaboratively with end users
- Options presented rather than mandates where feasible
- Resistance treated as diagnostic data throughout

**Maintain:**
- Post-implementation observation period to verify behavioral
  adoption, not just documentation compliance
- Near misses tracked and weighted in ongoing likelihood assessment
- Control friction monitored as an ongoing effectiveness indicator

---

### A final note

This methodology does not make GRC risk assessment softer or less
rigorous. It makes it more accurate — because it accounts for the
full range of variables that determine whether a security program
works in practice, not just on paper.

The technical assessment tells you what the vulnerabilities are.
The human factors layer tells you whether the controls you design
to address them will actually be used.

Both matter. A vulnerability with no control is a risk. A control
that nobody uses is also a risk — it's just a risk that looks
mitigated on paper.

The goal of risk assessment is not compliant documentation. It is
actual risk reduction. This methodology is built around that goal.
