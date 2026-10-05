# A-to-Z delivery playbook

This sequence is the core practical guide. Adapt gates to the organisation's existing change, procurement, privacy and assurance process. The 16-week durations are a planning illustration, not a sourced benchmark. Do not progress a gate while a blocking decision is unresolved.

## Phase 0 — Mobilise and agree the mandate (Week 1)

**Do:** Confirm sponsor, service, intended outcome, boundaries, in-scope systems, decision authority, governance forum, team capacity, delivery method, and access to Collibra / OneTrust sandbox or demo environment. Confirm whether products are already licensed and who administers them.

**Create:** signed project brief; stakeholder map; delivery plan; assumptions, dependencies and decision log; data-handling plan; access request.

**Gate 0:** sponsor confirms scope and non-negotiable prohibitions; platform owners confirm a safe non-production environment or agree that the result is a design-only portfolio pack.

## Phase 1 — Discover current state and AI estate (Weeks 1–3)

**Do:** Run workshops with service staff, data owners, DPO/privacy, security, architecture, procurement, records management, legal, equality/accessibility and residents' representatives where suitable. Review existing policies, data inventories, procurement pipelines, vendor AI features, model registries, service maps and incidents. Ask for evidence; record gaps as gaps. Identify shadow/embedded AI via staff attestation and supplier reviews.

**Create:** current-state data flow; AI use-case inventory; system/vendor list; policy and control gap log; problem baseline plan; stakeholder-approved use-case statement.

**Tool work:** Start a Collibra domain/asset candidate list. Create the draft OneTrust AI use-case record early so intake is visible. Do not scan broad production sources or upload records before scan scope, permissions and metadata exposure are approved.

**Gate 1:** service owner validates the real service problem and intended purpose; governance lead confirms the bounded use case is within the stated guardrails.

## Phase 2 — Define target governance and risk routing (Weeks 3–4)

**Do:** Agree lifecycle states, tier triage, minimum evidence by tier, RACI, decision rights, exception/escalation route, prohibited uses, review cadence, retention and incident handling. Align with existing council policies and statutory roles; confirm local policy owners.

**Create:** target operating model; AI policy and intake requirements; risk/control matrix; approval workflow design; definitions and measures dictionary.

**Tool work:** map policy statements and assessment questions into OneTrust questionnaires/workflows where product entitlement supports them. Define Collibra role assignments, domain structure, asset types and metadata ownership. Keep policy interpretation under council authority.

**Gate 2:** sponsor approves operating model and delegated authority; DPO/privacy, security, records and procurement confirm their mandatory gates.

## Phase 3 — Establish data governance foundation (Weeks 4–7)

**Do:** Inventory only the minimum pilot-scope data assets. Confirm authoritative sources, owner/steward, business definitions, classification, purpose restrictions, data quality rules, lineage evidence, access route, retention and source permissions. Choose one or two priority data products for a demonstrable vertical slice.

**Create:** approved glossary seed; source inventory; data product definition; lineage map with evidence and confidence; quality-control register; data issue process.

**Tool work:** configure Collibra community/domain and asset model; populate glossary terms and assets; assign owners and stewards; capture relationships/lineage using supported metadata or approved references; record source/scan scope and classification approvals. If automated lineage harvesting is unavailable, document a manually evidenced lineage view and owner. Do not claim the catalog automatically enforces access or improves source quality.

**Gate 3:** data owners approve definitions and permitted use; privacy/security approve metadata and any scanning scope; quality and lineage gaps are documented with accountable remediation.

## Phase 4 — Configure AI inventory and assessments (Weeks 5–8)

**Do:** Register the proposed use case, provider/model if known, owner, business purpose, impacted groups, data references, system context, lifecycle status, human oversight, risk and change triggers. Run intake screening and route specialist reviews. Use a placeholder only where facts are genuinely not selected; do not invent a model or vendor.

**Create:** completed use-case record; AI/model inventory; risk assessment; DPIA screening outcome; equality/accessibility and security review outcomes or open action; supplier due diligence; test and monitoring plans; decision record.

**Tool work:** configure OneTrust AI use-case inventory, risk questionnaire, workflow/approvals and evidence references as available in the licensed tenant. Set required fields and conditional routing with platform administrators. Link corresponding Collibra data asset IDs and glossary terms in an agreed field/reference convention. Confirm OneTrust AI Governance module/package and assessment templates in the tenant before relying on them.

