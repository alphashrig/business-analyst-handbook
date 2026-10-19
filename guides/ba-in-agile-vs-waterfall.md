# The BA in Agile vs Waterfall

[← When does a project need a BA?](when-does-a-project-need-a-ba.md) · [🏠 Contents](../README.md) · [Next: Your first 90 days →](your-first-90-days.md)

---

The BA's job, understanding needs and making sure the right thing is built, is the same in every methodology. What changes is the **rhythm** and the **artefacts**.

## The rhythm

```
WATERFALL   [ Requirements ████████ ][ Design ]████[ Build ]████████[ Test ]████[ Deploy ]
             BA effort heavily front-loaded, then support

AGILE       [Discovery]█ [Sprint 1]▓▓ [Sprint 2]▓▓ [Sprint 3]▓▓ [Sprint 4]▓▓ ... [Release]
             BA effort spread out; always refining 1–2 sprints ahead

HYBRID      [ Discovery + baseline requirements ████ ][S1]▓▓[S2]▓▓[S3]▓▓[S4]▓▓[UAT]██[Deploy]
             Upfront scope for the contract, detailed stories per sprint
```

## Comparison

| Aspect | Waterfall BA | Agile BA |
|--------|--------------|----------|
| **When requirements are detailed** | Upfront, all at once | Just in time, 1–2 sprints ahead |
| **Main artefacts** | BRD, FRS/SRS, use cases, RTM | Product vision, epics, user stories, acceptance criteria, story maps |
| **Sign-off** | Formal sign-off of the full document | PO accepts stories; continuous acceptance at reviews |
| **Change** | Formal change control against a baseline | Expected; handled by reprioritising the backlog |
| **Customer feedback** | Mostly at UAT | Every sprint review |
| **Documentation** | Comprehensive | "Just enough", often living in tools (Jira, Confluence) |
| **BA's daily life** | Long analysis phases, then support | Constant refinement, Three Amigos, daily team contact |
| **Risk** | Late discovery that requirements were wrong | Losing the big picture; thin analysis of rules and edge cases |

## What stays the same

Regardless of methodology, a good BA:

- Understands the **problem and the value** before diving into features.
- Engages **all relevant stakeholders**, not only the loudest.
- Makes requirements **clear and testable**.
- Keeps **traceability** from objectives to delivered features (lighter in Agile, but still there).
- Supports **validation** with real users.
- Cares about **outcomes**, not just output.

## Mapping phases to Agile events

| Lifecycle chapter | Where it happens in Agile/Scrum |
|-------------------|--------------------------------|
| [Idea](../book/03-phase-1-idea-and-opportunity.md), [Initiation](../book/04-phase-2-initiation-and-business-case.md) | Discovery / Sprint 0 / product vision and roadmap |
| [Planning](../book/05-phase-3-planning-the-ba-approach.md) | Release planning; agreeing Definition of Ready/Done |
| [Elicitation](../book/06-phase-4-requirements-elicitation.md), [Analysis](../book/07-phase-5-requirements-analysis-and-documentation.md) | Story mapping; backlog refinement (continuous) |
| [Design](../book/08-phase-6-solution-design.md) | Refinement + design spikes; UX works a sprint ahead |
| [Build](../book/09-phase-7-development-and-build.md) | Sprints: planning, daily stand-up, review |
| [Test and UAT](../book/10-phase-8-testing-and-uat.md) | In-sprint testing + PO acceptance; often a UAT or hardening sprint before release |
| [Deploy](../book/11-phase-9-deployment-and-transition.md) | Release; may happen every sprint in mature teams |
| [Closure](../book/12-phase-10-project-closure.md) | Retrospectives every sprint; final project retrospective at the end |

## Agile BA techniques worth learning

| Technique | What it is |
|-----------|-----------|
| **Story mapping** | Lay out the user journey horizontally, stories vertically by priority; slice into releases |
| **INVEST** | Stories should be Independent, Negotiable, Valuable, Estimable, Small, Testable |
| **Gherkin (Given/When/Then)** | Structured acceptance criteria |
| **Impact mapping** | Goal → actors → impacts → deliverables |
| **MVP / MMP** | Minimum Viable / Marketable Product: the smallest release that delivers value |
| **Spikes** | Time-boxed research stories to reduce uncertainty |

---

[← When does a project need a BA?](when-does-a-project-need-a-ba.md) · [🏠 Contents](../README.md) · [Next: Your first 90 days →](your-first-90-days.md)
