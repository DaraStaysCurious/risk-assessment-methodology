# Corrective Action to Remediation
> Addressing the symptom looks good on paper.
> Addressing the root cause actually reduces risk.

---

## Table of Contents
- [Executive Summary](#executive-summary)
- [Finding Identification](#finding-identification)
- [The POA&M](#the-poam)
- [Root Cause Analysis](#root-cause-analysis)
- [Multi-Owner Remediation](#multi-owner-remediation)
- [Verification and Residual Risk](#verification-and-residual-risk)
- [Implications for GRC Practice](#implications-for-grc-practice)
- [Key Takeaways](#key-takeaways)
- [Contact](#contact)

---

## Executive Summary

OHS corrective action and GRC remediation are the same process —
find it, score it, own it, fix the cause, verify it worked.

The most common failure in both fields is the same: addressing the
symptom instead of the root cause. A corrective action that doesn't
change the underlying condition doesn't reduce risk. It produces
documentation that says the risk was addressed — which is not the
same thing.

---

## Finding Identification

**Findings come from six sources. Every source triggers the same
process.**

| Finding source | OHS example | GRC equivalent |
|---------------|-------------|---------------|
| Routine inspection | Worker climbing shelves instead of using a ladder | Vulnerability scan finding |
| Near miss | Forklift almost struck a pedestrian | Failed login escalated for investigation |
| Incident | Chemical spill in storage area | Confirmed data breach |
| Employee report | Frayed electrical cable reported | Phishing email reported |
| Internal audit | No lockout/tagout procedure found | No access review process found |
| Regulatory inspection | OSHA cites inadequate PPE storage | HIPAA audit identifies control gap |

**Every finding source is equally valid.** A finding from an
employee report carries the same weight as a regulatory citation —
because the risk is identical regardless of how it was discovered.

---

## The POA&M

**A finding without a POA&M is an observation.
A finding with a POA&M is a managed risk.**

The Plan of Action and Milestones is the operational mechanism
through which risk gets reduced. Required by NIST 800-53, referenced
in FedRAMP, and expected in virtually every compliance framework.

**Every POA&M contains:**

| Field | Purpose |
|-------|---------|
| Finding ID | Unique identifier for tracking |
| Finding date | When the issue was identified |
| Finding source | How it was discovered |
| Risk score | Likelihood × Exposure × Impact |
| Root cause | Why it happened |
| Remediation tasks | Specific actions required to close |
| Task owners | One named person per task |
| Due dates | Specific dates — not "ASAP" |
| Status | Open / In Progress / Closed |
| Verification method | How closure will be confirmed |
| Residual risk score | Re-scored after remediation |

---

## Root Cause Analysis
### The Five Whys Method

**Ask why until you reach the cause — not just the symptom.**

**Case study: Worker climbing warehouse shelving**

| Why | Answer |
|-----|--------|
| Why was the employee climbing the shelves? | No ladder was nearby |
| Why was no ladder nearby? | Only one ladder existed |
| Why did only one ladder exist? | Budget was never approved |
| **Root cause** | **No process for identifying and escalating equipment gaps** |

**Obvious corrective action:** Retrain employee. ❌
**Actual corrective action:** Buy ladders, install them, fix the
process that allowed the gap to exist. ✅

**The same logic in GRC:**

| Finding | Obvious fix | Root cause | Actual fix |
|---------|------------|------------|------------|
| Employees sharing passwords | Retrain on policy | System requires simultaneous access | Redesign access controls |
| Phishing clicks | Awareness training | Email filtering is inadequate | Improve filtering first |
| Patches consistently delayed | Send reminders | No defined ownership or SLA | Establish patch management process |

---

## Multi-Owner Remediation

**Complex findings require multiple tasks with multiple owners.**

The ladder finding had four tasks — each with a different owner:

| Task | Owner | Status |
|------|-------|--------|
| Purchase 3 ladders | Procurement | Open |
| Install ladders | Maintenance | Open |
| Update safe work procedure | Safety Manager | Open |
| Conduct employee training | Safety Manager + Supervisors | Open |

**Three rules for multi-owner remediation:**

- **One named owner per task** — shared ownership is no ownership
- **Every task has a specific due date** — "ASAP" is not a date
- **Finding stays open until every task is verified closed** —
  three of four complete is an open finding

---

## Verification and Residual Risk

**A remediation that isn't verified isn't closed.
It's assumed closed — which is a different thing entirely.**

**Two-step verification:**

**Step 1 — Observational:** Return to where the finding was
identified. Confirm implementation in practice, not just on paper.

**Step 2 — Re-score:** Run the risk calculation again with the
corrective action in place.

| Variable | Pre-remediation | Post-remediation |
|----------|----------------|-----------------|
| Likelihood | High | Low |
| Exposure | Very High | Moderate |
| Impact | High | High |
| **Risk level** | **Very High** | **Moderate** |

**If the score hasn't meaningfully changed — the finding stays
open. The corrective action didn't work.**

**When full remediation isn't possible:**
Residual risk must be formally accepted — documented, signed off
by the risk owner, and scheduled for reassessment. Undocumented
residual risk is avoidance, not acceptance.

---

## Implications for GRC Practice

1. **Treat all finding sources equally** — employee reports and
   audit findings carry the same weight.
2. **Create a POA&M for every finding** — named owner, due date,
   status, verification method.
3. **Always use the Five Whys** — before writing a single
   remediation task.
4. **One named owner per task** — not a team. A person.
5. **Keep findings open until every task is verified** — partial
   completion is not closure.
6. **Re-score after remediation** — documentation is not evidence
   of effectiveness. Risk reduction is.

---

## Key Takeaways

- Corrective actions that address symptoms — not root causes —
  don't reduce risk. They produce paperwork.
- The Five Whys reveals root causes that obvious fixes miss
- Every finding needs a POA&M with a named owner, due date,
  and verification method
- Multi-owner findings stay open until every task is closed
- Verification requires re-scoring — not just task completion
- Residual risk must be formally accepted, not silently ignored

---

## Contact

**Dara Thomas** — GRC Analyst & Consultant | Human-Centered Risk & Compliance

[LinkedIn](YOUR_LINKEDIN_URL) · dara.thomas.grc@gmail.com · [GitHub Portfolio](https://github.com/DaraStaysCurious)

---

*Part of the [risk-assessment-methodology](../README.md) repository.*
*Next: [human-factors-in-risk.md](human-factors-in-risk.md) — coming soon*
