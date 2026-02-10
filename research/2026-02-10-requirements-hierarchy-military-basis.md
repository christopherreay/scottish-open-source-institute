# Requirements Hierarchy: Military Basis for Digital Sovereignty

- **Date:** 2026-02-10
- **Purpose:** Filter 173 risk surfaces through DEC-0001 scope criteria on a "military" (operational continuity) basis
- **Method:** Apply three-filter test: (1) Continuity-critical, (2) Sovereignty-relevant, (3) Intervention-leverage

---

## Filter Methodology (DEC-0001 Applied)

A risk surface is **IN SCOPE** for the Institute only if it satisfies **ALL THREE**:

| Criterion | Test | Examples IN | Examples OUT |
|-----------|------|-------------|--------------|
| **1. Continuity-critical** | Required for government/civil continuity if disrupted | NHS patient records, emergency communications, benefit payments | Social media, entertainment streaming, non-essential services |
| **2. Sovereignty-relevant** | Meaningful coercive dependency risk | US CLOUD Act jurisdiction, single-vendor lock-in, extraterritorial legal exposure | Multi-vendor markets, EU-controlled infrastructure |
| **3. Intervention-leverage** | Institute can materially reduce risk via procurement, standards, architecture, or delivery support | Cloud procurement, open source alternatives, reference architectures | Reserved telecommunications regulation, UK-wide payment rails |

---

## TIER 1: Life-Safety / Emergency Response (Highest Priority)

**Definition:** Disruption risks immediate harm to life or catastrophic civil disorder.

| # | Risk Surface | Current State | Dependency Risk | Intervention |
|---|-------------|---------------|-----------------|--------------|
| 1.1 | **Emergency Services Network (ESN)** | EE (BT) network, £1.85bn UK Home Office contract, completion delayed to 2029 | UK-contracted; Scottish emergency responders dependent on non-Scottish contract | LOW — reserved matter, but Institute can document dependency |
| 1.2 | **Police Scotland Digital Evidence Sharing (DESC)** | Microsoft Azure UK datacentres; biometric data under US CLOUD Act jurisdiction | HIGH — law enforcement data subject to US extraterritorial reach | MEDIUM — procurement lever at renewal; sovereign alternative assessment |
| 1.3 | **NHS Emergency Patient Data** | National Digital Platform on AWS; 200,000 Microsoft licenses | HIGH — health emergency data on US cloud | HIGH — procurement lever; sovereign health cloud candidate |
| 1.4 | **Shetland/Orkney Connectivity** | SHEFA-2 submarine cable; 22,000 residents isolated Oct 2022 | HIGH — single cable, no Scottish redundancy authority | LOW — reserved telecommunications, but Institute can advocate |
| 1.5 | **Scottish Water SCADA Systems** | £50M cybersecurity contract; foreign SCADA vendors, default passwords common | MEDIUM — critical infrastructure control systems | MEDIUM — procurement standards; sovereign ICS assessment |
| 1.6 | **Energy Grid Control Systems** | SSEN/SP Transmission; 25% foreign-owned; Active Network Management | MEDIUM — foreign ownership, digital control surfaces | LOW-MEDIUM — limited devolved competence |

**TIER 1 IN SCOPE (3 of 6):** 1.2, 1.3, 1.5 (intervention-leverage exists)

---

## TIER 2: Government Continuity (High Priority)

**Definition:** Disruption prevents functioning of devolved government operations.

