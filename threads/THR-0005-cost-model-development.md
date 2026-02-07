# THR-0005 — Cost Model Development

## Summary
Build a costed, phased proposal with capex/opex/headcount scenarios. Must be credible to Finance and comparable to European models.

## Decisions
- **DEC-0008**: Cost model structure (needed)
- **DEC-0009**: Delivery timeline (needed)

## Axes / dimensions
- **Cost category**: capex (infrastructure) / opex (running) / headcount / training / risk reserve
- **Scenario**: conservative (minimal viable) / moderate / ambitious (comprehensive)
- **Phase**: Phase 0 (diagnosis) / Phase 1 (MVP baseline) / Phase 2 (expansion)
- **Time horizon**: Year 1 / Year 2 / Year 3 / 5-year total

## Unknowns / questions
- What is comparable scale? Schleswig-Holstein (€15M saved, €9M invested)? Denmark (national)?
- What headcount models work? OSPO (small, catalytic) vs. delivery agency (large, implementing)?
- What cost avoidance can we claim? Microsoft licensing, cloud egress, vendor lock-in risk?
- What is the "do nothing" cost baseline?

## Evidence / sources
- `docs/SCOPE.md` — phases and deliverables
- `decisions/DEC-0001-institute-mandate-and-scope-boundary.md` — scope affects cost
- `research/2026-02-03-european-digital-sovereignty-policy-inventory.md`:
  - Schleswig-Holstein: €15M annual savings, €9M one-time investment
  - Germany openDesk: 70,000+ licenses, federal-scale
  - France S3NS/Bleu: commercial pricing
  - Denmark OS2: municipal collaboration model
- [To research]: Scottish public sector IT spend baseline
- [To research]: Comparable scale nations (Wales, Ireland, Nordic countries)

## Costing approach options
1. **Bottom-up**: Estimate per-system migration costs × number of systems
2. **Top-down**: Percentage of IT spend redirected (Schleswig-Holstein model)
3. **Comparable**: Direct adaptation from similar jurisdiction
4. **Scenario-based**: Three scenarios with ranges for key variables

## Next actions
- [ ] Define cost model structure decision (DEC-0008)
- [ ] Gather Scottish IT spend baseline data
- [ ] Build scenario model spreadsheet
- [ ] Validate assumptions with Finance/costing experts
- [ ] Produce draft cost ranges for John Bargman meeting
