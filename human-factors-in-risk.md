# Human Factors in Risk
> Security programs fail when they treat human error as the problem.
> They succeed when they treat human error as a signal that the
> system needs to be redesigned.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [The Core Thesis](#the-core-thesis)
- [Three Case Studies](#three-case-studies)
- [The Five Principles](#the-five-principles)
- [Human Factors in GRC](#human-factors-in-grc)
- [Implications for GRC Practice](#implications-for-grc-practice)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

Unsafe behavior is almost always a system design failure — not a
human failure. The welder using cardboard instead of a fire-rated
blind, the warehouse worker climbing shelves instead of a ladder,
the cruise ship crew running over each other's feet — none of these
are recklessness problems. They are design problems producing
reckless-looking behavior as their inevitable output.

GRC faces the same dynamic constantly. Employees sharing passwords,
clicking phishing links, bypassing security controls — these are
signals. The question is not "how do we enforce compliance?" It is
"what does this behavior tell us about the design of the system?"

---

## The Core Thesis

**Controls fail when they're designed around ideal human behavior.
Controls succeed when they're designed around actual human behavior.**

| Wrong question | Right question |
|---------------|---------------|
| Why aren't people following the procedure? | Why does the procedure make unsafe behavior the easier choice? |
| How do we enforce compliance? | What does non-compliance tell us about the control design? |
| How do we train people to do this correctly? | How do we redesign the system so correct behavior is the path of least resistance? |

**The shift:** from behavior modification to system redesign.

---

## Three Case Studies

### Case Study 1: The Welding Blind
**Environment:** Powdered laundry detergent factory

| Element | Detail |
|---------|--------|
| Observed behavior | Welders using cardboard to block sparks instead of fire-rated welding blinds |
| Management interpretation | Reckless behavior — safety violation |
| Root cause | Welding blinds stored three floors below the work area |
| System failure | Control designed without accounting for the friction cost of use |
| Fix | Built a storage closet on the correct floor |
| Lesson | The wrong behavior was easier than the right one — until the environment changed |

**GRC parallel:** Employees writing passwords on sticky notes aren't
being careless. The password policy is so complex that memorization
is genuinely harder than the workaround.

---

### Case Study 2: The Missing Ladder
**Environment:** Warehouse

| Element | Detail |
|---------|--------|
| Observed behavior | Worker climbing shelving instead of using a ladder |
| Management interpretation | Safety violation — needs retraining |
| Root cause | Only one ladder existed in the entire warehouse |
| System failure | Equipment gap created by a process that never formally identified or escalated it |
| Fix | Purchased additional ladders, installed them accessibly, fixed the gap reporting process |
| Lesson | You cannot train people to use equipment that doesn't exist |

**GRC parallel:** Employees bypassing the VPN aren't ignoring
security policy. The VPN drops connections during video calls —
making bypass the only practical option for getting work done.

---

### Case Study 3: The I-95 Corridor
**Environment:** Cruise ship — embarkation day

| Element | Detail |
|---------|--------|
| Observed behavior | Crew members' feet being run over by luggage carts |
| Management interpretation | Crew being reckless during a busy period |
| Root cause | Three simultaneous system failures |
| System failure 1 | Single corridor required for opposing traffic flows — collisions were geometrically inevitable |
| System failure 2 | Worn cart wheels spinning unpredictably — equipment degradation made carts uncontrollable |
| System failure 3 | 4-hour turnaround made rushing a structural requirement, not a personal choice |
| Fix | Time-based traffic scheduling: 1.5hr disembarkation window → 1hr cart-free period → 1.5hr embarkation window |
| What couldn't be fixed | The 4-hour turnaround — outside safety manager authority. Designed around instead. |
| Result | Significant accident reduction, increased productivity, better guest satisfaction |
| Lesson | When rushing is a system requirement, you can't train people to stop rushing. Redesign the system. |

**GRC parallel:** Developers bypassing security reviews before
deployments aren't ignoring policy. The review process takes longer
than the deployment window — making bypass the only way to meet
the deadline.

---

## The Five Principles

**Derived from a decade of OHS practice. Applicable in every GRC
context.**

**1. The people closest to the risk know the most about it.**
Their knowledge doesn't surface automatically — it requires
deliberate, structured conversation with enough psychological
safety to name problems rather than defend the status quo.

**2. Resistance is data.**
Classify it before dismissing it:

| Type | Sounds like | Tells you |
|------|------------|-----------|
| Convenience resistance | "Who has time for this" / impatient tone | Examine the friction cost of the control |
| Substantive resistance | "That won't work because..." / theory about the risk | There's contextual knowledge in the room your assessment missed |

**3. Friction kills controls.**
A control that requires significant extra effort will be routed
around — not occasionally, but reliably. The correct behavior must
always be easier than the workaround.

**4. Absence of incident ≠ absence of risk.**
"We've never been breached" is not a risk assessment. Near misses,
failed logins, and caught phishing emails are likelihood data —
not reassurance.

**5. Co-design produces better controls than top-down design.**
Controls built with the people who must use them are more effective,
more durable, and more practically intelligent than controls handed
down for implementation.

---

## Human Factors in GRC

**The same system design failures that produced accidents on factory
floors and cruise ships produce security incidents in organizations.**

| Human behavior | Typical GRC response | Human factors response |
|---------------|--------------------|-----------------------|
| Sharing passwords | Retrain on password policy | Redesign access controls to eliminate shared credential requirement |
| Clicking phishing links | Conduct awareness training | Improve email filtering — training is supplementary |
| Bypassing VPN | Remind of security policy | Fix the VPN connection stability issue |
| Ignoring MFA prompts | Enforce MFA strictly | Reduce MFA friction — hardware tokens, push notifications |
| Using personal Dropbox | Block personal cloud storage | Provide a fast, accessible approved alternative |
| Writing passwords down | Security awareness training | Implement a password manager |

**The pattern:** every typical GRC response addresses the behavior.
Every human factors response addresses the system condition that
produced the behavior.

**Both matter.** But system redesign without behavior change produces
durable risk reduction. Behavior change without system redesign
produces compliance theater.

---

## Implications for GRC Practice

1. **When a control fails, ask why before enforcing compliance** —
   the failure is data about the control design, not just the user.

2. **Map the friction cost of every control before finalizing it** —
   what is the easiest way to not do this? If the workaround is
   easier than compliance, the control will fail.

3. **Treat non-compliance as a signal, not just a violation** —
   classify it: is this convenience resistance or substantive
   resistance? Both require different responses.

4. **Interview the people inside the system** — not a survey, a
   conversation. Ask what they actually do, what workarounds they've
   developed, and what they'd fix if they could fix anything.

5. **Design controls with end users, not for them** — co-design
   produces controls that fit the reality people work in. Top-down
   design produces controls people route around.

6. **Distinguish between what can be changed and what must be
   designed around** — the 4-hour turnaround couldn't be changed.
   The corridor scheduling could. Know the difference and act on
   what's within your authority.

---

## Key Takeaways

- Unsafe behavior is almost always a system design failure —
  not a human failure
- The three case studies illustrate the same principle across
  three environments: factory, warehouse, cruise ship
- Controls fail when designed around ideal behavior — they succeed
  when designed around actual behavior
- Non-compliance is data — classify it before responding to it
- Friction kills controls reliably — the correct behavior must
  always be easier than the workaround
- Co-design produces more durable controls than top-down design
- Distinguish between what can be fixed and what must be designed
  around — and act on what's within your authority

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)

---

*Part of the [risk-assessment-methodology](../README.md) repository.*
*Next: [applications.md](applications.md) — coming soon*