| # | Risk Surface | Current State | Dependency Risk | Intervention |
|---|-------------|---------------|-----------------|--------------|
| 2.1 | **Social Security Scotland Platform** | IBM Cúram; £5bn benefits for 1.8M people | HIGH — proprietary platform dependency | HIGH — renewal timeline; sovereign alternative assessment |
| 2.2 | **NHS Scotland Clinical Systems** | GP systems: EMIS, Vision/INPS, Microtest (£9.4M/year); vendor failure risk demonstrated | MEDIUM — vendor concentration, recent failures | HIGH — procurement framework lever |
| 2.3 | **Scottish Government Productivity (M365)** | Deep Microsoft 365 dependency post-COVID | HIGH — productivity/continuity tied to US platform | HIGH — Schleswig-Holstein model; openDesk assessment |
| 2.4 | **Local Government e-Counting** | Fujitsu/Idox contract; £12M 2027 tender | MEDIUM — proprietary e-counting for STV | HIGH — procurement lever; open source alternative |
| 2.5 | **Identity Authentication (myaccount)** | 2.9M users (59%); Improvement Service platform | MEDIUM — coverage gaps vs Estonia/Denmark | MEDIUM — sovereign identity expansion |
| 2.6 | **Scottish Courts/Tribunals (SCTS)** | Case management on Azure | HIGH — judicial data on US cloud | MEDIUM — procurement lever |
| 2.7 | **Procurement/Payment Systems** | Public spending dependent on foreign payment infrastructure | MEDIUM — operational but not immediately critical | MEDIUM — procurement standards |

**TIER 2 IN SCOPE (7 of 7):** All have intervention-leverage via procurement

---

## TIER 3: Critical Civil Services (Medium Priority)

**Definition:** Disruption causes significant civil hardship but not immediate government collapse.

| # | Risk Surface | Current State | Dependency Risk | Intervention |
|---|-------------|---------------|-----------------|--------------|
| 3.1 | **Education (Glow/Microsoft 365 Education)** | Entire Scottish schools system on Microsoft platform | HIGH — entire education digital infrastructure | HIGH — Schleswig-Holstein education model |
| 3.2 | **University Research Systems** | Dependent on US cloud for research data/compute | MEDIUM — academic freedom/research continuity | MEDIUM — sovereign research cloud |
| 3.3 | **Transport Systems (ScotRail)** | Now publicly owned but digital signalling vulnerable | MEDIUM — TfL attack cost £30M+ | LOW-MEDIUM — limited direct lever |
| 3.4 | **Cash Infrastructure** | LINK ATMs (6,350 in Scotland); Vocalink/Mastercard; G4S (US-owned) cash logistics | MEDIUM — offline payment resilience declining | LOW — UK-wide infrastructure |
| 3.5 | **Supply Chain Visibility** | NHS Supply Chain, logistics tracking foreign-controlled | MEDIUM — medical supply visibility | MEDIUM — procurement standards |

**TIER 3 IN SCOPE (4 of 5):** 3.1, 3.2, 3.4, 3.5

---

## TIER 4: Economic Infrastructure (Lower Priority)

**Definition:** Important for economic function but not immediate civil continuity.

| # | Risk Surface | Current State | Dependency Risk | Intervention |
|---|-------------|---------------|-----------------|--------------|
| 4.1 | **Challenger Bank Infrastructure** | Monzo, Starling, Revolut 100% AWS-based | HIGH — retail banking on US cloud | LOW — private sector, limited lever |
| 4.2 | **SME Digital Infrastructure** | 86% struggle to find skilled workers; £353M annual cost | MEDIUM — economic competitiveness | MEDIUM — workforce development |
| 4.3 | **Data Centre Capacity** | 37 facilities, 10-30MW current; 17 hyperscale planned | MEDIUM — potential hyperscaler dependency | MEDIUM — planning/investment incentives |

**TIER 4 IN SCOPE (2 of 3):** 4.2, 4.3

---

## TIER 5: Reserved/No Intervention Lever (Out of Scope)

| # | Risk Surface | Why Out of Scope |
|---|-------------|------------------|
| 5.1 | **Telecommunications regulation** | Reserved to Westminster (Scotland Act 1998, Schedule 5) |
| 5.2 | **Spectrum allocation** | Ofcom jurisdiction; no Scottish input |
| 5.3 | **Kill switch powers** | Communications Act 2003, Civil Contingencies Act 2004 — UK authority only |
| 5.4 | **SWIFT payment rails** | Belgium-based, UK-wide; requires independence for separate membership |
| 5.5 | **Card networks (Visa/Mastercard)** | Global duopoly; no Scottish regulatory lever |
| 5.6 | **Media ownership regulation** | Reserved broadcasting powers |
| 5.7 | **National security/counter-hybrid** | Reserved; NCSC coordination only |
| 5.8 | **Platform content moderation** | Online Safety Act enforced by Ofcom |

