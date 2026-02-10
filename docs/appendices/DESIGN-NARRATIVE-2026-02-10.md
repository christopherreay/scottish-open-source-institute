# DESIGN — Working notes

This document captures architecture options, tradeoffs, and evolving design for the Scottish Open Source Institute proposal.

---

## 1. Capability Map

### What the Institute MUST Deliver (Non-Negotiable)

| Capability | Purpose | How |
|------------|---------|-----|
| **Dependency Observatory** | Continuous monitoring of 173 risk surfaces | Research + automated scanning + intelligence partnerships |
| **Procurement Influence** | Sovereignty requirements in public sector buying | Standards, reference architectures, buying consortium |
| **Open Source Coordination** | Scottish OS2 equivalent for municipal collaboration | Shared codebases, procurement frameworks, legal clarity |
| **Sovereign Platform Delivery** | Reduce hyperscaler dependency for critical services | Cloud platform, workplace suite, migration services |
| **Workforce Development** | Platform-agnostic skills, vendor independence | Training partnerships, certification alternatives |

### What the Institute WILL NOT Deliver (Explicit Boundary)

| Out of Scope | Why | Who Does |
|--------------|-----|----------|
| Telecommunications regulation | Reserved to Westminster | Ofcom, UK Government |
| National security operations | Reserved; NCSC role | NCSC, Police Scotland |
| Payment rail infrastructure | UK-wide; SWIFT, Vocalink | Bank of England, private sector |
| Media ownership regulation | Reserved broadcasting | Ofcom |
| All implementation | Catalytic, not monolithic | Delivery partners, councils, NHS |

---

## 2. Threat Model Summary

### Critical Dependency Risks (Tiers 1-2)

| Risk | Likelihood | Impact | Current Mitigation | Institute Role |
|------|------------|--------|-------------------|----------------|
| US CLOUD Act data access | CERTAIN | HIGH | None acknowledged | Sovereign platform alternative |
| AWS/Azure service withdrawal | LOW | CRITICAL | None | Multi-provider strategy |
| Microsoft licensing coercion | MEDIUM | HIGH | Limited alternatives | Open source exit path |
| Submarine cable partition | LOW | CRITICAL | None (reserved) | Document + advocate |
| ESN failure/delay | HIGH | HIGH | UK Home Office | Monitor + contingency |
| SCADA/ICS compromise | MEDIUM | HIGH | £50M MSS contract | Sovereign ICS assessment |

### Sovereignty-Relevant vs. Reserved (Devolution Map)

```
┌─────────────────────────────────────────────────────────────────┐
│  RESERVED (Westminster)                                         │
│  ───────────────────────                                         │
│  • Telecommunications regulation                                │
│  • Spectrum allocation                                          │
│  • Kill switch powers                                           │
│  • National security                                            │
│  • SWIFT/card payment rails                                     │
│  • Media/broadcasting regulation                                │
│                                                                 │
│  Institute role: Document, advocate, coordinate                 │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│  DEVOLVED (Scottish Government)                                 │
│  ───────────────────────────────                                 │
│  • Public sector procurement  ←←← PRIMARY LEVER                 │
│  • NHS service delivery                                         │
│  • Police/law enforcement systems                               │
│  • Social Security Scotland                                     │
│  • Education (Glow, schools)                                    │
│  • Local government services                                    │
│  • Planning/economic development                                │
│                                                                 │
│  Institute role: Direct intervention, standards, delivery       │
└─────────────────────────────────────────────────────────────────┘
```

---

## 3. Architecture Options

### Option A: Coordination Body (Wales CDPS Model)

**Structure:** Arm's-length body, 20-30 staff, £3-5M annually

**Functions:**
- Standards and reference architectures
- Procurement guidance
- Municipal coordination
- Research and advocacy

**Delivery:** Catalytic — enables others to deliver

**Pros:**
- Lower cost, lower risk
- Fits devolution constraints
- Proven model (Wales)

**Cons:**
- Limited direct sovereignty reduction
- Dependent on partner buy-in
- Slower impact

**Fit:** Conservative scenario

---

### Option B: Delivery Agency (Germany ZenDiS Model)

**Structure:** Government agency, 50-100 staff, £15-25M annually

**Functions:**
- Direct platform operation (sovereign cloud)
- Application migration and support
- Municipal shared services
- Workforce development

**Delivery:** Direct — Institute builds and operates

**Pros:**
- Maximum sovereignty reduction
- Faster implementation
- Clear accountability

**Cons:**
- Higher cost, higher risk
- Requires sustained political commitment
- Scale challenges

**Fit:** Ambitious scenario

---

### Option C: Hybrid (RECOMMENDED)

**Structure:** Arm's-length body with delivery capability, 25-40 staff, £8-18M annually

**Functions:**
- **Core:** Standards, procurement, coordination (like Wales)
- **Delivery:** Sovereign platform for priority systems (NHS, Police, critical)
- **Catalytic:** Enable council/NHS delivery of their own migrations

