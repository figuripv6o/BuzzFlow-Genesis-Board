# ADR-0003: Licensing & Commercial Boundary

## Status
Accepted

## Date
2026-02-03

## Context

With Genesis (ADR-0001) and the Execution Model (ADR-0002) established,
BuzzFlow requires a clear boundary between:
- open usage
- future commercial pathways
- governance of licensing changes over time

Without an explicit boundary, projects risk:
- accidental loss of control
- unclear commercial rights
- retroactive restriction attempts
- contributor confusion

This ADR defines the **Licensing & Commercial Boundary**.

---

## Decision

BuzzFlow adopts a **versioned, forward-only licensing strategy**.

### Current State
- License: MIT
- Scope: Entire repository unless explicitly stated
- Attribution required per MIT terms

### Future State (Planned)
- Dual-license model may be introduced:
  - Open license (e.g., MIT) for community use
  - Commercial or restricted license for specific modules, branding, or services

### Boundary Rules
- Existing MIT-licensed commits remain MIT
- License changes apply only to:
  - future versions, or
  - explicitly marked components
- Commercial paths never rewrite historical licenses

---

## Consequences

### Positive
- Legal clarity without blocking adoption
- Safe
