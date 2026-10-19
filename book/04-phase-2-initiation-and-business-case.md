# Chapter 4: Phase 2, Initiation and the business case

[← Previous](03-phase-1-idea-and-opportunity.md) · [🏠 Contents](../README.md) · [Next: Phase 3, Planning →](05-phase-3-planning-the-ba-approach.md)

---

## What's happening

The idea has passed its first gate. Now the organisation decides **whether to invest** in it. This phase produces:

- A **business case** that justifies the investment.
- A **project charter** (or *Project Initiation Document*, PID) that formally creates the project, names the sponsor and PM, and sets high-level scope.
- In an ICT services company, often a **proposal / Statement of Work (SoW)** for the client.

The **Project Manager** is usually appointed here and owns the charter. The **BA** owns (or heavily contributes to) the analysis that makes the business case credible.

## Why the BA matters here

A business case is only as good as the analysis behind it. Without a BA:

- Only one option is considered (usually the one the sponsor already likes).
- Benefits are guessed, not estimated from evidence.
- Scope is written so loosely that every later conversation becomes a dispute.
- Key stakeholders (compliance, operations, IT security) are discovered too late.

## Your responsibilities

- [ ] Analyse **options** for solving the problem, including "do nothing".
- [ ] Assess **feasibility** of each option: business, technical, financial, operational, legal.
- [ ] Estimate **benefits** and help the PM and finance estimate **costs**.
- [ ] Define **high-level scope**: what's in, what's out.
- [ ] Identify and analyse **stakeholders** (start the stakeholder register).
- [ ] Capture high-level **assumptions, constraints, dependencies and risks**.
- [ ] Define **success measures (KPIs)** that will be checked after go-live.
- [ ] Contribute business sections of the charter / SoW.

## Who you work with

| Person | Relationship in this phase |
|--------|---------------------------|
| **Sponsor** | Owns the business case and the decision. You give them the analysis. |
| **Project Manager** | Owns the charter, cost and schedule estimates. You provide scope and requirements input. |
| **Finance** | Validates cost/benefit numbers |
| **Solution architect** | Assesses technical feasibility and high-level cost of options |
| **Legal / compliance / security** | Flags regulatory constraints early |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Options analysis** | Compare 3–4 options against weighted criteria |
| **Feasibility study** | Check each option is possible and sensible |
| **Cost-benefit analysis, ROI, payback period** | Quantify the case |
| **Stakeholder analysis (power/interest grid)** | Decide how to engage each stakeholder |
| **Context diagram** | Show the system boundary and what it interacts with |
| **In/out scope table** | Make scope explicit |
| **SMART objectives** | Make goals Specific, Measurable, Achievable, Relevant, Time-bound |

### Power / interest grid

```
           High │  KEEP SATISFIED        │  MANAGE CLOSELY
                │  (e.g. CIO, Compliance)│  (e.g. Sponsor, Claims Ops Mgr)
   POWER        │────────────────────────┼─────────────────────────────
                │  MONITOR               │  KEEP INFORMED
           Low  │  (e.g. Marketing)      │  (e.g. Claims agents, customers)
                └────────────────────────┴─────────────────────────────
                          Low          INTEREST           High
```

## Deliverables

| Deliverable | Template |
|-------------|----------|
| Business case (or BA sections of it) | [Business case template](../templates/business-case.md) |
| Stakeholder register and power/interest grid | [Stakeholder register](../templates/stakeholder-register.md) |
| High-level scope statement and context diagram | Part of the business case / charter |
| Initial assumptions, constraints, risks | Shared with the PM's RAID log |

## QuickClaim in this phase

You compare four options:

| Option | Cost (est.) | Time | Meets outcomes? | Score |
|--------|-------------|------|-----------------|-------|
| A. Do nothing, hire more agents | Low upfront, high ongoing | Immediate | Wait drops, cost rises, satisfaction barely moves | 2/10 |
| B. Web claim form on the website | Low | 3 months | Partly: poor photo upload on phones | 5/10 |
| C. Claims feature in existing mobile app | Medium | 6 months | Yes: photos, GPS, policy already logged in | **8/10** |
| D. Full new claims platform replacing back office | Very high | 18+ months | Yes, plus much more | 6/10 (too big, too slow) |

**Recommendation: Option C**, with a phase-2 option to extend later.

High-level scope:

| In scope | Out of scope |
|----------|--------------|
| First notification of loss (FNOL) for motor claims in the existing mobile app | Home and travel claims |
| Photo and document upload | Replacing the back-office claims system |
| Claim status tracking | Automated claim settlement / payment |
| Integration with policy and claims systems | Web version (future phase) |

KPIs agreed with the sponsor: claim reporting time under 10 minutes, 40% of motor claims via app within 6 months of launch, claims satisfaction from 54% to 70%.

You also found a stakeholder nobody had invited: the **Data Protection Officer**, because the app will collect accident photos and location data. Finding that now saves weeks later.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Only analysing the sponsor's favourite option | Always include "do nothing" and at least two alternatives |
| Benefits like "improved efficiency" | Put a number and a date on every benefit |
| Vague scope ("claims app") | Use an explicit in/out-of-scope table |
| Forgetting non-obvious stakeholders | Ask "who else could stop or be hurt by this?" |

## Exit checklist

- [ ] Options analysed and a recommendation made
- [ ] Business case approved by the sponsor
- [ ] High-level scope agreed (in and out)
- [ ] Stakeholder register started
- [ ] KPIs and success measures defined
- [ ] Project charter / SoW signed

---

[← Previous](03-phase-1-idea-and-opportunity.md) · [🏠 Contents](../README.md) · [Next: Phase 3, Planning →](05-phase-3-planning-the-ba-approach.md)
