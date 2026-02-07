# DEC-0001 — Institute mandate + scope boundary

- **Status:** Proposed
- **Date:** 2026-02-03
- **Owner:** Scottish Open Source Institute proposal (repo)

## Context
This repository’s purpose (per `docs/GOALS.md` and `docs/SCOPE.md`) is to produce a **costed, phased proposal** for a Scottish Open Source Institute focused on practical sovereignty over **critical information flows**.

To avoid scope creep and slogan-driven outcomes, we need a crisp operational mandate and explicit boundaries:
- What the Institute is accountable for delivering (as a proposal and as an operating entity)
- What it is **not** attempting to do (especially “build everything”)
- How we decide what belongs inside the “critical information flows” set

## Decision
The proposal will define the Institute’s initial mandate as:

1) **Identify and continuously maintain** (from public sources where possible) a dependency map of Scotland’s critical information flows for government and basic civil continuity.

2) **Design and cost** a phased plan to achieve a **minimal viable sovereign baseline** for those flows:
   - Operable under partial connectivity / partition / cloud provider outage
   - Minimizing single-vendor and single-jurisdiction dependencies in critical paths
   - With incident response and recovery built in (not bolted on)

3) **Coordinate and catalyze adoption** via standards, reference architectures, procurement guidance, and targeted delivery support—rather than attempting to implement every subsystem.

### Scope boundary rules
A capability is in-scope for the Institute’s initial mandate if it satisfies **all** of:
- **Continuity-critical:** required for continuity of government or basic civil needs (as defined in `docs/GOALS.md`)
- **Sovereignty-relevant:** has meaningful coercive dependency risk (single vendor/jurisdiction, opaque control planes, irreversible lock-in)
- **Intervention-leverage:** the Institute can materially reduce that risk via open architectures/standards, reference designs, procurement levers, or supporting delivery partners

A capability is explicitly out-of-scope for the initial mandate if it is:
- Primarily **offensive** in nature (military/offensive cyber)
- Purely “nice to have” (no continuity-critical linkage)
- Best handled as routine product delivery by existing agencies/teams without sovereignty leverage

## Rationale
- Keeps “sovereignty” grounded as an **operational capability** (non-negotiable).
- Creates a tractable first deliverable: a costed baseline + roadmap.
- Establishes the Institute as an enabler (standards, reference architectures, procurement guidance) rather than a monolithic implementer.
- Provides a repeatable rule for inclusion/exclusion to prevent endless debate and uncontrolled expansion.

## Consequences
- We will need an early **capability map** and dependency taxonomy to apply the scope boundary rules.
- Costing will emphasize scenarios and ranges (capex/opex/headcount) rather than false precision.
- Future decisions will refine definitions for “critical information flow” and “sovereignty-relevant dependency” into measurable criteria.

## Links
- `docs/GOALS.md`
- `docs/SCOPE.md`
- `docs/DESIGN.md`