**Delivery:** Mixed — direct for crown jewels, enable for rest

**Pros:**
- Balanced risk/impact
- Proves concept before scaling
- Retains flexibility

**Cons:**
- Complex governance
- Dual focus challenges

**Fit:** Moderate scenario (baseline recommendation)

---

### Platform Architecture Options

#### Cloud Strategy

| Option | Description | Sovereignty | Cost | Risk |
|--------|-------------|-------------|------|------|
| **A. European IaaS** | OVHcloud, T-Systems, Scaleway | HIGH (EU-controlled) | Lower | Broader service gaps |
| **B. Sovereign Wrapper** | Scottish-owned entity running hyperscaler tech | MEDIUM (legal, not technical) | Medium | Maintains vendor dependency |
| **C. Scottish Government Cloud** | Self-operated OpenStack/Kubernetes | HIGHEST | Higher | Skills, operational risk |
| **D. Hybrid** (RECOMMENDED) | Sovereign for sensitive; European for general; hyperscaler for non-critical | TIERED | Optimized | Complexity |

**Recommendation:** Option D (Hybrid Tiered)
- Tier 1 (life-safety): Scottish/European sovereign only
- Tier 2 (gov continuity): European sovereign preferred
- Tier 3 (non-critical): Market competitive

#### Workplace Suite Strategy

| Option | Description | Reference |
|--------|-------------|-----------|
| **A. openDesk** (Germany) | Proven 70,000+ licenses, complete suite | Schleswig-Holstein, Federal Ministries |
| **B. Municipal stack** | Best-of-breed open source (Nextcloud, Collabora, Jitsi) | Denmark OS2 components |
| **C. Phased exit** | LibreOffice + gradual service replacement | Austria Bundesheer |
| **D. Hybrid retention** | Keep some Microsoft, reduce dependency | France (mixed approach) |

**Recommendation:** Option A (openDesk) for government; Option B (municipal stack) for councils

---

## 4. Governance Model

### Organizational Structure (Hybrid Model)

```
┌─────────────────────────────────────────────────────────────┐
│                    BOARD OF DIRECTORS                        │
│           (Scottish Government + Council reps +              │
│            Independent + Academic)                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                 CHIEF EXECUTIVE OFFICER                      │
└─────────────────────────────────────────────────────────────┘
                              │
        ┌─────────────────────┼─────────────────────┐
        │                     │                     │
        ▼                     ▼                     ▼
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│  COO         │     │  CTO         │     │  Policy &    │
│  Operations  │     │  Technology  │     │  Research    │
└──────────────┘     └──────────────┘     └──────────────┘
        │                     │                     │
   ┌────┴────┐           ┌────┴────┐          ┌────┴────┐
   │         │           │         │          │         │
   ▼         ▼           ▼         ▼          ▼         ▼
Delivery  Municipal   Platform  Security   Research  Advocacy
Partners  Coordination Team     Team       Team      Team
```

### Funding Governance

| Source | Proportion | Governance |
|--------|-----------|------------|
| Scottish Government core | 50-60% | Annual grant, performance milestones |
| Project-specific funding | 25-35% | NHS, Police, council contributions |
| Municipal cost-sharing | 10-15% | OS2-style participation fees |
| Research/innovation grants | 5-10% | EU, research council funding |

### Accountability Framework

- **To Scottish Government:** Strategic objectives, budget, sovereignty outcomes
- **To Councils:** Service standards, participation value
- **To Parliament:** Annual reporting, transparency
- **To Public:** Open source code, open data, public reporting

---

## 5. Costing Approach

### Financial Model Summary

| Scenario | 5-Year Investment | 5-Year Savings | Net | Break-Even |
|----------|------------------|----------------|-----|------------|
| Conservative | £45-65M | £30M | (£15-35M) | Year 3 (savings only) |
| **Moderate** | **£80-120M** | **£105M** | **-£15M to +£25M** | **Year 2** |
| Ambitious | £150-200M | £265M | +£65-115M | Year 3 |

**Note:** Conservative scenario has negative direct ROI but delivers strategic sovereignty benefits not quantified here.

### Cost Categories (Moderate Scenario)

```
5-YEAR COST BREAKDOWN: £80-120M

CAPEX (One-Time): £53M
├── Institute setup          £3M   ████
├── Platform infrastructure £25M   ███████████████████████████
├── Migration costs         £25M   ███████████████████████████

OPEX (Annual, ×5 years): £95M
├── Institute operations    £25M   ███████████████████████████████
├── Platform operations     £60M   ████████████████████████████████████████████████████████████████████████
└── Municipal collaboration £10M   ████████████████

Total: £148M (high estimate) to £98M (low estimate)
```

### Sensitivity Analysis

