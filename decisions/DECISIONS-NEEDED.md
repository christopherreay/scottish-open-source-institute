# DECISIONS — Scottish Open Source Institute Proposal

## Decisions Made (Proposed)

| ID | Decision | Status | Date |
|---|---|---|---|
| DEC-0001 | Institute mandate + scope boundary | Proposed | 2026-02-03 |

---

## Decisions Needed

### Strategic Decisions (Pre-Meeting with John Bargman)

| ID | Decision | Context | Deadline |
|---|---|---|---|
| DEC-0002 | **Critical information flows taxonomy** — What specific capabilities satisfy "continuity-critical" threshold? | Needed for dependency mapping. Categories: identity, messaging, DNS/time/PKI, incident comms, etc. | Before meeting |
| DEC-0003 | **Sovereignty measurement criteria** — How to quantitatively measure "sovereignty-relevant dependency"? | Needed to evaluate options. Metrics: vendor concentration, jurisdiction risk, lock-in assessment. | Before meeting |
| DEC-0004 | **Strategic approach selection** — Pure sovereignty (Schleswig-Holstein) vs. sovereign wrapper (France S3NS/Bleu) vs. hybrid segmentation? | Core strategic choice affecting cost, timeline, and capability. See research on European models. | Meeting topic |
| DEC-0005 | **Governance model preference** — OSPO-style coordination? Delivery agency? Standards body? | Affects operating model and headcount. Reference: Germany's ZenDiS, France's DINUM, Denmark's OS2. | Meeting topic |

### Operational Decisions (Post-Meeting)

| ID | Decision | Context | Timeline |
|---|---|---|---|
| DEC-0006 | **Scope boundary application** — Specific in/out capabilities for Phase 0/1/2 | Apply DEC-0001 rules to concrete systems (NHS, education, civil service, etc.) | Week 1-2 |
| DEC-0007 | **Architecture baseline selection** — Which European provider(s) or models to evaluate? | OVHcloud? T-Systems? Open source stack? Hybrid? | Week 2-3 |
| DEC-0008 | **Cost model structure** — Scenario ranges: conservative / moderate / ambitious? | Capex/opex/headcount framing. 3-year vs 5-year horizon? | Week 2-3 |
| DEC-0009 | **Delivery timeline** — Phase 0 duration? Phase 1 MVP deadline? | Political constraints: election cycles, budget cycles | Week 3-4 |
| DEC-0010 | **Stakeholder engagement model** — Scottish Government, NHS Scotland, local authorities, private sector? | Who pays, who decides, who delivers? | Week 3-4 |

---

## Questions for John Bargman Meeting

### Understanding Context
1. What is the political mandate/timeline? Is this for a specific budget cycle or policy announcement?
2. Who are the key decision-makers? Digital Scotland? Cabinet Office? Finance?
3. What is the appetite for cost — are we talking £1M, £10M, £100M scale?
4. Are there existing initiatives we should align with or avoid duplicating?

### Strategic Direction
5. Is the priority defensive (reduce Microsoft/Google dependency) or generative (build indigenous capability)?
6. What's the risk tolerance for service breadth reduction? Can we trade features for sovereignty?
7. Are there "untouchable" systems (e.g., NHS Epic, specific Microsoft contracts)?

### Deliverables
8. What form does the output take? Formal proposal document? Cabinet submission? Public consultation?
9. Who is the audience? Ministers? Civil servants? Public? Tech community?
10. What is the hard deadline for delivery?

### Practical
11. Can we interview key stakeholders (NHS Scotland digital, Education Scotland, etc.)?
12. Is there existing work on critical information flows or dependency mapping?
13. What is Scotland's current cloud spend — any visibility into procurement data?

---

## Research Needed (Before Decisions)

| Topic | Source | Priority |
|---|---|---|
| Scotland's current cloud/digital procurement spend | Public contracts Scotland, G-Cloud data | High |
| NHS Scotland digital infrastructure | NHS National Services Scotland, open data | High |
| Education Scotland platforms | Glow, Microsoft 365 education data | Medium |
| Local government digital landscape | COSLA, improvement service | Medium |
| Existing Scottish Government cloud strategy | Digital Scotland, Scottish Tech Scaler | High |
| Comparable nations: Wales CDPS, Ireland digital strategy | Published strategies | Medium |
| Vendor landscape: current Scottish public sector contracts | FOI if needed | Medium |

---

## Thread Map

```
THR-0001 (Mandate/Scope) ──┬──→ DEC-0001 (Proposed)
                           ├──→ DEC-0002 (Taxonomy needed)
                           ├──→ DEC-0003 (Metrics needed)
                           └──→ DEC-0006 (Application)

THR-0002 (EU Research) ────┬──→ DEC-0004 (Strategic approach)
                           └──→ DEC-0007 (Architecture options)

THR-0003 (Hyperscaler) ────┬──→ DEC-0004 (Strategic approach)
                           └──→ DEC-0007 (Provider selection)

THR-0004 (Threat Model) ───┬──→ DEC-0002 (Taxonomy)
                           └──→ DEC-0003 (Metrics)

THR-0005 (Costing) ────────┬──→ DEC-0008 (Cost structure)
                           ├──→ DEC-0009 (Timeline)
                           └──→ DEC-0010 (Stakeholders)

THR-0006 (Governance) ─────┬──→ DEC-0005 (Governance model)
                           └──→ DEC-0010 (Stakeholders)
```
