# Template: Change request (CR)

[🏠 Contents](../README.md) · Used in: [Phase 7, Build](../book/09-phase-7-development-and-build.md), [Phase 8, Testing](../book/10-phase-8-testing-and-uat.md)

> Any change to the **baselined** scope, requirements, schedule or budget goes through a CR. The BA documents the change and analyses business impact; the PM adds time/cost impact; the sponsor or PO decides.

---

## 1. Request

| Field | Value |
|-------|-------|
| CR ID | *CR-0xx* |
| Title | *...* |
| Raised by | *Name, role* |
| Date raised | *dd/mm/yyyy* |
| Description of change | *What is being asked for?* |
| Reason / business justification | *Why? What problem or opportunity?* |
| Urgency | *High / Medium / Low* |

## 2. Impact analysis

| Area | Impact | Assessed by |
|------|--------|-------------|
| **Requirements affected** | *REQ IDs added / changed / removed* | BA |
| **Business processes / users affected** | *...* | BA |
| **Benefits / objectives** | *Does it increase, reduce or not affect value?* | BA |
| **Design / architecture** | *...* | Architect |
| **Effort** | *e.g. +3 sprints / X person-days* | Tech lead |
| **Schedule** | *Impact on milestones and go-live* | PM |
| **Cost** | *...* | PM |
| **Risk** | *New risks introduced* | PM / BA |
| **Testing** | *Retesting / regression needed* | QA |
| **Contract** | *Billable? SoW amendment needed?* | PM / account manager |

## 3. Options

| Option | Description | Pros | Cons |
|--------|-------------|------|------|
| 1 | Approve now | | |
| 2 | Defer to a later release | | |
| 3 | Reject | | |
| 4 | Approve a reduced version | | |

**BA recommendation:** *...*

## 4. Decision

| Field | Value |
|-------|-------|
| Decision | *Approved / Deferred / Rejected / Approved with conditions* |
| Decided by | *Name, role* |
| Date | |
| Conditions / notes | |

## 5. Follow-up actions (BA)

- [ ] Update requirements baseline / BRD
- [ ] Update RTM
- [ ] Update backlog
- [ ] Inform stakeholders
