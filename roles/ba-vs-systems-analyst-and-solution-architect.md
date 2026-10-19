# Business Analyst vs Systems Analyst and Solution Architect

[← BA vs Product Owner](ba-vs-product-owner.md) · [🏠 Contents](../README.md) · [Next: BA vs QA, Developers and UX →](ba-vs-qa-developers-and-ux.md)

---

These three roles sit along a line from **business problem** to **technical solution**.

```
  BUSINESS PROBLEM ◀─────────────────────────────────────────────────▶ TECHNICAL SOLUTION

     Business Analyst            Systems Analyst              Solution Architect
   "What does the business     "What exactly must the        "How should the system be
    need, and why?"             system do to meet it?"        structured to deliver it?"
```

The boundaries blur, and in many ICT companies the BA covers some systems analysis too. What matters is knowing which question you're answering.

## Side-by-side comparison

| Area | Business Analyst | Systems Analyst | Solution Architect |
|------|------------------|-----------------|-------------------|
| **Focus** | Business needs, processes, value | System behaviour and functional specification | Overall technical structure and technology choices |
| **Key question** | Why and what (business view)? | What exactly (system view)? | How (technically)? |
| **Typical artefacts** | Business case input, BRD, process maps, user stories, business rules | Functional / system requirements spec (FRS/SRS), use cases, data models, interface specs | Architecture diagrams, solution design document, integration and infrastructure designs, technology decisions |
| **Works mostly with** | Business stakeholders, PO, PM | BA, developers, architects | Tech leads, enterprise architects, security, infrastructure |
| **Technical depth** | Low to medium | Medium to high | High |
| **Owns NFRs?** | Elicits them from the business | Specifies them precisely | Designs to meet them |

## The same requirement, three views

| Role | How they express it |
|------|---------------------|
| **BA** | *"Injured customers must get a callback from a claims handler within 1 hour of reporting, at any time of day."* (business need + rule) |
| **Systems analyst** | *"On submission of a claim where `injury_reported = true`, the system shall create a priority-1 task in the Claims Queue and send a push alert to on-duty handlers within 60 seconds."* (system behaviour) |
| **Solution architect** | *"The intake service publishes a `ClaimSubmitted` event to the message bus; an alerting service subscribes and calls the workforce management API; the legacy batch path is bypassed for priority claims."* (technical design) |

## How the BA works with the Solution Architect

- **Early (idea and initiation):** the architect assesses feasibility and rough cost of options. You give business context and constraints.
- **Requirements:** you share NFRs and interface needs; they flag technical constraints (like QuickClaim's nightly batch).
- **Design:** they design; you review the design against requirements and take trade-offs to the business.
- **Golden rule:** you never tell the architect *how* to build it. They never decide *what* the business needs. Trade-offs go to the PO/sponsor.

## If you are expected to do systems analysis too

In many ICT companies, especially smaller ones, the BA also writes the functional specification. Build these skills gradually:

- Reading API documentation and understanding request/response data.
- Basic data modelling (entities, relationships, keys).
- Basic SQL to query and verify data.
- Understanding of integration patterns (APIs, batch files, events).
- State diagrams and sequence diagrams.

See [Skills, tools and career path](../guides/skills-tools-and-career-path.md).

---

[← BA vs Product Owner](ba-vs-product-owner.md) · [🏠 Contents](../README.md) · [Next: BA vs QA, Developers and UX →](ba-vs-qa-developers-and-ux.md)
