# Template: UAT plan and sign-off

[🏠 Contents](../README.md) · Used in: [Phase 8, Testing and UAT](../book/10-phase-8-testing-and-uat.md)

---

## Part A: UAT plan

| Section | Content |
|---------|---------|
| **Objective** | *Confirm the solution supports the business processes and meets the agreed requirements* |
| **Scope** | *Features / epics in UAT; anything excluded* |
| **Participants** | *Names, roles, availability* |
| **Environment** | *UAT environment URL / build version; access set up by...* |
| **Test data** | *Realistic data incl. edge cases; who prepares it* |
| **Schedule** | *Start / end dates; daily triage time* |
| **Entry criteria** | *System testing complete; no open Sev-1 defects; environment and data ready; testers briefed* |
| **Exit criteria** | *All scenarios executed; 0 open Sev-1/Sev-2 (or agreed workarounds); all Must requirements passed; sign-off* |
| **Defect process** | *Where to log; severity definitions; triage owners* |
| **Roles** | *BA: plan, scenarios, support, triage. Business testers: execute. QA: environment and defects. PO: decisions.* |

### Severity definitions

| Severity | Meaning |
|----------|---------|
| 1, Critical | Business process cannot be completed; no workaround |
| 2, High | Major function impaired; workaround is difficult |
| 3, Medium | Function impaired; reasonable workaround exists |
| 4, Low | Cosmetic or minor |

## Part B: UAT scenario

| Field | Value |
|-------|-------|
| Scenario ID | *UAT-07* |
| Title | *Night-time injury claim with lost connection* |
| Business process | *First notification of loss* |
| Requirements covered | *REQ-014, REQ-019, REQ-033* |
| Preconditions | *Test policy active; user logged in* |
| Steps | *1. ... 2. ... 3. ...* |
| Expected result | *...* |
| Actual result | |
| Pass / Fail | |
| Tester / date | |
| Defect IDs | |

## Part C: UAT summary and sign-off

| Metric | Value |
|--------|-------|
| Scenarios planned / executed / passed | */ /* |
| Issues raised | |
| ... of which defects / changes / training / out of scope | */ / /* |
| Open defects by severity | *Sev-1: 0 · Sev-2: 0 · Sev-3: x · Sev-4: y* |
| Accepted known issues (with workaround and fix date) | *...* |

**Statement:**
> I confirm that User Acceptance Testing has been completed in line with the UAT plan, that the exit criteria have been met (with the exceptions listed above), and that the solution is accepted for production deployment.

| Name | Role | Decision | Signature / date |
|------|------|----------|------------------|
| | Business owner / sponsor | Accepted / Accepted with conditions / Not accepted | |
| | Product Owner | | |
