# Cost Model Framework: Scottish Open Source Institute

- **Date:** 2026-02-10
- **Status:** Draft for DEC-0008 decision
- **Purpose:** Credible capex/opex/headcount scenarios for Institute proposal

---

## Executive Summary

| Scenario | 5-Year Total | Phase 1 (Y1-2) | Phase 2 (Y3-5) | Annual Run Rate |
|----------|-------------|----------------|----------------|-----------------|
| **Conservative** | £45-65M | £20-30M | £25-35M | £8-12M |
| **Moderate** | £80-120M | £35-50M | £45-70M | £15-22M |
| **Ambitious** | £150-200M | £60-80M | £90-120M | £28-38M |

**Key comparators:**
- Schleswig-Holstein: €9M one-time, €15M annual savings (30,000 PCs)
- Wales CDPS: ~£3M annually (29 staff, coordination body)
- Denmark OS2: Municipal-funded, ~£2M annually shared costs
- Austria Bundesheer: $6.5M annual savings (16,000 desktops to LibreOffice)

---

## Costing Methodology

**Hybrid approach: Comparable × Scottish Scale × Scenario Factor**

1. **Baseline:** Schleswig-Holstein migration (proven, documented)
2. **Scale factor:** Scotland vs. Schleswig-Holstein population (5.5M vs. 2.9M = 1.9x)
3. **Complexity factor:** NHS + Police + Government + Councils vs. single state
4. **Scenario factor:** Conservative (0.7x) / Moderate (1.0x) / Ambitious (1.5x)

---

## Cost Structure

### 1. CAPEX (One-Time Investment)

| Category | Conservative | Moderate | Ambitious |
|----------|-----------|----------|-----------|
| **Institute establishment** | £2M | £3M | £5M |
| Office, legal, governance setup | £0.5M | £0.5M | £1M |
| Initial staff recruitment | £0.5M | £1M | £2M |
| Systems/setup | £1M | £1.5M | £2M |
| **Platform infrastructure** | £10M | £25M | £50M |
| Sovereign cloud build/buy | £5M | £15M | £30M |
| Open source platform deployment | £3M | £7M | £15M |
| Security/accreditation | £2M | £3M | £5M |
| **Migration costs** | £10M | £25M | £50M |
| NHS NDP migration (AWS → sovereign) | £3M | £8M | £15M |
| Government M365 exit | £4M | £10M | £20M |
| Police Azure migration | £2M | £5M | £10M |
| Council systems | £1M | £2M | £5M |
| **TOTAL CAPEX** | **£22M** | **£53M** | **£105M** |

### 2. OPEX (Annual Operating)

| Category | Conservative | Moderate | Ambitious |
|----------|-----------|----------|-----------|
| **Institute operations** | £3M | £5M | £8M |
| Staff (15 / 25 / 40 FTE) | £1.5M | £2.5M | £4M |
| Facilities/overhead | £0.5M | £1M | £2M |
| Research/advocacy | £1M | £1.5M | £2M |
| **Platform operations** | £5M | £12M | £25M |
| Sovereign cloud opex | £3M | £8M | £18M |
| Open source maintenance | £1M | £2M | £4M |
| Security operations | £1M | £2M | £3M |
| **Municipal collaboration (OS2 equiv)** | £1M | £2M | £3M |
| Coordination body | £0.5M | £1M | £1.5M |
| Shared codebase maintenance | £0.5M | £1M | £1.5M |
| **TOTAL OPEX (Annual)** | **£9M** | **£19M** | **£36M** |

### 3. Headcount

| Scenario | Institute Staff | Delivery Partners | Total Ecosystem |
|----------|-----------------|-------------------|-----------------|
| **Conservative** | 15 FTE | 30-50 | ~65 |
| **Moderate** | 25 FTE | 75-100 | ~125 |
| **Ambitious** | 40 FTE | 150-200 | ~240 |

**Roles (Moderate scenario example):**
- Executive: 3 (CEO, COO, CFO)
- Technical: 10 (platform, security, architecture)
- Delivery: 8 (council liaison, NHS coordination, gov engagement)
- Research/Policy: 4 (sovereignty framework, procurement)

---

## Scenario Definitions

### Conservative Scenario
**Definition:** Minimum viable sovereignty — demonstrate capability, single major migration, limited scope

**Scope:**
- Institute established as coordination body (Wales CDPS model)
- NHS NDP migration only (crown jewel approach)
- 8-12 council participation (OS2 pilot)
- No government M365 exit
- Open source preference policy only (no mandate)

**Rationale:** Prove concept with lowest risk; expand based on demonstrated success

---

### Moderate Scenario
**Definition:** Meaningful sovereignty reduction across critical services; comparable to Schleswig-Holstein achievement

**Scope:**
- Full Institute capability (delivery + coordination)
- NHS NDP + Police DESC migration
- Government M365 phased exit (pilot departments)
- 20+ council OS2 participation
- Sovereign cloud platform operational

**Rationale:** Achieves "minimum viable sovereign baseline" from SCOPE.md Phase 1; credible comparator to European examples

---

### Ambitious Scenario
**Definition:** Comprehensive sovereignty across devolved services; Scotland as European leader

**Scope:**
- Institute as major delivery body (Germany ZenDiS scale)
- All Tier 1-2 risk surfaces addressed
- Full government M365 exit
- All 32 councils in OS2
- Sovereign research cloud
- Data embassy capability
- Sub-national sovereignty framework (academic contribution)

**Rationale:** Positions Scotland alongside Estonia/Norway as digital sovereignty exemplar

