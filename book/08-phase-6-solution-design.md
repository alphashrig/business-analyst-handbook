# Chapter 8: Phase 6, Solution design

[← Previous](07-phase-5-requirements-analysis-and-documentation.md) · [🏠 Contents](../README.md) · [Next: Phase 7, Development and build →](09-phase-7-development-and-build.md)

---

## What's happening

With requirements baselined, the **solution architect**, **tech lead** and **UX designer** decide **how** the solution will work: architecture, integrations, data structures, screens and technology choices.

The BA does **not** design the technical solution. But the BA is essential to make sure the design **still meets the business need**.

## Why the BA matters here

Designers and architects make dozens of trade-offs. Every trade-off can quietly drop or bend a requirement. The BA is the **guardian of the requirements** during design:

- Checks that every Must-have requirement is covered by the design.
- Explains business context when designers face a choice ("which matters more to users, speed or completeness?").
- Spots when a technical constraint forces a business decision, and takes it to the business rather than letting the team decide silently.

## Your responsibilities

- [ ] **Walk the design team through** the requirements and the reasons behind them.
- [ ] **Answer questions** and clarify business rules quickly, so design doesn't stall.
- [ ] **Review designs** (architecture overviews, wireframes, interface specs) against requirements.
- [ ] Help write or review the **Functional Specification (FS/FRS)**, if your company uses one.
- [ ] Assess the **business impact** of design trade-offs and constraints.
- [ ] **Update the RTM**: link requirements to design elements.
- [ ] Run **design walkthroughs** with business stakeholders (especially for UX).
- [ ] Raise **change requests** if design reveals requirements must change.

## Who you work with

| Person | They own | You provide |
|--------|----------|-------------|
| **Solution architect** | Technical architecture, integration patterns, technology choices | Business context, NFRs, priorities |
| **UX / UI designer** | User experience, screen designs, prototypes | User needs, personas, journeys, business rules |
| **Tech lead** | Detailed technical design, estimates | Clarifications, acceptance criteria |
| **Product Owner / sponsor** | Decisions on trade-offs | Clear options and impact analysis |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Requirements-to-design traceability** | Prove every requirement is covered |
| **Prototype / wireframe walkthroughs** | Validate UX with real users before build |
| **Impact analysis** | Explain what a constraint or design choice means for the business |
| **Interface / integration specifications** | Agree data exchanged between systems (with the architect) |
| **State diagrams** | Clarify the lifecycle of key objects (e.g. claim statuses) |

## Deliverables

| Deliverable | BA's role |
|-------------|-----------|
| Functional specification | Author or co-author (in some companies the BA writes it, in others a systems analyst does) |
| Reviewed wireframes / prototypes | Reviewer and validator with users |
| Updated RTM (requirement → design) | Owner |
| Design decisions log entries with business impact | Contributor |
| Change requests arising from design | Author |

## QuickClaim in this phase

The architect proposes a design: the app writes claims into a new **cloud claims-intake service**, which syncs to the legacy claims system through the nightly batch.

You review it against the requirements and find:

| Requirement | Design coverage | Issue |
|-------------|-----------------|-------|
| REQ-031 Customer sees claim reference immediately | ✅ Intake service generates it | — |
| REQ-033 Urgent injury claims flagged for agent callback within 1 hour | ❌ Batch is nightly | **Gap.** An injured customer could wait until the next morning |
| REQ-040 Status tracking | ⚠️ Status updates only daily | Acceptable? Needs a business decision |

For REQ-033 you run a short session with the architect and the Claims Ops Manager. The agreed fix: injury claims also trigger an **instant alert** to the claims team queue. A small design change, captured before a single line of code.

For REQ-040 you present options to the PO: daily status (no extra cost) vs near-real-time (new API on the legacy system, +6 weeks). The PO accepts daily status for release 1. You record the decision and update the requirement.

You then run a **clickable-prototype session** with 6 real customers. Two couldn't find the "add photo" button on smaller phones. The UX designer fixes it in a day.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Disappearing after BRD sign-off | Stay close; design is where requirements get lost |
| Designing the technical solution yourself | Describe needs and constraints; let architects design |
| Letting the tech team silently drop a requirement | Make the trade-off visible and take it to the decision-maker |
| Reviewing designs without the RTM | Use the RTM as your checklist |

## Exit checklist

- [ ] Every Must-have requirement traced to a design element
- [ ] Design gaps resolved or raised as change requests
- [ ] Prototypes validated with users
- [ ] Trade-off decisions recorded with the business owner's approval

---

[← Previous](07-phase-5-requirements-analysis-and-documentation.md) · [🏠 Contents](../README.md) · [Next: Phase 7, Development and build →](09-phase-7-development-and-build.md)
