# Chapter 2: The ICT project lifecycle at a glance

[← Previous](01-who-is-a-business-analyst.md) · [🏠 Contents](../README.md) · [Next: Phase 1, Idea →](03-phase-1-idea-and-opportunity.md)

---

## The big picture

Every ICT project, whether it's a mobile app, an ERP rollout or a network upgrade, passes through roughly the same stages. Names vary between companies and methodologies, but the shape is the same.

```
 ┌────────┐  ┌────────────┐  ┌──────────┐  ┌──────────────┐  ┌────────┐  ┌───────┐  ┌──────┐  ┌────────┐  ┌───────┐  ┌──────────┐
 │  IDEA  │─▶│ INITIATION │─▶│ PLANNING │─▶│ REQUIREMENTS │─▶│ DESIGN │─▶│ BUILD │─▶│ TEST │─▶│ DEPLOY │─▶│ CLOSE │─▶│ BENEFITS │
 └────────┘  └────────────┘  └──────────┘  └──────────────┘  └────────┘  └───────┘  └──────┘  └────────┘  └───────┘  └──────────┘
   Ph 1          Ph 2            Ph 3          Ph 4–5           Ph 6        Ph 7       Ph 8       Ph 9        Ph 10      After
```

## BA involvement across the lifecycle

The BA is involved from the very first conversation to well after go-live. But the **intensity** of the work changes.

| Phase | BA effort | The BA's main question |
|-------|-----------|------------------------|
| 1. Idea | 🟨🟨⬜⬜⬜ | *Is this a real problem worth solving?* |
| 2. Initiation | 🟨🟨🟨⬜⬜ | *What's the business case, and who's involved?* |
| 3. Planning | 🟨🟨🟨⬜⬜ | *How will we do the analysis work?* |
| 4. Elicitation | 🟨🟨🟨🟨🟨 | *What do stakeholders actually need?* |
| 5. Analysis and documentation | 🟨🟨🟨🟨🟨 | *Are the requirements complete, clear and agreed?* |
| 6. Design | 🟨🟨🟨🟨⬜ | *Does the proposed design meet the requirements?* |
| 7. Build | 🟨🟨🟨⬜⬜ | *Is the team building the right thing? What about changes?* |
| 8. Test and UAT | 🟨🟨🟨🟨⬜ | *Does the solution do what the business needs?* |
| 9. Deploy | 🟨🟨🟨⬜⬜ | *Is the business ready to use it?* |
| 10. Closure | 🟨🟨⬜⬜⬜ | *Did we deliver what was agreed? What did we learn?* |
| After closure | 🟨⬜⬜⬜⬜ | *Did we get the benefits we promised?* |

> **Key insight:** the BA's heaviest work happens *early*, when changes are cheap. That is exactly why involving a BA from the idea phase pays off.

## The cost-of-change curve

The later a misunderstanding is found, the more it costs to fix.

```
 Cost to fix
     ▲
     │                                                    ●  After go-live
     │                                              
     │                                        ●  Testing
     │                              
     │                       ●  Build
     │              ●  Design
     │   ●  Requirements
     └─────────────────────────────────────────────────────────▶ Time
```

A missing requirement caught in a workshop costs an hour of conversation. The same gap found after go-live may need a redesign, rework, retesting, a new release, customer complaints and a damaged client relationship.

## Waterfall, Agile and hybrid

| | Waterfall | Agile (e.g. Scrum) | Hybrid |
|-|-----------|--------------------|--------|
| **Shape** | Phases happen once, in order | Requirements → build → test repeat every 1–4 weeks | Upfront analysis and planning, then iterative delivery |
| **Requirements** | Mostly defined upfront in a BRD/SRS | Evolve in a product backlog as user stories | High-level upfront, detailed per sprint |
| **BA artefacts** | BRD, FRS, use cases, RTM | Epics, user stories, acceptance criteria, backlog | Both |
| **Common in** | Fixed-price contracts, government, regulated work | Product companies, digital teams | Most ICT services companies today |

Most ICT services companies run **hybrid** projects: a contract and business case upfront (Waterfall-style), then delivery in sprints (Agile-style). QuickClaim is hybrid.

More detail: [The BA in Agile vs Waterfall](../guides/ba-in-agile-vs-waterfall.md).

## Governance gates

Between phases, organisations usually hold a **gate** (or *stage gate*, or *phase review*): a decision point where the sponsor decides to **go**, **stop**, or **go back**. The BA's deliverables are often key evidence at these gates.

| Gate | Decision | BA evidence |
|------|----------|-------------|
| Idea → Initiation | Is this worth exploring? | Problem statement, opportunity summary |
| Initiation → Planning | Approve the project and budget? | Business case, options analysis, stakeholder map |
| Requirements → Design | Are requirements baselined? | Signed-off BRD / prioritised backlog, RTM |
| Test → Deploy | Ready for go-live? | UAT sign-off, defect status, readiness checklist |
| Deploy → Close | Can we formally close? | Requirements coverage, handover docs, lessons learned |

---

[← Previous](01-who-is-a-business-analyst.md) · [🏠 Contents](../README.md) · [Next: Phase 1, Idea →](03-phase-1-idea-and-opportunity.md)
