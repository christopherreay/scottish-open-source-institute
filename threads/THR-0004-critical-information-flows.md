# THR-0004 — Critical Information Flows Taxonomy

## Summary
Develop a concrete taxonomy of Scotland's critical information flows to operationalize the scope boundary from DEC-0001. This thread produces the dependency mapping foundation.

## Decisions
- **DEC-0002**: Critical information flows taxonomy (needed)
- **DEC-0003**: Sovereignty measurement criteria (needed)

## Axes / dimensions
- **Criticality tier**: life-safety / government continuity / civil service / economic / convenience
- **Flow type**: identity / messaging / compute / storage / time/PKI / incident comms / payments
- **Current dependency**: hyperscaler / sovereign European / on-prem / mixed / unknown
- **Jurisdiction risk**: US-controlled / EU-controlled / UK-controlled / Scottish-controlled
- **Intervention leverage**: high (procurement levers exist) / medium / low (locked in)

## Unknowns / questions
- What is the exhaustive list of Scottish Government digital services?
- Which systems are currently on Azure/AWS/GCP vs. on-prem vs. other?
- What is the renewal timeline for major contracts?
- Which capabilities have no European alternative (yet)?

## Evidence / sources
- `docs/GOALS.md` — definitions
- `decisions/DEC-0001-institute-mandate-and-scope-boundary.md` — scope boundary rules
- `research/2026-02-03-european-digital-sovereignty-policy-inventory.md` — EU comparator approaches
- [To research]: Scotland's current cloud procurement data
- [To research]: NHS Scotland digital infrastructure map
- [To research]: Education Scotland (Glow) architecture

## Next actions
- [ ] FOI request or data call: Scottish public sector cloud spend 2023-2025
- [ ] Interview: NHS Scotland National Services Scotland (digital infrastructure)
- [ ] Interview: Education Scotland (Glow platform, Microsoft 365 education)
- [ ] Interview: Scottish Government CDO/Digital Scotland
- [ ] Compile initial taxonomy spreadsheet (capability × current provider × risk level)
