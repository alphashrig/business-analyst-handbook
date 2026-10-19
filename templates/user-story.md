# Template: User story and acceptance criteria

[🏠 Contents](../README.md) · Used in: [Phase 5, Analysis](../book/07-phase-5-requirements-analysis-and-documentation.md), [Phase 7, Build](../book/09-phase-7-development-and-build.md)

---

## Format

```
Title:   <short, action-based>
ID:      <e.g. QC-123>     Epic: <epic name>     Priority: <MoSCoW>

As a   <type of user>
I want <goal / capability>
So that <business value / reason>

Acceptance criteria:
  Scenario 1: <name>
    Given <context>
    When  <action>
    Then  <expected outcome>

Notes / business rules / links:
  - <links to designs, rules, RTM requirement ID>
```

## Example (QuickClaim)

```
Title:   Resume a claim draft after losing connection
ID:      QC-047     Epic: Start a claim     Priority: Must
Traces to: REQ-019, OBJ-1

As a   policyholder reporting a claim from the roadside
I want my claim progress saved automatically
So that I don't have to start again if my signal or battery drops

Acceptance criteria:
  Scenario 1: Draft saved while offline
    Given I have entered incident details and taken 2 photos
    When  the app loses network connection
    Then  my entered details and photos are saved on the device

  Scenario 2: Resume on reopening
    Given I have an unsubmitted claim draft
    When  I reopen the app
    Then  I see "Continue your claim" with my saved progress

  Scenario 3: Draft expiry
    Given a claim draft is older than 30 days
    When  I open the app
    Then  the draft is deleted and I see a message explaining why

Notes:
  - Business rule BR-004: claims must be reported within 30 days of the incident
  - Design: Figma > Start claim > Draft states
```

## Quality checks: INVEST

| Letter | Question | ✔ |
|--------|----------|---|
| **I**ndependent | Can it be built without waiting for another story? | |
| **N**egotiable | Does it describe the need, not dictate the solution? | |
| **V**aluable | Is the "so that" a real benefit to a user or the business? | |
| **E**stimable | Can the team estimate it? | |
| **S**mall | Does it fit within one sprint? | |
| **T**estable | Can QA write tests from the acceptance criteria? | |

## Ways to split a large story

- By **workflow step** (start, add photos, submit)
- By **business rule** (normal claim vs injury claim)
- By **happy path vs exceptions**
- By **data type** (photos vs documents)
- By **user type** (customer vs agent)
- By **platform** (iOS vs Android), only if truly different
