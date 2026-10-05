# Strategy and operating model

## Strategy statement

Make data and AI use visible, understandable, accountable and reviewable across the council. Apply proportionate controls from idea through retirement, using Collibra for governed data context and OneTrust for AI intake, inventory, risk and assurance workflow. Keep accountable decisions with authorised people; use evidence from delivery and operations to refresh governance.

## Design principles

1. **Public purpose first:** state the service purpose and resident impact before selecting technology.
2. **Know the estate:** inventory declared AI, embedded vendor features and experiments through procurement, architecture review and periodic owner attestation.
3. **Data before model:** establish authority, meaning, quality, permitted use, sensitivity, lineage and access before connecting data to AI.
4. **Accountability stays named:** every data product, use case, model/provider and control has an accountable owner and an operational contact.
5. **Proportionate and contestable:** scale evidence and review to plausible impact; affected people and staff need appropriate routes to question or correct outcomes.
6. **Human control is real:** reviewers have context, time, training, authority, access to the source record and a usable override; a click-through is not meaningful oversight.
7. **Evidence over attestation alone:** link approvals to test results, control operation, incidents, changes and review dates.
8. **Least data and least privilege:** expose the minimum necessary metadata and content; keep sensitive values out of catalogs and governance registers.
9. **Change triggers review:** a change in purpose, data, provider/model/version, prompt, retrieval, workflow, users, geography or impact can invalidate prior approval.
10. **Stop when controls fail:** define a person empowered to pause use and a route to resume only after reassessment.

## Federated governance

The central Data & AI Governance function sets the policy, process, common metadata, templates and assurance reporting. Service domains own the meaning, quality, purpose and operational use of their data and AI. Privacy, security, legal, equality/accessibility, records, procurement and architecture teams provide specialist review within their remits. Platform teams administer Collibra and OneTrust with least-privilege roles and change control. Executive sponsors accept residual service risk only within delegated authority; legal compliance is not waivable by a governance forum.

### Forums and cadence (proposed)

| Forum | Proposed cadence | Decisions / outputs |
|---|---|---|
| Data & AI Governance Council | Monthly, with urgent escalation | Policy, risk appetite proposals, cross-domain conflicts, exceptions within delegated authority, portfolio status |
| Use-case Review Panel | At intake and each stage gate; ad hoc for high impact | Proceed / revise / reject recommendation; conditions; reassessment and stop decisions |
| Data Domain Working Group | Fortnightly during setup, then monthly | Definitions, asset owners, data quality issues, lineage and access referrals |
| Operational service review | Monthly in pilot; incident-driven as needed | Quality, safety, complaints, override rates, access and control issues, actions and pause recommendation |

Cadences are design choices to confirm with the sponsor. The council's existing governance may absorb these responsibilities rather than create new committees.

## Decision rights and RACI

R = responsible, A = accountable, C = consulted, I = informed. One accountable role per row; validate actual delegations.

| Activity | Sponsor | Service owner | Data owner/steward | DPO/privacy | Security | AI/model owner | Governance lead | Procurement/legal/equality |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Strategy, policy and delegated risk limits | A | C | C | C | C | C | R | C |
| Data meaning, authority and quality rules | I | C | A/R | C | C | C | C | I |
| AI intake and complete inventory record | I | A | C | C | C | R | R | C |
| Privacy review and DPIA screening decision | I | C | C | A/R | C | C | C | C |
| Security and architecture review | I | C | C | C | A | R | C | C |
| Supplier due diligence and contract | I | A | I | C | C | C | C | R |
| Evaluation and ongoing model performance | I | A | C | C | C | R | C | C |
| Pilot go/no-go within delegated authority | A | R | C | C | C | C | C | C |
| Pause during incident or control failure | I | A/R | C | C | R | R | C | I |
| Annual policy and control review | A | C | C | C | C | C | R | C |

## Risk tiers (proposed triage, not a legal classification)

| Tier | Example signals | Minimum governance response |
|---|---|---|
| Tier 1: Administrative / low impact | Internal drafting or categorisation; no consequential decision; limited approved data; easy reversal | Inventory; purpose and data owner; privacy/security screen; synthetic/representative tests; human review; named operational owner |
| Tier 2: Material service influence | Recommendations materially shape service queues, staff actions, or residents' access/timing; sensitive data or vulnerable groups may be involved | Tier 1 plus full multidisciplinary review, documented impact/risk assessment, DPIA decision, equality/accessibility analysis as appropriate, stronger validation and monitoring, explicit senior approval |
| Tier 3: High impact / prohibited pending escalation | Eligibility, rights, enforcement, significant decisions, profiling, vulnerable-person risk, uncontrolled autonomous action, or unclear lawful basis | Stop normal pathway; specialist legal/privacy/ethics/security review; consider redesign or reject. No approval by this portfolio design. |

Tier is a local governance triage aid only. It does not determine statutory status, DPIA requirement, UK or EU legal classification, or an organisation's risk acceptance. Risk tiering must be validated and should not be used to downgrade obligations.

## Lifecycle and stage gates

Idea/intake → triage → discovery and data assessment → design and procurement → build/configure → validation → pilot readiness → controlled pilot (separate approval) → operational monitoring → material change/reassessment → retirement. Each gate leaves a decision, owner, date, evidence links, conditions, expiry/review trigger and dissent/escalation record. Rejected or paused items remain in the inventory with reason and retention handling.

## Policy set to approve locally

AI acceptable-use policy; data governance policy; classification and handling standard; AI intake and impact-assessment procedure; privacy/DPIA procedure; human-oversight standard; model/data testing standard; third-party AI procurement clauses; access and logging standard; incident and breach procedure; retention and disposal schedule; change/reassessment process; public transparency and complaints route. Use current council policy and counsel review; this list is a target framework, not proof of legal requirements in every case.

## Measures and definitions

Set baselines during discovery, targets with the sponsor, and definitions before reporting. Never invent a benefit estimate or declare compliance from a dashboard.

| Measure | Definition | Owner / cadence |
|---|---|---|
| AI inventory completeness | In-scope AI records with required fields, accountable owner, lifecycle status and review date / all in-scope discovered AI records | Governance lead, monthly |
| Data asset accountability | Priority assets with confirmed owner and steward / priority assets in agreed scope | Domain owner, monthly |
| Review lead time | Calendar days from complete intake to recorded decision, with incomplete submissions reported separately | Secretariat, monthly |
| Gate evidence completeness | Approved use cases with all required evidence links for their tier / approved use cases sampled | Assurance lead, each gate / quarterly |
| Data quality control pass rate | Passing valid test observations / all observations, by rule and period; exceptions shown separately | Data owner, agreed run cycle |
| Human override / correction rate | Recommendations materially edited, rejected, or re-routed / reviewed recommendations, with contextual analysis | Service owner, monthly during pilot |
| Harm and complaint signals | Confirmed incidents, near misses and complaints linked to the use case; severity and time to contain | Service owner, immediate / monthly |
| Change-review timeliness | Material changes reassessed before release / material changes sampled | Model owner, each release / quarterly |

