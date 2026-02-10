# THR-0005 — Cost Model Development

## Summary
Credible capex/opex/headcount scenarios for Institute proposal: **£80-120M over 5 years (Moderate scenario)** delivering £105M in direct cost savings. Conservative scenario £45-65M; Ambitious £150-200M.

## Decisions
- **DEC-0008**: Cost model structure — **RECOMMENDED: Option B** (Moderate baseline + Conservative fallback)
- **DEC-0009**: Delivery timeline — 5-year phased approach; break-even Year 2-3

## Cost Summary by Scenario

| Scenario | 5-Year Total | Phase 1 (Y1-2) | Phase 2 (Y3-5) | Annual Run Rate | 5-Year Savings | Break-Even |
|----------|-------------|----------------|----------------|-----------------|----------------|------------|
| **Conservative** | £45-65M | £20-30M | £25-35M | £8-12M | £30M | Year 3 |
| **Moderate** | £80-120M | £35-50M | £45-70M | £15-22M | £105M | Year 2 |
| **Ambitious** | £150-200M | £60-80M | £90-120M | £28-38M | £265M | Year 3 |

## Axes / dimensions
- **Cost category**: capex (infrastructure) / opex (running) / headcount / training / risk reserve
- **Scenario**: conservative (minimal viable) / moderate / ambitious (comprehensive)
- **Phase**: Phase 0 (diagnosis) / Phase 1 (MVP baseline) / Phase 2 (expansion)
- **Time horizon**: Year 1 / Year 2 / Year 3 / 5-year total

## Comparator Benchmarks
- **Schleswig-Holstein**: €9M one-time, €15M annual savings (30,000 PCs) — Scottish equivalent €17M/€28M
- **Wales CDPS**: ~£3M annually (29 staff, coordination body)
- **Denmark OS2**: Municipal-funded, ~£2M annually shared costs, 84% council participation
- **Austria Bundesheer**: $6.5M annual savings (16,000 desktops to LibreOffice)

## Cost Structure (Moderate Scenario)

### CAPEX (One-Time): £53M
- Institute establishment: £3M
- Platform infrastructure: £25M (sovereign cloud, open source platforms, security)
- Migration costs: £25M (NHS, Government, Police, Councils)

### OPEX (Annual): £19M
- Institute operations: £5M (25 FTE)
- Platform operations: £12M
- Municipal collaboration: £2M

### Headcount (Moderate)
- Institute staff: 25 FTE
- Delivery partners: 75-100
- Total ecosystem: ~125

## Phase 1 (MVP Baseline): £35-50M
1. Institute establishment: £3M
2. NHS sovereign health cloud: £8M
3. Police/law enforcement platform: £5M
4. Government workplace pilot: £10M
5. Scottish OS2 (councils): £4M
6. Platform infrastructure: £15M
7. Risk reserve (15%): £5M

## Financing Options
1. Scottish Government core funding (annual grant)
2. Municipal cost-sharing (OS2 model)
3. **Hybrid (RECOMMENDED):** Core + project-specific + council contributions
4. Scottish National Investment Bank (patient capital for infrastructure)

## Cost Avoidance / Benefits
| Source | Annual (Moderate) | 5-Year |
|--------|-------------------|--------|
| Microsoft licensing reduction | £8M | £40M |
| AWS/Azure savings | £10M | £50M |
| Vendor lock-in risk reduction | £3M | £15M |
| **Total** | **£21M** | **£105M** |

## Unknowns / questions (Resolved)
- ✓ Comparable scale: Schleswig-Holstein × Scottish population factor
- ✓ Headcount models: Wales CDPS (coordination) + Germany ZenDiS (delivery)
- ✓ Cost avoidance: Microsoft licensing + cloud infrastructure quantified
- ✓ Do nothing baseline: Current £2.9B UK public sector cloud spend; Scottish proportion ~£150-200M annually

## Evidence / sources
- `research/2026-02-10-cost-model-framework.md` — **PRIMARY COSTING DOCUMENT**
- `research/2026-02-03-european-digital-sovereignty-policy-inventory.md` — comparator data
- `research/2026-02-10-requirements-hierarchy-military-basis.md` — Phase 1 scope

## Next actions
- [x] Define cost model structure decision (DEC-0008) — **RECOMMENDED Option B**
- [ ] Present cost ranges to John Bargman meeting
- [ ] Validate assumptions with Finance/costing experts
- [ ] Build detailed spreadsheet model with sensitivity analysis
- [ ] Develop risk-adjusted contingency recommendations