| Variable | -20% | Base | +20% |
|----------|------|------|------|
| Migration complexity | £64M | £80M | £96M |
| Cloud infrastructure cost | £96M | £120M | £144M |
| Staff cost inflation | £72M | £80M | £88M |
| Council participation rate | £100M | £80M | £70M |

**Most sensitive:** Cloud infrastructure costs, migration complexity
**Least sensitive:** Staff costs (within normal ranges)

---

## 6. Delivery Plan / Milestones

### Phase 0: Foundation (Months 1-12)

| Month | Milestone | Deliverable |
|-------|-----------|-------------|
| 3 | Institute established | Legal entity, board, CEO appointed |
| 6 | Observatory operational | Risk surface monitoring active |
| 9 | NHS assessment complete | Migration feasibility, costed options |
| 12 | OS2 pilot launched | 8-12 councils committed |

**Budget:** £5-8M
**Staff:** 10-15 FTE

### Phase 1: MVP Baseline (Months 12-36)

| Quarter | Milestone | Deliverable |
|---------|-----------|-------------|
| Q5 | Sovereign platform live | NHS NDP migration begins |
| Q6 | Government pilot | 2-3 departments on openDesk |
| Q8 | Police migration | DESC on sovereign platform |
| Q10 | OS2 expansion | 20+ councils participating |
| Q12 | Phase 1 review | Sovereignty metrics, Phase 2 scope |

**Budget:** £30-42M (cumulative)
**Staff:** 20-30 FTE

### Phase 2: Expansion (Months 36-60)

| Year | Milestone | Deliverable |
|------|-----------|-------------|
| 4 | Full NHS migration | All critical systems sovereign |
| 4 | Government exit | 50% M365 replacement |
| 5 | OS2 complete | All 32 councils participating |
| 5 | Data embassy | Estonia-style capability explored |
| 5 | Framework published | Sub-national sovereignty methodology |

**Budget:** £45-70M additional
**Staff:** 30-40 FTE

### Critical Path Dependencies

```
Year 1                Year 2                Year 3                Year 4                Year 5
  │                     │                     │                     │                     │
  ├── Institute setup ──┤                     │                     │                     │
  ├─── Observatory ─────┤                     │                     │                     │
  │                     ├── NHS migration ────┤                     │                     │
  │                     ├── Police migration ─┤                     │                     │
  │                     ├── Gov pilot ────────┼── Gov expansion ────┤                     │
  └── OS2 pilot ────────┼── OS2 expansion ────┼── OS2 full ─────────┘                     │
                                              │                                           │
                                              └────── Sovereign baseline achieved ──────────┘
```

### Go/No-Go Decision Gates

| Gate | Criteria | Decision |
|------|----------|----------|
| **Gate 1** (M12) | Observatory credible? NHS migration viable? Council interest? | Proceed to Phase 1 / Pivot / Halt |
| **Gate 2** (M24) | NHS migration on track? Government pilot successful? | Expand scope / Maintain / Contract |
| **Gate 3** (M36) | Sovereignty metrics positive? ROI tracking? | Proceed to Phase 2 / Optimise / Exit |

---

## 7. Risk Mitigation

### Strategic Risks

| Risk | Mitigation |
|------|------------|
| Political change | Cross-party framework; evidence-based case; international alignment |
| Vendor retaliation | Phased approach; maintain relationships; legal safeguards |
| Skills shortage | University partnerships; training investment; international recruitment |
| Technical failure | Pilot approach; proven platforms; rollback plans |
| Cost overrun | 15% contingency; fixed-price contracts; stage gates |

### Devolution Risks

| Risk | Mitigation |
|------|------------|
| Reserved matter conflict | Clear scope boundaries; UK coordination; legal review |
| Procurement limits | Test limits; document gaps; advocate for expansion |
| Council non-participation | Incentive design; shared savings; phased opt-in |

---

## 8. Success Metrics

### Operational Metrics (Monthly)

- Risk surfaces monitored: 173
- Observatory reports issued: 12/year
- Council OS2 participation: % of 32
- Platform uptime/sovereignty: %

### Outcome Metrics (Annual)

- Systems migrated to sovereign platforms: count
- Hyperscaler dependency reduction: %
- Cost savings realized: £M
- Open source code releases: count
- Platform-agnostic staff certified: count

### Strategic Metrics (Phase-end)

- Tier 1-2 risk surfaces addressed: %
- Scottish control over critical flows: improved/not
- Resilience to partition scenario: tested
- European comparator ranking: position

---

## 9. Open Questions / Decisions Needed

1. **DEC-0008:** Cost model structure — Option B (Moderate baseline) recommended
2. **DEC-0009:** Delivery timeline — 5-year phased with gates confirmed
3. **DEC-0010:** Governance model — Hybrid (coordination + delivery) confirmed
4. **DEC-0011:** Devolved sovereignty framework — Research publication target Year 5
5. **DEC-0012:** John Bargman meeting scope — What decisions needed from meeting?

---

*Last updated: 2026-02-10*