**Gate 4:** use-case record is complete enough for the panel to determine whether it proceeds to design, is returned for evidence, or is rejected. Intake is not approval.

## Phase 5 — Design the data and human workflow (Weeks 7–9)

**Do:** Map every data transfer, prompt/context input, output, log and staff action. Minimise content and identifiers. Define access, authentication, retention/deletion, supplier boundaries, service fallback and incident route. Design staff UI and review so reviewer sees the original source, can edit/reject, knows the model's limits and can complete the task without AI. Consider accessibility, language, digital inclusion and routes to challenge/correct service records.

**Create:** logical/physical architecture; data protection and security design; DPIA (if required after screening, or document reasoned screening decision); threat model; supplier/contract controls; human factors and equality/accessibility analysis; operational runbook.

**Gate 5:** accountable specialists approve design within their remit; unresolved lawful basis, special-category condition, retention, hosting, supplier, or security question blocks live personal data.

## Phase 6 — Build/configure and validate with synthetic data (Weeks 9–12)

**Do:** Build only in an approved non-production environment. Keep any prototype isolated from live systems. Use synthetic examples, including ambiguous, incomplete, multilingual, adversarial and edge cases. Set pass/fail thresholds with service owner and reviewers before tests. Assess category accuracy, summary fidelity, omission/addition, subgroup performance where justified and feasible, prompt injection, data leakage, security and reviewer workload. Record limitations and sample representativeness.

**Create:** test protocol; data provenance; reproducible test set description; results; defects and mitigations; model/provider/version and configuration record; residual risk; revised controls.

**Tool work:** update OneTrust evidence and assessment outcomes, not just a score. Update Collibra lineage and source references if design changes. Store restricted raw test material in the approved test environment, not catalog descriptions or this repo.

**Gate 6:** service owner and assurance reviewers determine whether results meet pre-agreed criteria. Any unacceptable performance, leakage, bias concern or ineffective human review returns to redesign or stop.

## Phase 7 — Pilot readiness and authorisation (Weeks 12–14)

**Do:** Table a concise evidence pack: intended use, excluded use, data map, DPIA decision, security/privacy/procurement/equality reviews, testing, human-oversight evidence, training, resident/staff transparency, service fallback, monitoring, incident response, stop trigger, expiry date and owner. Validate that permissions and logs work.

**Create:** decision paper with proceed / revise / stop recommendation; signed approval and conditions; pilot plan; user training; communications; operational support and incident contacts.

**Gate 7:** authorised sponsor explicitly decides on any controlled pilot. A readiness review or platform record alone is not authorisation. If evidence is incomplete, do not process live data.

## Phase 8 — Controlled operation, monitor, reassess, retire (Weeks 14–16 and ongoing)

**Do:** If separately approved, begin limited pilot with capped scope and named participants. Review service outcomes, error/correction/override rates, complaints, incidents, data quality, access, model changes and workflow effects at agreed intervals. Check drift or provider updates where observable. Reassess on material change. Pause use when a stop trigger fires; preserve evidence under approved retention rules; report and investigate incidents. At closure, decide scale, redesign, extend with approval, or retire and remove access/data as scheduled.

**Create:** monitoring dashboard/report; issue and incident trail; change/reassessment records; periodic attestations; pilot exit report; retirement/scale decision; lessons learned.

**Gate 8:** continued use requires review evidence and renewed accountable approval at the defined interval. A vendor update or changed prompt/context can be material; assessment is case-specific.

## Handover checklist

- Named business, data, privacy, security, model and platform owners; deputies and escalation contacts.
- Approved definitions, assets, relationships, access routes, quality controls and review dates in Collibra.
- Current AI inventory, decision history, conditions, assessment evidence and monitoring owner in OneTrust.
- Stable cross-platform reference IDs; documented link/update owner and reconciliation procedure.
- Approved process documents, role permissions, change control and audit/log retention.
- Open risks/actions with due dates and accountable owners; no hidden blockers.
- Training for reviewers and staff; accessible alternative/fallback service path.
- Pilot decision and its limits communicated; portfolio narrative accurately states what was designed vs executed.

