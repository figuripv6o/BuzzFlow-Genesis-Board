# ADR-0002: BuzzFlow Execution Model

## Status
Accepted

## Date
2026-02-03

## Context

With **ADR-0001 (Genesis)** established, BuzzFlow now requires a clear execution model
that defines **how ideas move from concept to system** without losing intent,
ownership, or structure.

Common failure modes after genesis include:
- building without decision traceability
- mixing exploration with execution
- scaling artifacts before governance
- unclear boundaries between core and extensions

This ADR defines the **Execution Layer**.

---

## Decision

BuzzFlow adopts a **layered execution model**:

1. **Genesis Layer**
   - Immutable origin
   - Authorship, intent, and direction
   - Documented via ADR-0001

2. **Decision Layer**
   - Architecture Decision Records (ADRs)
   - Each major structural choice is logged
   - Changes are additive, not destructive

3. **Build Layer**
   - Repositories, modules, diagrams, and artifacts
   - May evolve rapidly
   - Must reference decisions when relevant

4. **Expansion Layer**
   - Optional modules, forks, or commercial paths
   - Governed separately if needed
   - May introduce dual licensing or trademarks

Execution flows **downward**, never backward.

---

## Rules of Execution

- No build without context
- No scale without structure
- No fork without attribution
- No governance added retroactively

---

## Consequences

### Positive
- Clear separation of thinking vs building
- Reduced chaos as complexity grows
- Easier onboarding for aligned contributors
- Long-term legal and structural clarity

### Trade-offs
- Slight overhead in documenting decisions
- Requires discipline to maintain boundaries

---

## Notes

ADR-0002 depends on ADR-0001 and must be read in sequence.
Future ADRs should reference one or both where applicable.

Execution is not speed.  
Execution is **alignment**.
