# Template: Requirements Traceability Matrix (RTM)

[🏠 Contents](../README.md) · Used from: [Phase 5, Analysis](../book/07-phase-5-requirements-analysis-and-documentation.md) to [Phase 10, Closure](../book/12-phase-10-project-closure.md)

> The RTM links every requirement **backwards** to why it exists (objective, source) and **forwards** to how it was delivered (design, story, test, release). It answers two questions: *"Why are we building this?"* and *"Did we deliver and test everything we agreed?"*

---

## Traceability chain

```
Business objective ─▶ Requirement ─▶ Design element ─▶ User story ─▶ Test case ─▶ Test result ─▶ Release
     (why)              (what)          (how)            (build)        (verify)     (evidence)     (live)
```

## Template

| Req ID | Requirement (short) | Priority | Source | Objective | Design ref | Story IDs | Test case IDs | Test result | Status | Change ref | Notes |
|--------|---------------------|----------|--------|-----------|------------|-----------|---------------|-------------|--------|------------|-------|
| REQ-001 | | Must | | OBJ-1 | | | | | | | |

**Status values:** Proposed · Approved · In design · In build · Built · Tested · Accepted · Delivered · Changed · Deferred · Withdrawn

## Example (QuickClaim)

| Req ID | Requirement | Priority | Source | Obj | Design | Stories | Tests | Result | Status | CR |
|--------|-------------|----------|--------|-----|--------|---------|-------|--------|--------|----|
| REQ-014 | Attach 1–10 photos per claim | Must | Claims workshop 12/03 | OBJ-1 | SD-4.2 | QC-031, QC-032 | TC-101..106, UAT-03 | Pass | Delivered | – |
| REQ-019 | Auto-save claim drafts offline | Must | Gap found in analysis | OBJ-1 | SD-4.5 | QC-047 | TC-140..143, UAT-07 | Pass | Delivered | – |
| REQ-033 | Injury claims trigger urgent alert | Must | Claims Ops interview | OBJ-3 | SD-6.1 (rev.) | QC-060 | TC-201, UAT-07 | Pass | Delivered with change | CR-002 |
| REQ-040 | Real-time claim status | Should | Customer survey | OBJ-3 | SD-7.1 | QC-071 | TC-230 | Pass | Changed (daily status) | CR-003 |
| REQ-058 | Book repair garage | Could | Sponsor at Sprint 4 demo | OBJ-3 | – | – | – | – | Deferred to phase 2 | CR-005 |

## How to use it in each phase

| Phase | What you add |
|-------|-------------|
| Analysis | Req ID, description, priority, source, objective |
| Design | Design references |
| Build | Story IDs, build status |
| Test | Test case IDs, results |
| Change | Change refs and status updates |
| Closure | Final status for every row; summary counts |

**Tip:** in Jira / Azure DevOps much of this can be done with issue links. Then the RTM is a filter or report rather than a spreadsheet.
