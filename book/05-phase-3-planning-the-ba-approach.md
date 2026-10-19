# Chapter 5: Phase 3, Planning the BA approach

[← Previous](04-phase-2-initiation-and-business-case.md) · [🏠 Contents](../README.md) · [Next: Phase 4, Elicitation →](06-phase-4-requirements-elicitation.md)

---

## What's happening

The project is approved. The **Project Manager** builds the project plan: schedule, budget, resources, risks, communication. In parallel, the **BA plans the business analysis work**: how requirements will be found, documented, approved and managed.

New BAs often skip this step and jump straight into meetings. Don't. A one-page BA plan saves weeks of confusion.

## Why the BA matters here

The PM's plan needs realistic dates for requirements work, and those dates come from you. Without a BA plan:

- Requirements workshops get scheduled with the wrong people, or not at all.
- Nobody knows who signs off requirements, so nothing is ever "final".
- Change requests arrive by email, chat and corridor conversations, with no control.
- The format of requirements (BRD? user stories?) gets argued about mid-project.

## Your responsibilities

- [ ] Choose the **BA approach**: predictive (Waterfall), adaptive (Agile), or hybrid.
- [ ] Plan **stakeholder engagement**: who, how often, through which channels.
- [ ] Plan **elicitation activities**: which techniques, with whom, when.
- [ ] Agree the **requirements format** and tools (e.g. BRD in Confluence, stories in Jira).
- [ ] Define **requirements governance**: who approves, how changes are handled, how priorities are decided.
- [ ] Plan **traceability**: how requirements link to design, tests and business objectives.
- [ ] Estimate **BA effort** and feed it into the PM's schedule.
- [ ] Agree on a **Definition of Ready** (when a requirement is ready for development).

## Who you work with

| Person | Relationship in this phase |
|--------|---------------------------|
| **Project Manager** | You provide BA activities, durations and dependencies; they integrate them into the master plan |
| **Sponsor / Product Owner** | Agree who approves requirements and how priorities are set |
| **Tech lead / architect** | Agree the level of detail developers need |
| **QA lead** | Agree how requirements will be made testable and traced to tests |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **BA planning (BABOK "Business Analysis Planning and Monitoring")** | Structure your approach |
| **RACI matrix** | Clarify who approves and who is consulted ([see RACI page](../roles/raci-who-does-what.md)) |
| **Prioritisation scheme (MoSCoW)** | Agree in advance how priorities will be set |
| **Work breakdown** | Break BA work into estimable tasks |

### MoSCoW in one table

| Priority | Meaning | Rule of thumb |
|----------|---------|---------------|
| **Must have** | Without it, the solution is useless or illegal | ≤ 60% of effort |
| **Should have** | Important, but there's a workaround | ~20% |
| **Could have** | Nice to have if time allows | ~20% |
| **Won't have (this time)** | Agreed as out for this release | Recorded, not built |

## Deliverables

### The BA plan (one or two pages)

| Section | Example content |
|---------|----------------|
| Approach | Hybrid: BRD for scope baseline, user stories for sprint delivery |
| Stakeholders and engagement | Weekly with Claims Ops Mgr; fortnightly steering with sponsor; 2 workshops with agents |
| Elicitation plan | 6 interviews, 3 workshops, 1 day contact-centre observation, survey of 200 customers |
| Requirements artefacts | BRD (Confluence), epics and stories (Jira), process maps (BPMN) |
| Approval | Sponsor signs BRD; PO accepts stories |
| Change control | All changes via [change request](../templates/change-request.md), assessed by BA + PM, approved by sponsor |
| Traceability | [RTM](../templates/requirements-traceability-matrix.md): objective → requirement → story → test case |
| Schedule | Elicitation weeks 1–3, BRD sign-off week 5 |

## QuickClaim in this phase

The PM tells you the build starts in week 6. You work backwards:

- Weeks 1–3: interviews, workshops, contact-centre observation.
- Week 4: write the BRD and process maps.
- Week 5: review and sign-off, with the sponsor's diary already booked.
- From week 5: break the BRD into epics and stories for Sprint 1.

You also agree with the sponsor that **the Claims Operations Manager acts as Product Owner** for day-to-day decisions, so you aren't waiting on the Head of Claims for every question.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| No named approver | Get one person's name for sign-off, in writing |
| Planning elicitation without checking stakeholder availability | Book diaries now; senior people fill up weeks ahead |
| No change process | Agree it before the first change arrives |
| Arguing format mid-project | Agree templates and tools in this phase |

## Exit checklist

- [ ] BA plan reviewed with the PM and integrated into the project plan
- [ ] Approvers and prioritisation method agreed
- [ ] Change control process agreed
- [ ] Workshops and interviews scheduled
- [ ] Tools and templates set up

---

[← Previous](04-phase-2-initiation-and-business-case.md) · [🏠 Contents](../README.md) · [Next: Phase 4, Elicitation →](06-phase-4-requirements-elicitation.md)
