# Why there are no European hyperscalers — notes + rough provider landscape

- **Date filed:** 2026-02-03
- **Source:** Posted by DayZee in Discord (#scottish-open-source-institute)
- **Original filename:** `422873b2-e886-4dc1-8631-98bfa5752c37.txt`

> Note: Stored essentially verbatim (light front-matter only). Contains unverified claims/figures and informal citations; treat as a starting point for follow-up sourcing.

---

can you explain how and why there are no European Hyperscalers? What the existing companies are, and if their services are lesser for some reason? or just smaller?02:59[immediate] Good question - this cuts to a structural issue that will surface in any Scottish policy discussion. Let me search for current state of European cloud providers and the hyperscaler gap.Searched the web[immediate] Now I have enough to give you a comprehensive answer.

Why No European Hyperscalers?
The short answer: It's a compound failure across three reinforcing dimensions - capital structure, timing/scale dynamics, and market fragmentation. European providers exist and are technically competent, but they're structurally unable to compete at hyperscale.

Dimension 1: Capital Structure Failure
The European financial system is fundamentally misaligned with hyperscale infrastructure investment:
FactorUSEuropeFinancial systemCapital markets-basedBank-basedLate-stage VCDeep multi-billion fundsAbsent - "scale-up gap"Risk appetiteEquity/high-growth orientedRisk-averse, collateral-focusedExit marketDeep domestic IPO/M&AForeign buyers, "Delaware flip"
EU scale-ups raise only half as much capital as their Silicon Valley peers. More than four out of five scale-up deals in the EU involve a foreign lead or sole investor. Symtr The "Delaware flip" phenomenon - where successful European companies restructure as US subsidiaries to access capital - demonstrates the systemic nature of this failure.
Current hyperscaler capex puts this in stark relief: Goldman Sachs projects total hyperscaler capex from 2025-2027 will reach $1.15 trillion. Each of the four largest hyperscalers now exceeds $100B in annual infrastructure spending. Introl
No European company has access to capital at this scale. As U.S. cloud providers continue to invest some €10 billion every quarter in European capex programs, that presents an impossible hill to climb for any companies who wish to seriously challenge their market leadership. Fierce Network

Dimension 2: Timing and Scale Economics
Cloud is a winner-take-most market due to:

Network effects: More customers → more services → more customers
Learning effects: Operational excellence compounds with scale
Ecosystem lock-in: Free credits, proprietary APIs, partner networks
Capital efficiency: Unit costs decline with scale

AWS launched in 2006, Azure in 2010. By the time European sovereignty concerns became acute (post-2018 GDPR, post-2020 Schrems II), the hyperscalers had 15+ year head starts and orders-of-magnitude scale advantages.
Between 2017 and 2020, hyperscalers cut local cloud providers' market share nearly in half to 15%. Since then, their market share has stabilized. Fierce Network
The 15% floor represents the sovereignty/compliance-driven demand that actively seeks European providers - not competitive market capture.

Dimension 3: Market Fragmentation
The European providers are just fragmented and subscale. They even struggle with being European but are often only domestically focused. Fierce Network

OVHcloud is French-focused
Hetzner is German-focused
T-Systems serves German enterprise
No pan-European champion emerged

Despite regulatory leadership, Europe failed to cultivate its own cloud champions. Historical underinvestment, risk-averse capital markets and fragmentation among member states hindered large-scale tech projects. Akave
China provides the counter-example: In China the cloud ecosystem is dominated by local players. Tencent Cloud held ~15% of China's market. Holori But China achieved this through market exclusion, not market competition.

European Providers: What They Are
ProviderHQRevenueStrengthsLimitationsOVHcloudFrance€897M (2023)IaaS, bare metal, GDPR compliance, 3x cheaper storage than AWSLimited managed services, EU-focusedHetznerGermany~€500M est.Lowest cost/performance ratio in Europe, excellent bare metalMinimal PaaS, self-managed onlyScalewayFrance>€100MDeveloper-friendly, sustainability focus, KubernetesEU-only data centers, limited enterprise featuresOpen Telekom CloudGermanyN/AEnterprise-grade, ISG/Forrester "Leader" ratingsDeutsche Telekom subsidiary, German-focusedIONOSGermanyN/ASMB-focused, strong hosting heritageLimited advanced servicesSTACKITGermanyN/ASchwarz Group (Lidl) backed, enterprise focusNew entrant

Are Their Services "Lesser"?
For IaaS (compute/storage/networking): No - often better price/performance.
OVHcloud offers a diverse range of services, from bare metal servers to public cloud solutions, all with a focus on compliance with European data protection regulations. While OVHcloud's product offerings may not be as extensive as those of the hyperscalers, it effectively covers essential services like compute, storage, and networking at a significantly lower cost. For instance, their S3 equivalent storage product is three times cheaper than AWS. Holori
For PaaS/managed services: Yes - significantly narrower.
Microsoft Azure encompasses over 600 services. AWS offers over 200 services across compute, storage, databases, networking, analytics, machine learning and more. Intercept
European providers offer maybe 20-50 services. The gap isn't capability per service - it's breadth of managed services:

No equivalent to AWS Lambda/Azure Functions ecosystems at scale
Limited AI/ML managed services
Fewer database options
Less sophisticated IAM/security tooling
Weaker DevOps/CI-CD integration

Hetzner is unbeatable for performance-per-euro, and OVHcloud delivers full-stack capabilities at scale. Gart But with no native managed databases, Kubernetes, or PaaS options, Hetzner's budget-friendly compute requires more hands-on infrastructure management as you scale. DigitalOcean

The Practical Gap
CapabilityHyperscalersEuropean ProvidersIaaS (VMs, storage)✓✓ (often cheaper)Managed Kubernetes✓✓ (limited)Serverless functions✓ (deep)✓ (basic)Managed databases (10+ types)✓✗AI/ML platform services✓ (extensive)✗ (minimal)Global edge network✓✗200+ integrated services✓✗Enterprise support SLAs✓Variable

Implications for Scotland
This analysis reveals Scotland's strategic options:

Pure sovereignty (Schleswig-Holstein model): Accept narrower service breadth, use European IaaS + open source PaaS (Kubernetes, self-managed databases). Requires more in-house expertise.
Sovereign wrapper (France's S3NS/Bleu model): European-owned entities running hyperscaler technology under local legal jurisdiction. Preserves service breadth, creates legal/political sovereignty, but maintains technical dependency.
Hybrid segmentation: Hyperscalers for non-sensitive workloads, European/Scottish infrastructure for sensitive data. Requires clear data classification and architectural discipline.

The honest assessment: European providers can run government workloads competently, but switching from Azure/AWS means accepting either (a) reduced managed service convenience or (b) increased internal platform engineering capacity. Both are manageable with political commitment and appropriate investment.

Interesting pattern: China is the only major economy that achieved cloud sovereignty through market exclusion. Every other sovereignty initiative operates within the competitive reality of hyperscaler dominance. The European 15% market share floor appears stable - it represents the natural demand for sovereignty rather than competitive advantage.so does anyone offer anything close to the enterprise features of AWS?and ...03:05[immediate] Let me search for specifics on enterprise feature parity.Searched the web[immediate] Now I can give you a direct answer on enterprise feature parity.

Does Anyone Offer Enterprise Features Close to AWS?
Short answer: T-Systems/Open Telekom Cloud (now "T Cloud Public") is the closest, and they're explicitly targeting feature parity by end of 2026. But "close" still means meaningful gaps today.

The Current State
"The platform automates many background processes, already delivers 80 percent of the familiar core hyperscaler features and significantly reduces IT administration effort. By the end of 2026, we will reach full core feature parity," says Dr. Ferri Abolhassan. Deutsche Telekom
So the most enterprise-ready European provider currently claims 80% feature parity with hyperscalers, with full parity targeted for late 2026.
According to Information Services Group (ISG), the platform not only outperforms European alternatives, but is already more competitive than some offerings from Big Tech companies. WebWire

The Ranking (Enterprise Readiness)
Based on analyst reports and feature assessments:
ProviderEnterprise ReadinessKey StrengthKey GapT Cloud Public (Open Telekom Cloud)Highest in EUThe only European platform that fully meets all the technical requirements defined by the independent experts. Open Telekom Cloud BSI C5 certified, OpenStack-based, 4,000+ enterprise customersAI/ML depth, global reachOVHcloudStrongBroad IaaS/PaaS, Kubernetes, bare metal, SecNumCloud certifiedCons: Non-intuitive UI for newcomers, fewer integrations than AWS, limited managed databases LinktlySTACKITGrowingSchwarz Group backing (Lidl), enterprise focus, managed servicesSTACKIT may not offer the same breadth of specialized services (e.g., serverless functions, advanced AI/ML) as AWS, Azure, or GCP. XomniaScalewayDeveloper-focusedDeveloper UX, transparent pricing, sustainabilityScaleway uses US-based services for their Representation and Management of Core Service Xomnia - disqualifies from pure sovereigntyHetznerIaaS onlyBest price/performance in EUNo managed services, self-managed only

What "80% Feature Parity" Actually Means
The covered capabilities (most European enterprise providers now offer):

✓ Compute (VMs, containers, Kubernetes)
✓ Storage (object, block, file)
✓ Networking (VPCs, load balancers, firewalls)
✓ Managed databases (PostgreSQL, MySQL, Redis) - limited variety
✓ Identity/IAM
✓ Basic monitoring/logging
✓ Terraform/IaC support
✓ Container registries

The gap capabilities (where hyperscalers still dominate):

✗ AI/ML platform depth (SageMaker, Vertex AI equivalents are nascent)
✗ 200+ integrated services vs 30-50
✗ Serverless breadth (Lambda/Functions ecosystems)
✗ Global edge network (CloudFront, CDN at scale)
✗ Data analytics ecosystem (Redshift, BigQuery, Synapse equivalents)
✗ Enterprise integrations (Salesforce, SAP, Microsoft 365 native connectors)
✗ IoT platforms
✗ DevOps toolchain depth


The Performance Reality
Interestingly, where European providers do compete, they often outperform:
OVH PostgreSQL achieves more than 28,000 operations/s making it the clear winner for this workload. OVH PostgreSQL outperforms the second – Azure Database for PostgreSQL – by more than 9,000 operations per second, more than 30%. AWS RDS PostgreSQL (13,989 operations per second) and DigitalOcean PostgreSQL (12,562 operations per second) achieve less than 50% of OVH PostgreSQL's performance. Benchant
So for specific workloads (database performance, bare metal compute), European providers can actually beat hyperscalers. The gap is breadth, not depth in core services.
