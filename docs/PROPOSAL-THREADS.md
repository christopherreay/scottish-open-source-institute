# PROPOSAL-THREADS — Live outline + threads for the Scottish Open Source Institute proposal

> This is the **live working spine** of the proposal. New research/content should be:
> 1) **linked here** into an existing thread, or
> 2) used to create a **new thread section**.
>
> We will tidy later; for now we optimize for capture + traceability.

- **Status:** Living document
- **Last updated:** 2026-02-03

## How to use this document (working rules)

When new material arrives:
- **Decide where it belongs**: an existing thread, or a new one.
- Add:
  - a short **claim/insight** summary (1–3 bullets)
  - **questions** it raises for Scotland
  - **links** to research artefacts (`research/...`) and any decisions (`decisions/...`)
  - (optional) a **costing hooks** note: what would need to be priced (capex/opex/headcount)

When writing the final proposal:
- Each thread becomes a section (or sub-section), with:
  - baseline option(s)
  - phased roadmap (timeframes)
  - cost ranges + assumptions
  - governance / delivery model

---

## Thread index (add freely)

### A. Framing: sovereignty + critical information flows
- A1. Operational definition of “sovereignty” for information flows
- A2. Identify Scotland’s **critical information flows** set (what counts / what doesn’t)
- A3. Threat model + dependency map (public-source feasible)

### B. Architecture: minimal viable sovereign baseline (Phase 1)
- B1. Core baseline capabilities (identity, messaging, DNS/time/PKI, incident comms, etc.)
- B2. Offline/partitioned operation + degraded modes
- B3. Security operations + incident response readiness

### C. Delivery & governance: what the Institute is / isn’t
- C1. Institute mandate and scope boundary
- C2. Operating model (OSPO-like functions, convening, reference architectures)
- C3. Procurement + standards leverage (policy levers)

### D. Cloud sovereignty strategy options (the “hyperscaler” question)
- D1. “No European hyperscalers” — constraints + implications
- D2. Sovereign wrapper models (e.g., France-style)
- D3. Hybrid segmentation (what stays on hyperscalers vs sovereign baseline)
- D4. Scotland/UK legal constraints & procurement realities

### E. Open source adoption patterns & comparators
- E1. EU / member-state policy inventory (what works, what failed)
- E2. Workplace / productivity migrations (Schleswig-Holstein, Denmark, etc.)
- E3. Municipal collaboration models (OS2, Sambruk)
- E4. Cross-border interoperability (X-Road / NIIS)

### F. Workstreams (“projects”) to include in the proposal
> Each workstream should become a costed project with timeframe options.
- F1. Capability map → project portfolio mapping
- F2. Prioritisation method (risk reduction vs cost vs time-to-value)
- F3. Delivery sequencing (Phase 0/1/2)

### G. Costing model
- G1. Costing method + assumptions catalogue
- G2. Scenario ranges (low/med/high) and uncertainty handling
- G3. Headcount model (Institute + delivery partners)

---

## Thread details (expand these over time)

### C1. Institute mandate and scope boundary
**Current position**
- Decision node exists; this is the working boundary for what the Institute does first.

**Questions**
- What are the initial “in-scope” capabilities for Phase 1 baseline in Scotland’s context?
- What governance is needed to keep the scope boundary enforceable?

**Links**
- `decisions/DEC-0001-institute-mandate-and-scope-boundary.md`

---

### D1. “No European hyperscalers” — constraints + implications
**Key claims/insights to validate**
- EU hyperscaler gap driven by capital structure, timing/scale effects, market fragmentation.
- EU providers strong on IaaS; weaker on breadth of managed services.

**Questions for Scotland**
- What workloads truly require hyperscaler-managed breadth vs can be delivered by a sovereign platform layer?
- What is the minimum internal platform engineering capacity needed for a “pure sovereignty” option?
- Where does “sovereign wrapper” reduce risk vs just relocate risk?

**Costing hooks**
- Platform engineering headcount (SRE/platform/security)
- Migration programme costs (applications, identity, data)
- Contracting/procurement transition costs

**Links**
- `research/2026-02-03-european-hyperscaler-gap-notes.md`

---

### E1. EU / member-state policy inventory
**Key claims/insights**
- Mature, replicable models exist (Switzerland law, Germany openDesk, Denmark phase-out, Italy reuse mandates).
- Patterns cluster into regulatory / operational / collaborative / regulatory-positioning approaches.

**Questions for Scotland**
- Which approaches are feasible under devolution + UK frameworks?
- What are the best comparators for Scotland (Wales, Ireland, Nordics, etc.)?

**Links**
- `research/2026-02-03-european-digital-sovereignty-policy-inventory.md`

---

## Parking lot (unassigned notes)
- Add anything here if you can’t yet decide where it belongs; we’ll triage later.
