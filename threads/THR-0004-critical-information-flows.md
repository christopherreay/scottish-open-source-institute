# THR-0004 — Critical Information Flows Taxonomy

## Summary
Comprehensive taxonomy identifying **173 distinct risk surfaces** across **13 dimensions** where external actors could attack, disrupt, or control Scotland's information infrastructure. Key finding: Scotland has "service sovereignty without infrastructure sovereignty"—devolved control over services (health, education, justice) but reserved telecommunications, broadcasting, and national security powers leaving critical infrastructure under UK/foreign control.

## Decisions
- **DEC-0002**: Critical information flows taxonomy (completed — see research/2026-02-10-information-flow-sovereignty-taxonomy.md)
- **DEC-0003**: Sovereignty measurement criteria (needed)
- **DEC-0011**: Devolved digital sovereignty framework (needed — no academic literature exists for sub-national sovereignty)

## Axes / dimensions
The taxonomy maps risk across 13 independent dimensions:

1. **Physical infrastructure layer** (23 risk surfaces) — submarine cables, terrestrial fiber, mobile towers, data centres
2. **Telecommunications and connectivity** (12) — kill switch capabilities, internet exchange architecture
3. **Essential civic services** (18) — NHS Scotland, Social Security Scotland, electoral systems
4. **Financial information infrastructure** (21) — payment rails, challenger banks, SWIFT, cash systems
5. **Identity and authentication** (11) — myaccount, voter registration, biometric systems
6. **Democratic and media flows** (19) — media ownership, platform dependencies, disinformation
7. **Critical infrastructure control** (16) — SCADA/ICS, energy grid, transport systems
8. **Supply chain dependencies** (9) — logistics tracking, NHS Supply Chain
9. **Software and platforms** (18) — OS control surfaces, cloud concentration, app store gatekeeping
10. **Data sovereignty** (12) — CLOUD Act jurisdiction, GDPR adequacy, data residency
11. **Human capital** (6) — skills crisis, vendor certification lock-in
12. **Legal and regulatory** (8) — Schedule 5 reservations, regulatory gaps
13. **Economic levers** (procurement as primary tool)

## Critical single points of failure
1. **SHEFA-2 submarine cable** — 22,000 Shetland residents lost connectivity Oct 2022
2. **Dunnet Bay landing station** — FARICE-1 termination
3. **London backhaul routes** — Scottish traffic transits south
4. **EE network** — sole Emergency Services Network provider
5. **Vocalink/Mastercard** — all UK interbank payments infrastructure
6. **AWS** — NHS Scotland National Digital Platform (£15m/10yr contract)
7. **Microsoft Azure** — Police Scotland DESC (biometric data under US jurisdiction)

## Highest-impact foreign control risks
1. **US CLOUD Act** — extraterritorial data access regardless of storage location
2. **SWIFT disconnection** — demonstrated against Russia 2022
3. **Card network withdrawal** — Visa/Mastercard dependency
4. **Platform content decisions** — Meta/Google/X algorithmic control
5. **Kill switch powers** — Communications Act 2003, Civil Contingencies Act 2004

## Small nation comparators
| Country | Model | Key Achievement | Applicability to Scotland |
|---------|-------|-----------------|---------------------------|
| **Estonia** | X-Road federated architecture | 450+ orgs, 3,000+ services, Data Embassy in Luxembourg | High — open source, peer-to-peer, no central DB |
| **Denmark** | OS2 municipal collaboration | 82/98 municipalities (84%) sharing 25 open source codebases | High — procurement-based, council collaboration |
| **Norway** | Altinn business-government platform | 90%+ population, 15bn NOK annual savings, open source | Medium — requires central platform investment |
| **Wales** | CDPS arm's-length body | 29 staff coordinating digital transformation | High — devolved context, similar constraints |
| **Switzerland** | EMBAG legal mandate | "Public Money, Public Code" federal law (2024) | Medium — requires legislative competence |

## Unknowns / questions
- Which of the 173 risk surfaces fall within Institute intervention scope under DEC-0001 criteria?
- What is the costed roadmap for addressing Tier 1 risks (life-safety / government continuity)?
- Can procurement levers realistically shift provider mix given contract lock-in periods?
- What are the renewal timelines for major contracts (AWS NHS, Azure Police Scotland, etc.)?

## Evidence / sources
- `research/2026-02-10-information-flow-sovereignty-taxonomy.md` — **PRIMARY SOURCE** (173 risk surfaces, 13 dimensions)
- `docs/GOALS.md` — definitions
- `decisions/DEC-0001-institute-mandate-and-scope-boundary.md` — scope boundary rules
- `research/2026-02-03-european-digital-sovereignty-policy-inventory.md` — EU comparator approaches
- `research/2026-02-03-european-hyperscaler-gap-notes.md` — provider landscape analysis

## Next actions
- [ ] Apply DEC-0001 scope boundary rules to filter 173 risk surfaces to in-scope set
- [ ] Prioritise risk surfaces by: impact × likelihood × intervention leverage
- [ ] Cost minimal viable sovereign baseline (Phase 1 per SCOPE.md)
- [ ] Interview: NHS Scotland National Services Scotland (AWS contract renewal timeline)
- [ ] Interview: Police Scotland (Azure DESC contract details)
- [ ] Interview: Scottish Government CDO (procurement lever assessment)
