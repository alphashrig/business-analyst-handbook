# Chapter 13: After closure, benefits realisation

[← Previous](12-phase-10-project-closure.md) · [🏠 Contents](../README.md) · [Next: BA vs Project Manager →](../roles/ba-vs-project-manager.md)

---

## What's happening

The project is closed, but the **business case is not yet proven**. Benefits like "40% fewer claims calls" only appear months after go-live. **Benefits realisation** is the work of measuring whether the promised value arrived, and acting if it didn't.

The **sponsor / business owner** is accountable for benefits. A BA (from the project, or the product/operations team) often does the measurement and analysis.

## Why the BA matters here

- The BA defined the KPIs back in [initiation](04-phase-2-initiation-and-business-case.md), so they know exactly what was promised and how to measure it.
- If benefits fall short, analysis finds out **why**: adoption, usability, process, or a wrong assumption in the business case.
- The findings feed the next phase's business case, closing the loop back to [Phase 1](03-phase-1-idea-and-opportunity.md).

```
     ┌──────────────────────────────────────────────────────────────┐
     │                                                              │
     ▼                                                              │
   IDEA ─▶ INITIATION ─▶ ... ─▶ DEPLOY ─▶ CLOSE ─▶ BENEFITS REVIEW ─┘
                                                   "What should we do next?"
```

## Your responsibilities (if assigned)

- [ ] Collect **KPI data** at agreed intervals (e.g. 3, 6 and 12 months).
- [ ] Compare **actuals vs targets** from the business case.
- [ ] Analyse **causes** of any shortfall (user research, analytics, process review).
- [ ] Recommend **actions**: training, UX fixes, process changes, further development.
- [ ] Report to the sponsor and feed insights into the next initiative.

## QuickClaim: the 6-month review

| KPI | Baseline | Target | Actual at 6 months | Status |
|-----|----------|--------|--------------------|--------|
| Time to report a claim | 25 min call + 38 min wait | < 10 min | 7 min median | ✅ |
| Share of motor claims via app | 0% | 40% | 31% | ⚠️ |
| Claims satisfaction | 54% | 70% | 72% | ✅ |
| Contact-centre claims calls | 100% | −40% | −28% | ⚠️ |

Adoption is below target. You analyse app analytics and run 10 short customer interviews, and find:

- Many customers **don't know** the feature exists. The phone IVR doesn't mention it.
- 18% of customers **abandon** at the policy login screen because they forgot their password.

Recommendations: add an IVR message offering an SMS link to the app; add one-time-code login for claims. Both are cheap. At 12 months: **44%** via app and **−41%** calls. The business case is met.

Those findings, and the phase 2 backlog, become the starting point for BrightCover's next project. The lifecycle starts again, and you're in the room from the first idea.

## Key takeaway

> A project's success isn't "we delivered on time and budget". It's "we delivered the value we promised". The BA is the role that keeps that question alive from the first idea to the last KPI.

---

[← Previous](12-phase-10-project-closure.md) · [🏠 Contents](../README.md) · [Next: BA vs Project Manager →](../roles/ba-vs-project-manager.md)
