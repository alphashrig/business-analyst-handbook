# Chapter 7: Phase 5, Requirements analysis and documentation

[← Previous](06-phase-4-requirements-elicitation.md) · [🏠 Contents](../README.md) · [Next: Phase 6, Solution design →](08-phase-6-solution-design.md)

---

## What's happening

You have pages of notes, sticky notes, survey results and process sketches. Now you turn that raw material into **clear, consistent, prioritised, agreed requirements** that a team can design, build and test against.

Elicitation and analysis overlap in practice. You'll go back to stakeholders with questions many times.

## Why the BA matters here

This is where requirements become a **contract**: between the business and the delivery team, and in an ICT services company often literally between your company and the client. Without solid analysis:

- Requirements contradict each other and developers guess.
- "The system shall be user-friendly" can't be tested, so it can't be accepted.
- Scope keeps moving because there was never a signed baseline.
- Nobody can tell which requirements matter most when time runs short.

## Your responsibilities

- [ ] **Organise** requirements (by process, feature, or epic).
- [ ] **Model** the future state: processes, data, screens, rules.
- [ ] **Analyse** for gaps, conflicts, duplicates and ambiguity.
- [ ] **Prioritise** with stakeholders (MoSCoW or similar).
- [ ] **Specify** requirements so they're clear and testable.
- [ ] **Validate** that requirements support the business objectives.
- [ ] **Verify** quality: complete, consistent, unambiguous, feasible.
- [ ] Get **sign-off** and set the **baseline**.
- [ ] Start the **Requirements Traceability Matrix (RTM)**.

## What makes a good requirement?

| Quality | Bad | Good |
|---------|-----|------|
| **Clear** | The app should handle photos well | The app shall allow the user to attach 1–10 photos per claim |
| **Testable** | The app should be fast | Claim submission shall complete within 3 seconds for 95% of requests |
| **Atomic** | The user can upload photos and track status | Split into two requirements |
| **Necessary** | The app shall show the weather | (Traces to no objective → remove) |
| **Feasible** | Real-time updates from the claims system | Status refreshed every 15 min (given the batch constraint) |
| **Traceable** | (no ID, no source) | REQ-014, source: Claims workshop 12 Mar, objective OBJ-2 |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Process modelling (BPMN, swimlanes)** | Show the to-be workflow and who does what |
| **Use cases / use case diagrams** | Describe system interactions step by step, including alternate and exception flows |
| **User stories + acceptance criteria** | Express requirements for Agile teams ([template](../templates/user-story.md)) |
| **Data modelling (ERD, data dictionary)** | Define data entities, fields and rules |
| **Wireframes / mock-ups** | Make screens concrete and validate early |
| **Decision tables** | Capture complex business rules unambiguously |
| **Gap analysis** | Compare as-is and to-be; list what must change |
| **MoSCoW prioritisation** | Agree what's essential |
| **Peer review / walkthroughs** | Find defects in requirements before build |

### Example: decision table

*Can the claim be submitted through the app?*

| Rule | Policy active? | Incident ≤ 30 days ago? | Injury reported? | Outcome |
|------|---------------|------------------------|------------------|---------|
| 1 | No | – | – | Block: show "contact us" |
| 2 | Yes | No | – | Block: late claim, route to agent |
| 3 | Yes | Yes | Yes | Submit + flag for urgent agent callback |
| 4 | Yes | Yes | No | Submit normally |

## Deliverables

| Deliverable | Template / note |
|-------------|----------------|
| **Business Requirements Document (BRD)** or equivalent | [BRD template](../templates/brd.md) |
| To-be process maps | BPMN or swimlane |
| Use cases and/or **product backlog** of epics and stories | [User story template](../templates/user-story.md) |
| Data dictionary, business rules catalogue | Appendices of the BRD |
| Wireframes | Usually with the UX designer |
| **Requirements Traceability Matrix** | [RTM template](../templates/requirements-traceability-matrix.md) |
| Sign-off record | Email or formal sign-off in the BRD |

## QuickClaim in this phase

You organise 74 raw requirements into five epics:

1. **Start a claim**: eligibility, incident details, location
2. **Capture evidence**: guided photos, documents, witness details
3. **Submit and confirm**: review, consent, submission, reference number
4. **Track claim**: status, messages, next steps
5. **Agent workspace**: view app claims in the claims system

During analysis you find a **conflict**: Marketing wants the claim form to collect "how did you hear about us?" data; the DPO says it isn't necessary for a claim and must not be mandatory. You bring both to the PO, who decides it is **Won't have**. The decision is recorded with the reason.

You also find a **gap**: nobody specified what happens if the customer loses connection mid-claim. New requirement: *drafts auto-save locally and resume when the app reopens.*

Final priority split: 38 Must, 19 Should, 11 Could, 6 Won't. The sponsor signs the BRD in week 5, and it becomes the **baseline**. From now on, changes go through change control.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Writing a 200-page BRD nobody reads | Use diagrams, tables and examples; keep prose short |
| Everything is "Must have" | Push back: "If we could only deliver half, which half?" |
| Only the happy path | Write alternate and exception flows |
| Solution-specific requirements ("a blue dropdown") | Describe the need; let UX/design choose the control |
| No sign-off | No baseline means no change control and endless scope creep |

## Exit checklist

- [ ] Requirements organised, modelled, prioritised
- [ ] Ambiguities, conflicts and gaps resolved or logged
- [ ] Reviewed with business, dev and QA
- [ ] Signed off and baselined
- [ ] RTM started, linking requirements to objectives

---

[← Previous](06-phase-4-requirements-elicitation.md) · [🏠 Contents](../README.md) · [Next: Phase 6, Solution design →](08-phase-6-solution-design.md)
