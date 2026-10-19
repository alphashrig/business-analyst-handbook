# Chapter 9: Phase 7, Development and build

[← Previous](08-phase-6-solution-design.md) · [🏠 Contents](../README.md) · [Next: Phase 8, Testing and UAT →](10-phase-8-testing-and-uat.md)

---

## What's happening

Developers are building the solution. In most ICT companies today this happens in **sprints** (1–4 week cycles), even if the earlier phases were Waterfall-style. Each sprint takes a set of user stories from the backlog, builds them, tests them, and demos them.

## Why the BA matters here

Developers will have questions every day. If the answers are slow or wrong, they **guess**, and guesses become defects. The BA keeps the build pointed at the business need:

- Stories are **ready** before the sprint starts (clear, estimated, with acceptance criteria).
- Questions are answered in hours, not days.
- **Changes** are controlled instead of slipping in through side conversations.
- The business sees progress in demos and gives feedback early.

## Your responsibilities

- [ ] **Backlog refinement:** split epics into stories, write acceptance criteria, keep the backlog ordered with the PO.
- [ ] Make sure stories meet the **Definition of Ready** before sprint planning.
- [ ] Attend **sprint planning** to explain stories and answer questions.
- [ ] Be **available** to developers and testers daily (stand-ups, chat, quick calls).
- [ ] **Clarify** requirements; never make business decisions alone; escalate to the PO.
- [ ] Run **impact analysis** for every change request.
- [ ] Support **sprint reviews / demos**: help explain to the business what was built and capture feedback.
- [ ] Keep the **RTM** updated (requirement → story → build status).
- [ ] Start preparing for **UAT** and **business readiness** (training, process changes).

## Who you work with

| Person | Typical interaction |
|--------|-------------------|
| **Developers** | Daily clarification, walkthroughs of stories |
| **Scrum Master / PM** | Impediments, timeline impact of changes, sprint goals |
| **Product Owner** | Prioritisation, decisions on changes and trade-offs |
| **QA / testers** | Aligning acceptance criteria and test cases |
| **Business SMEs** | Quick answers to rule questions, demo feedback |

## Change control: the BA's critical job in build

Changes **will** happen. The question is whether they are controlled.

```
 Change raised ─▶ BA logs it ─▶ BA + tech lead + PM assess impact ─▶ PO / sponsor decides ─▶ Update baseline, RTM, backlog
   (anyone)        (CR form)     (scope, cost, time, risk, quality)    (approve/reject/defer)     (BA)
```

Use the [change request template](../templates/change-request.md). The **BA** analyses business impact, the **PM** analyses schedule and cost impact, the **business** decides.

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Backlog refinement** | Keep upcoming stories ready |
| **Story splitting** (by workflow step, rule, data, happy/unhappy path) | Make stories small enough for a sprint |
| **Acceptance criteria in Given/When/Then (Gherkin)** | Make stories testable and unambiguous |
| **Three Amigos** (BA + Dev + QA) | Discuss each story from three angles before build |
| **Impact analysis** | Assess every change |
| **Definition of Ready / Definition of Done** | Shared quality bars |

### Example: Definition of Ready

A story is ready when:
- [ ] It's written in user story format with a clear "so that" (business value)
- [ ] Acceptance criteria are written and agreed by the PO
- [ ] Dependencies are known (APIs, designs, data)
- [ ] UX designs are attached, if needed
- [ ] The team has estimated it
- [ ] It fits in one sprint

## Deliverables

| Deliverable | Notes |
|-------------|-------|
| Refined, prioritised backlog | Owned by the PO, maintained with the BA |
| User stories with acceptance criteria | [Template](../templates/user-story.md) |
| Change requests and impact analyses | [Template](../templates/change-request.md) |
| Updated RTM | Requirement → story → status |
| Demo feedback log | Captured and turned into backlog items |

## QuickClaim in this phase

**Sprint 3:** a developer asks, *"If the customer takes a photo but the upload fails, do we retry automatically or ask them?"* It isn't in the requirements. You don't guess. You ask the PO in a 5-minute call: *retry 3 times silently, then show a "try again" button.* You add it to the acceptance criteria the same day.

**Sprint 4 demo:** the Head of Claims sees the app and says, *"Can we add a feature for customers to book a repair garage?"* That's a change. You log a CR and run an impact analysis with the tech lead: +3 sprints, new integration with a garage network partner. The sponsor **defers** it to phase 2. Scope stays protected, and the idea isn't lost.

**Sprint 5:** you notice the agent workspace stories have slipped down the backlog. Without them, agents can't see app claims at launch. You raise this with the PO, who moves them up. A small save that prevents a launch-day disaster.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Answering business questions yourself to "save time" | Clarify facts yourself; take decisions to the PO |
| Saying "yes" to every change in a demo | Thank them, log it, analyse it, let the decision-maker decide |
| Stories without acceptance criteria | No AC means not ready |
| Losing touch with the business during build | Keep SMEs engaged through demos and quick checks |
| Forgetting transition and training | Start business readiness now, not the week before go-live |

## Exit checklist

- [ ] All in-scope stories built and accepted in sprint reviews
- [ ] Change requests decided and reflected in the baseline
- [ ] RTM shows each requirement's build status
- [ ] UAT scenarios drafted with business users

---

[← Previous](08-phase-6-solution-design.md) · [🏠 Contents](../README.md) · [Next: Phase 8, Testing and UAT →](10-phase-8-testing-and-uat.md)
