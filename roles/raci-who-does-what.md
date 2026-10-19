# Who does what: RACI across the lifecycle

[← BA vs QA, Developers and UX](ba-vs-qa-developers-and-ux.md) · [🏠 Contents](../README.md) · [Next: When does a project need a BA? →](../guides/when-does-a-project-need-a-ba.md)

---

A **RACI matrix** shows, for each activity, who is:

| Letter | Means | Rule |
|--------|-------|------|
| **R** | **Responsible**: does the work | Can be several people |
| **A** | **Accountable**: owns the outcome, signs off | Exactly **one** per activity |
| **C** | **Consulted**: gives input before | Two-way communication |
| **I** | **Informed**: told after | One-way communication |

This is a **typical** RACI for an ICT services project. Every company differs, so use it as a starting point and agree your own in [Phase 3, Planning](../book/05-phase-3-planning-the-ba-approach.md).

**Roles:** SP = Sponsor · PO = Product Owner · PM = Project Manager · BA = Business Analyst · SA = Solution Architect · DEV = Developers / Tech Lead · QA = QA / Test · UX = UX Designer · SME = Business users / SMEs · OPS = IT support / operations

## RACI matrix

| Activity | SP | PO | PM | BA | SA | DEV | QA | UX | SME | OPS |
|----------|----|----|----|----|----|-----|----|----|-----|-----|
| **Idea and initiation** |
| Problem statement | A | C | I | **R** | C | – | – | – | C | – |
| Options and feasibility analysis | A | C | C | **R** | R | C | – | – | C | C |
| Business case | **A** | C | R | R | C | – | – | – | – | – |
| Project charter / SoW | A | C | **R** | C | C | – | – | – | – | – |
| Stakeholder register | I | C | R | **R** | – | – | – | – | C | – |
| **Planning** |
| Project plan | A | C | **R** | C | C | C | C | C | – | – |
| BA plan | I | C | C | **A/R** | – | – | C | – | – | – |
| **Requirements** |
| Elicitation | I | C | I | **A/R** | C | C | C | C | C | C |
| BRD / requirements spec | A | R | I | **R** | C | C | C | C | C | – |
| Prioritisation | C | **A** | C | R | C | C | – | – | C | – |
| Requirements sign-off | **A** | R | I | R | I | I | I | I | C | – |
| **Design** |
| Solution architecture | I | C | I | C | **A/R** | C | – | C | – | C |
| UX design | – | A | I | C | C | C | – | **R** | C | – |
| Design review against requirements | – | C | I | **R** | C | C | C | C | – | – |
| **Build** |
| Backlog ordering | – | **A/R** | C | R | – | C | – | – | – | – |
| Story writing and refinement | – | A | – | **R** | C | C | C | C | C | – |
| Development | – | I | A | C | C | **R** | C | – | – | – |
| Change request impact analysis | C | C | R | **R** | C | C | – | – | – | – |
| Change request decision | **A** | R | C | C | – | – | – | – | – | – |
| **Test** |
| System testing | – | I | A | C | – | C | **R** | – | – | – |
| UAT planning and scenarios | – | A | C | **R** | – | – | C | – | C | – |
| UAT execution | – | A | I | C | – | – | C | – | **R** | – |
| UAT sign-off | **A** | R | I | C | – | – | I | – | C | – |
| **Deploy** |
| Release / deployment | I | I | **A** | C | C | R | C | – | – | R |
| Business readiness and training | C | A | C | **R** | – | – | – | – | R | C |
| Go / no-go decision | **A** | R | R | C | C | C | C | – | C | C |
| Hypercare triage | – | C | A | **R** | – | R | C | – | C | R |
| **Close** |
| Final RTM and scope reconciliation | I | C | C | **A/R** | – | – | C | – | – | – |
| Closure report | A | C | **R** | R | C | C | C | – | – | – |
| Lessons learned | I | C | **A** | R | R | R | R | R | C | C |
| **After** |
| Benefits measurement | **A** | R | – | R | – | – | – | – | C | C |

## How to read this as a new BA

- Where you see **A/R** for the BA, that's your work and your outcome.
- Where you see **R** with someone else as **A**, you do the work but someone else signs off. Don't treat your draft as final.
- Where the BA is only **C**, give input but don't take over. For example, solution architecture is the architect's call.

---

[← BA vs QA, Developers and UX](ba-vs-qa-developers-and-ux.md) · [🏠 Contents](../README.md) · [Next: When does a project need a BA? →](../guides/when-does-a-project-need-a-ba.md)
