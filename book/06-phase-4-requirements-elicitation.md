# Chapter 6: Phase 4, Requirements elicitation

[← Previous](05-phase-3-planning-the-ba-approach.md) · [🏠 Contents](../README.md) · [Next: Phase 5, Analysis and documentation →](07-phase-5-requirements-analysis-and-documentation.md)

---

## What's happening

This is the heart of the BA role. **Elicitation** means *drawing out* requirements. We say "elicit", not "gather", because requirements aren't lying around waiting to be picked up. Stakeholders often don't know what they need, can't put it into words, or assume you already know.

## Why the BA matters here

Everyone on the project has opinions about what should be built. The BA is the one person whose job is to make sure **all** the relevant voices are heard, the **real** needs are found, and **unspoken** assumptions are surfaced. Without that:

- The loudest stakeholder's wish list becomes the scope.
- Front-line users, the ones who'll use the system every day, are never asked.
- Non-functional needs (security, performance, accessibility) are forgotten until testing.

## Your responsibilities

- [ ] **Prepare** for each session: objectives, questions, materials, the right attendees.
- [ ] **Conduct** elicitation using a mix of techniques.
- [ ] Understand the **current state (as-is)** in detail.
- [ ] Explore the **future state (to-be)** with stakeholders.
- [ ] Capture **business, stakeholder, functional and non-functional** requirements, plus business rules.
- [ ] **Confirm** what you heard: send notes back and play back understanding.
- [ ] Track **open questions** and chase answers.

## Types of requirements

| Type | Question it answers | QuickClaim example |
|------|---------------------|--------------------|
| **Business requirement** | Why is the organisation doing this? | Reduce claims calls by 40% |
| **Stakeholder / user requirement** | What does each group need? | Customers need to report a claim without calling |
| **Functional requirement** | What must the system do? | The app shall let the user attach up to 10 photos |
| **Non-functional requirement (NFR)** | How well must it do it? | Photo upload completes in < 5 s on 4G; WCAG 2.1 AA accessible |
| **Business rule** | What policy constrains it? | Claims must be reported within 30 days of the incident |
| **Transition requirement** | What's needed to switch over? | Agents trained before launch; in-flight phone claims unaffected |

## Who you work with

| Person | What you get from them |
|--------|-----------------------|
| End users (customers, agents) | How the work is really done, frustrations, needs |
| Subject matter experts | Rules, exceptions, edge cases |
| Product Owner / sponsor | Priorities, goals, decisions |
| IT / architects | Existing systems, integrations, technical constraints |
| Compliance, legal, security, DPO | Regulatory and policy requirements |
| UX designer | User research and early prototypes |

## Techniques

| Technique | Best for | Tip |
|-----------|----------|-----|
| **Interviews** | Depth with individuals | Use open questions; ask "can you show me?" |
| **Workshops** | Agreement across groups | Have a clear agenda, a facilitator (you) and a decision-maker present |
| **Observation (job shadowing)** | Seeing what people really do, not what they say they do | Sit with users for a few hours; note workarounds |
| **Document analysis** | Existing rules, forms, policies, old specs | Read before interviews to ask better questions |
| **Surveys / questionnaires** | Many users, quick data | Keep it short; mix ratings with one open question |
| **Prototyping / wireframes** | Making abstract ideas concrete | Low-fidelity first; people critique sketches more honestly |
| **Brainstorming** | Generating options | Quantity first, judgement later |
| **Focus groups** | Customer perspectives | Use a neutral facilitator |
| **Interface analysis** | System-to-system needs | Work with the architect on data flowing in and out |

### Good questions to ask

- "Walk me through the last time you did this."
- "What happens when it goes wrong?"
- "What do you do that the system doesn't help with?"
- "If you could change one thing, what would it be?"
- "Who else should I talk to?"
- "How would you know this project was a success?"

## Deliverables

| Deliverable | Description |
|-------------|-------------|
| Elicitation notes | Confirmed with participants within 24–48 hours |
| As-is process maps | How things work today |
| Raw requirements list | Unrefined but captured, with source |
| Open questions / issues log | Who owes an answer, by when |

## QuickClaim in this phase

- **Observation:** you spend a day in BrightCover's contact centre. You see agents asking customers to spell their registration number letter by letter, then retyping it from the policy system. → *Requirement: pre-fill vehicle and policy data from the logged-in customer's policy.*
- **Customer survey (212 responses):** 61% had an accident at night or at a weekend, when the contact centre was closed. → *Requirement: 24/7 reporting.*
- **Workshop with claims handlers:** they need photos tagged by damage area, or they waste time sorting them. → *Requirement: guided photo capture (front, rear, sides, damage close-up).*
- **Interview with the DPO:** location data may only be stored with explicit consent. → *Requirement: GPS capture is opt-in, with a manual address alternative.*
- **Interface analysis with the architect:** the legacy claims system accepts new claims only through a nightly batch file. → *Major constraint, raised to the PM as a risk.*

That last finding alone could have broken the "claim status tracking" feature. You found it in week 2, not in testing.

## Common mistakes

| Mistake | Instead |
|---------|---------|
| Only talking to managers | Always include the people doing the work |
| Asking "what do you want?" | Ask about tasks, problems and goals; analyse wants yourself |
| Writing notes nobody confirms | Send notes back and ask for corrections |
| Forgetting NFRs | Use a checklist: security, performance, availability, accessibility, privacy, audit |
| Treating every request as a requirement | Capture everything; filter and prioritise in analysis |

## Exit checklist

- [ ] All key stakeholder groups engaged
- [ ] As-is processes understood and mapped
- [ ] Requirements captured with their source
- [ ] NFRs and business rules covered
- [ ] Notes confirmed by participants
- [ ] Open questions tracked with owners

---

[← Previous](05-phase-3-planning-the-ba-approach.md) · [🏠 Contents](../README.md) · [Next: Phase 5, Analysis and documentation →](07-phase-5-requirements-analysis-and-documentation.md)