---

## Cost Avoidance / Benefit Quantification

### Direct Savings (Quantifiable)

| Source | Conservative | Moderate | Ambitious |
|--------|-------------|----------|-----------|
| Microsoft licensing reduction | £2M/yr | £8M/yr | £20M/yr |
| AWS/Azure egress/infra savings | £3M/yr | £10M/yr | £25M/yr |
| Vendor lock-in risk reduction | £1M/yr | £3M/yr | £8M/yr |
| **Annual Savings** | **£6M** | **£21M** | **£53M** |
| **5-Year Savings** | **£30M** | **£105M** | **£265M** |

**ROI Timeline:**
- Conservative: Break-even Year 3; positive ROI Year 4
- Moderate: Break-even Year 2; positive ROI Year 3
- Ambitious: Break-even Year 3; positive ROI Year 4

### Strategic Benefits (Non-Quantified)

- **Resilience:** Operational continuity under connectivity partition
- **Sovereignty:** Data outside US CLOUD Act jurisdiction
- **Capability:** Indigenous digital skills and platforms
- **Agility:** Reduced vendor lock-in enables faster change
- **Reputation:** European leadership in sub-national digital sovereignty

---

## Comparator Benchmarking

### Schleswig-Holstein (Germany)
- **Scale:** 2.9M population; 30,000 PCs
- **Investment:** €9M one-time (2019 euros)
- **Savings:** €15M annually from 2026
- **Scottish equivalent:** €17M one-time (1.9x scale); €28M annual savings
- **Lessons:** Migration took 5+ years; legal mandate critical; procurement lever essential

### Wales CDPS
- **Scale:** 3.1M population; 22 councils
- **Investment:** ~£3M annually (operational budget)
- **Staff:** 29 permanent
- **Scope:** Coordination body, not delivery agency
- **Scottish equivalent:** £3-5M annually for coordination function
- **Lessons:** Arm's-length body enables cross-organizational coordination

### Denmark OS2
- **Scale:** 5.9M population; 98 municipalities
- **Investment:** Municipal-funded (shared costs)
- **Participation:** 82/98 councils (84%)
- **Scottish equivalent:** £1-2M annually for coordination + council contributions
- **Lessons:** Procurement law clarification enabled open source specification

### Austria Bundesheer
- **Scale:** 16,000 desktops
- **Investment:** Not published (migration costs)
- **Savings:** $6.5M annually (Microsoft license elimination)
- **Scottish equivalent:** ~$13M annually for 30,000 government desktops
- **Lessons:** Military-grade security achievable on open source; training investment essential

---

## Risk Adjustments

| Risk | Probability | Cost Impact | Mitigation |
|------|-------------|-------------|------------|
| **Contract lock-in** | HIGH | +20-30% | Negotiate early exit; wait for renewal cycles |
| **Skills shortage** | MEDIUM | +15-25% | Invest in training; partner with universities |
| **Vendor retaliation** | LOW | +10-15% | Phased approach; maintain relationships |
| **Political change** | MEDIUM | Programme risk | Cross-party support; evidence-based case |
| **Technical failures** | LOW | +10-20% | Pilot approach; proven platforms only |

**Recommended Risk Reserve:** 15-20% on top of base estimates

---

## Financing Options

### Option 1: Scottish Government Core Funding
- **Model:** Annual grant (Wales CDPS approach)
- **Pros:** Direct accountability; stable funding
- **Cons:** Subject to budget cycles; political exposure
- **Fit:** Conservative/Moderate scenarios

### Option 2: Municipal Cost-Sharing (OS2 Model)
- **Model:** Council contributions based on usage/participation
- **Pros:** Aligns incentives; shared ownership
- **Cons:** Coordination overhead; uneven participation
- **Fit:** Municipal collaboration components

### Option 3: Hybrid (Recommended)
- **Model:** Core government funding + project-specific funding + council contributions
- **Example:** £3M core + £5M NHS migration funding + £1M council pool
- **Pros:** Diversified risk; aligned incentives
- **Cons:** Complex governance
- **Fit:** All scenarios

### Option 4: Scottish National Investment Bank
- **Model:** Patient capital for infrastructure
- **Pros:** Off-budget; commercial discipline
- **Cons:** Return requirements; limited grant capacity
- **Fit:** Sovereign cloud platform capex

---

## Recommended Approach for Proposal

**Present Moderate scenario as baseline with Conservative as fallback:**

> "The Scottish Open Source Institute requires £80-120M over 5 years (Moderate scenario), delivering £105M in direct cost savings and strategic sovereignty benefits. A minimum viable approach (Conservative) delivering reduced but meaningful sovereignty requires £45-65M. Full European leadership (Ambitious) requires £150-200M."

**Key financial metrics to highlight:**
- Break-even: Year 2-3
- 5-year ROI: 30-120% depending on scenario
- Annual savings at steady state: £21M+ (Moderate)
- Risk-adjusted: Add 15% contingency

---

## Decision Required: DEC-0008

**Question:** Which cost model structure should the proposal adopt?

| Option | Structure | Use Case |
|--------|-----------|----------|
| A | Conservative only (safe) | Risk-averse Finance; pilot approach |
| B | Moderate baseline + Conservative fallback | Balanced; most credible |
| C | All three scenarios with decision gates | Political buy-in; phased commitment |
| D | Top-down (% of IT spend) | Simple messaging; hard to validate |

**Recommendation:** Option B (Moderate baseline) — demonstrates ambition with credible fallback