---

## Summary: In-Scope Requirements

| Tier | Risk Surfaces | Priority | Primary Intervention |
|------|--------------|----------|---------------------|
| **T1: Life-Safety** | 3 of 6 | CRITICAL | Sovereign cloud assessment, procurement standards |
| **T2: Gov Continuity** | 7 of 7 | HIGH | Procurement levers, open source alternatives |
| **T3: Critical Civil** | 4 of 5 | MEDIUM | Education/government platform sovereignty |
| **T4: Economic** | 2 of 3 | LOWER | Workforce development, planning incentives |
| **TOTAL IN SCOPE** | **16 of 21** | | |

---

## Phase 1: Minimal Viable Sovereign Baseline (Proposal Requirement)

**Definition:** The smallest set of capabilities that achieves meaningful sovereignty reduction for continuity-critical functions.

**Recommended Phase 1 Scope (from Tiers 1-2):**

1. **NHS Sovereign Health Cloud Platform** (T1.3)
   - Migrate National Digital Platform from AWS to sovereign/EU-controlled infrastructure
   - Replace Microsoft 365 with openDesk-style sovereign workplace
   - Timeline: 3-5 years
   - Cost: £15-30M (reference: Schleswig-Holstein €9M one-time for 30,000 PCs)

2. **Police/Law Enforcement Sovereign Platform** (T1.2)
   - DESC migration from Azure to sovereign cloud
   - Biometric data residency guarantee
   - Timeline: 2-3 years (contract renewal)
   - Cost: £5-10M

3. **Government Workplace Sovereignty** (T2.3)
   - Scottish Government M365 exit strategy
   - openDesk deployment (German proven model)
   - Timeline: 3-5 years
   - Cost: £10-20M (proportional to Schleswig-Holstein scale)

4. **Social Security Platform Sovereignty Assessment** (T2.1)
   - IBM Cúram dependency analysis
   - Open source alternative roadmap for next renewal
   - Timeline: Assessment year 1; implementation 2028-2030
   - Cost: £500K assessment; £20-40M implementation

5. **Municipal Open Source Collaboration (Scottish OS2)** (T2.4, T3.1)
   - Establish coordinating body for 32 councils
   - Shared open source codebases
   - Timeline: 2 years to establish
   - Cost: £2-3M annually (reference: Denmark OS2 runs on municipal contributions)

**Phase 1 Total Estimated Cost:** £50-100M over 5 years
- Capex: £30-60M (infrastructure, migration)
- Opex: £10-20M annually (platform operations)
- Headcount: 50-100 FTE across delivery

---

## Phase 2: Capability Expansion

- Identity infrastructure (myaccount → full e-ID)
- Education platform sovereignty (Glow replacement)
- Research cloud sovereignty
- Data embassy capability (Estonia model)
- Sub-national sovereignty framework (academic contribution)

---

## Critical Dependencies for Success

1. **Political mandate:** Scottish Government commitment to procurement-based sovereignty
2. **Council participation:** At least 50% of 32 councils for OS2-equivalent
3. **UK coordination:** Reserved matters require UK engagement (even if no control)
4. **International partnerships:** X-Road/NIIS, Wales CDPS, Nordic cooperation
5. **Workforce:** Platform-agnostic skills development (vendor certification exit)

---

## Key Uncertainties

- **Contract renewal timelines:** NHS AWS (2020+10yr?), Police Azure (unknown), Social Security IBM (unknown)
- **Political durability:** Multi-year commitment across government terms
- **Devolution constraints:** Can procurement levers alone achieve meaningful sovereignty?
- **Technical feasibility:** Are open source alternatives mature enough for all use cases?
