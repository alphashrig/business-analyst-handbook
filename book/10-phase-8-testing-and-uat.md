# Chapter 10: Phase 8, Testing and UAT

[← Previous](09-phase-7-development-and-build.md) · [🏠 Contents](../README.md) · [Next: Phase 9, Deployment and transition →](11-phase-9-deployment-and-transition.md)

---

## What's happening

The solution is (mostly) built. Now it's tested at several levels:

| Test level | Who runs it | Question it answers |
|------------|-------------|---------------------|
| Unit testing | Developers | Does each piece of code work? |
| Integration testing | Developers / QA | Do the pieces and systems work together? |
| System testing | QA team | Does the whole system meet the specification? |
| Non-functional testing | QA / specialists | Is it fast, secure, accessible, reliable enough? |
| Regression testing | QA (often automated) | Did new changes break old features? |
| **User Acceptance Testing (UAT)** | **Business users**, supported by the **BA** | **Does it meet the business need, in real-world use?** |

The BA is most involved in **UAT**, and supports QA throughout.

## Why the BA matters here

QA checks that the system works **as specified**. UAT checks that the specification was **right**. The BA connects both:

- QA test cases are only as good as the requirements and acceptance criteria they're based on.
- Business users are not professional testers. Someone must prepare scenarios, guide them and interpret results.
- Every defect needs triage: is it a bug, a missed requirement, a change, or a misunderstanding? The BA knows the requirements best.
- UAT sign-off is often a **contractual milestone** in ICT services. Getting it cleanly matters.

## Your responsibilities

- [ ] Review **QA test cases** against requirements and acceptance criteria.
- [ ] Plan **UAT** with the business: scope, participants, environment, data, schedule, entry/exit criteria.
- [ ] Write **UAT scenarios** based on real business processes (not just screens).
- [ ] Prepare and brief **UAT testers**.
- [ ] **Support** testers during UAT: answer questions, help log defects clearly.
- [ ] **Triage defects** with QA, dev lead and PO (bug vs change vs misunderstanding; severity; priority).
- [ ] Update the **RTM** (requirement → test case → result).
- [ ] Obtain **UAT sign-off** from the business owner.

## Who you work with

| Person | Relationship |
|--------|-------------|
| **QA lead** | Owns system test; you align test coverage with requirements |
| **Business users / SMEs** | Execute UAT; you prepare and support them |
| **Product Owner / sponsor** | Decide on defects and give sign-off |
| **Developers** | Fix defects; you clarify expected behaviour |
| **PM** | Tracks the test schedule and go-live readiness |

## Techniques

| Technique | Use it to... |
|-----------|--------------|
| **Scenario-based testing** | Test end-to-end business processes, not isolated features |
| **Requirements-based test coverage (RTM)** | Prove every requirement was tested |
| **Defect triage** | Classify and prioritise issues quickly |
| **Entry / exit criteria** | Agree when UAT can start and when it's done |

### Defect triage: is it really a bug?

| Finding | Classification | Action |
|---------|---------------|--------|
| System behaves differently from the agreed requirement | **Defect** | Fix, by severity |
| System behaves as specified, but the spec was wrong or missed something | **Requirement gap / change** | Change request; PO decides |
| User expected something never in scope | **Out of scope / enhancement** | Log for future; explain the baseline |
| User misunderstood how it works | **Training / usability** | Clarify; consider UX or training improvements |

### Typical UAT exit criteria

- 100% of planned scenarios executed
- 0 open critical (Severity 1) and 0 high (Severity 2) defects, or each one has an agreed workaround and fix date
- All Must-have requirements passed
- Sign-off by the named business owner

## Deliverables

| Deliverable | Template |
|-------------|----------|
| UAT plan and scenarios | [UAT plan and sign-off](../templates/uat-sign-off.md) |
| Defect triage log | Usually in Jira / Azure DevOps |
| Updated RTM with test results | [RTM](../templates/requirements-traceability-matrix.md) |
| UAT sign-off | [UAT sign-off](../templates/uat-sign-off.md) |

## QuickClaim in this phase

You build 24 UAT scenarios from real claims, for example:

> **UAT-07:** *It's 11pm. Priya was rear-ended at a junction, has a sore neck, and is reporting from the roadside with 30% battery and weak signal.*
> Expected: she can start a claim, flag the injury, capture 4 photos, lose connection, reopen the app and resume, submit, and get a reference number. The claims team receives an urgent alert.

UAT runs for two weeks with 8 claims handlers and 15 real customers (in a test environment, with test policies).

Results:

- 37 issues logged. After your triage: **19 defects**, **6 changes**, **8 training/usability**, **4 out of scope**.
- One finding is serious: claims handlers can't see photo damage-area tags in the agent workspace. It traces to REQ-022 (Must) and is a real defect, fixed in 3 days.
- One "defect" is that customers can't edit a claim after submitting. That was never a requirement. The PO decides it's a **Should** for release 1.1.

All exit criteria are met in week 2. The Head of Claims signs UAT.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Letting users "just play with it" | Give them structured scenarios plus some exploratory time |
| Using clean, perfect test data | Use realistic and messy data, including edge cases |
| Treating every issue as a defect | Triage it: defect vs change vs training |
| Accepting "looks fine" as sign-off | Get explicit, written sign-off against exit criteria |
| Doing UAT yourself | UAT belongs to the business; you support it |

## Exit checklist

- [ ] All UAT scenarios executed
- [ ] Defects triaged and resolved per exit criteria
- [ ] RTM shows each requirement as tested and passed (or accepted exception)
- [ ] Written UAT sign-off from the business owner

---

[← Previous](09-phase-7-development-and-build.md) · [🏠 Contents](../README.md) · [Next: Phase 9, Deployment and transition →](11-phase-9-deployment-and-transition.md)
