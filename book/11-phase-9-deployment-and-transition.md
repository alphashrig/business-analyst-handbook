# Chapter 11: Phase 9, Deployment and transition

[← Previous](10-phase-8-testing-and-uat.md) · [🏠 Contents](../README.md) · [Next: Phase 10, Project closure →](12-phase-10-project-closure.md)

---

## What's happening

The solution goes **live**. Technically, deployment is owned by the dev/DevOps team and coordinated by the PM. But a technically successful release can still be a **business failure** if people don't know how to use it, processes haven't changed, or support isn't ready.

**Transition** means moving the organisation from the old way of working to the new one.

## Why the BA matters here

The BA understands both the new solution and the business processes it changes. That makes the BA the natural person to make sure the **business is ready**, not just the software:

- Processes, roles and procedures are updated.
- Users are trained on real scenarios.
- Support teams know the business rules and common questions.
- Data migrated from old systems is correct and complete.
- Someone checks after go-live that it's actually working for the business.

## Your responsibilities

- [ ] Define and track **transition requirements** (training, data migration, process changes, communications).
- [ ] Support **business readiness** assessment: are people, processes and data ready?
- [ ] Update **business process documentation** and standard operating procedures (SOPs).
- [ ] Support or lead creation of **training materials** and user guides.
- [ ] Validate **data migration** results with the business (sample checks, reconciliation).
- [ ] Contribute to the **go/no-go** decision with evidence on business readiness.
- [ ] Prepare **support handover**: FAQs, known issues, business rules, escalation paths.
- [ ] Provide **hypercare** (early-life support): monitor issues, triage feedback, quick clarifications.

## Who you work with

| Person | Relationship |
|--------|-------------|
| **PM** | Owns the deployment plan and go/no-go meeting |
| **DevOps / release team** | Technical deployment |
| **Business operations managers** | Owners of new processes and staff readiness |
| **Trainers / change managers** | Training and change communication (the BA may do this on smaller projects) |
| **IT support / service desk** | Receive the handover; will support the live system |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Business readiness checklist** | Assess go-live readiness from the business side |
| **Stakeholder impact assessment** | Identify who is affected and how (role changes, new tasks) |
| **Data reconciliation** | Compare record counts and samples before and after migration |
| **Train-the-trainer** | Scale training through super-users |
| **Hypercare triage** | Sort early issues quickly (defect, training, change) |

### Business readiness checklist (example)

| Area | Ready? | Evidence |
|------|--------|----------|
| Users trained | ✅ | 142 / 150 agents trained; rest scheduled |
| SOPs updated | ✅ | "Handling app claims" SOP published |
| Support team briefed | ✅ | Handover session done; FAQ in knowledge base |
| Customer comms ready | ✅ | App store notes, email, website banner |
| Rollback plan understood by business | ✅ | Phone channel stays open as before |
| Hypercare rota | ✅ | BA + dev on call for 2 weeks |

## Deliverables

| Deliverable | Description |
|-------------|-------------|
| Transition requirements | What must happen for a successful switch-over |
| Updated process maps and SOPs | The to-be process, now the as-is |
| Training materials / user guides | Scenario-based, short |
| Business readiness assessment | Input to go/no-go |
| Support handover pack | FAQs, business rules, known issues, contacts |
| Hypercare issue log | Triaged early-life issues |

## QuickClaim in this phase

- **Soft launch:** the PO and you recommend releasing to 10% of customers first. The PM agrees and builds it into the release plan.
- **Training:** you write a one-page "App claims in 5 minutes" guide for agents, with screenshots of the agent workspace, and run 3 train-the-trainer sessions with team leads.
- **SOP update:** you update the claims handling procedure so app-submitted injury claims get a callback within 1 hour.
- **Go/no-go:** you present the business-readiness checklist. Everything is green. **Go.**
- **Hypercare (2 weeks):** 41 issues come in. You triage them daily with the dev lead: 9 defects (2 urgent, fixed in a hotfix), 21 training/how-to questions (FAQ updated), 11 enhancement ideas (logged for phase 2).
- After one week at 10%, metrics look good. Rollout goes to 100%.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Thinking "deployed" means "done" | Business adoption is the real finish line |
| Training on features, not tasks | Train on real scenarios: "a customer reports an injury claim..." |
| No support handover | The service desk will be flooded with questions they can't answer |
| Leaving the project on go-live day | Plan hypercare; early issues need the BA's knowledge |

## Exit checklist

- [ ] Business readiness confirmed at go/no-go
- [ ] Users trained; SOPs updated
- [ ] Data migration validated (if applicable)
- [ ] Support handover complete
- [ ] Hypercare completed; remaining issues handed to support or the backlog

---

[← Previous](10-phase-8-testing-and-uat.md) · [🏠 Contents](../README.md) · [Next: Phase 10, Project closure →](12-phase-10-project-closure.md)
