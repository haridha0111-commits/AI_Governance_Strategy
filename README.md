# UK Local Authority AI Governance Strategy

**Interview portfolio project | Fictional composite council | Collibra + OneTrust | 2 September 2026**

This is an end-to-end, UK market-ready governance strategy and implementation workbook for a Data & AI Governance Lead / Manager interview. It gives a realistic public-service problem, target operating model, delivery roadmap, tool configuration plans for Collibra and OneTrust, assurance gates, measures, reusable registers, and an evidence-led source list.

> **Case integrity:** “Rivermere Council” and the service challenge are fictional, composite portfolio material. The scenario is not an actual council engagement and is not attributed to a named client, NHS body, supplier or consultancy. Public sources establish context and design requirements; they do not establish the fictional facts. Do not present this pack as a deployed tenant implementation.

## The project in one minute

Rivermere Council has fragmented service-request data, inconsistent definitions, unclear ownership, uneven quality and no dependable view of AI use across service teams. It is considering a narrowly bounded AI-assisted service-request routing pilot. The council needs to know what data and AI exist, who owns them, what use is approved, what risks and controls apply, and what evidence supports continued use.

The proposal establishes a federated Data & AI Governance operating model. **Collibra** is the enterprise business glossary, data catalogue, ownership and lineage context; **OneTrust AI Governance** is the AI use-case / model inventory, intake, risk and review workflow record. The operating model links records using stable IDs and approved references. Any native integration, API, connector, feature entitlement, or data synchronisation is a discovery item to validate with the actual vendors and tenant; this pack does not imply an out-of-the-box Collibra–OneTrust integration.

The pilot is a proposal only. Initial evaluation uses synthetic data. Production use requires sponsor approval, data-owner authority, privacy/DPO review including a documented DPIA screening decision, security and procurement review, equality/accessibility review where relevant, representative testing, a tested human override, and a recorded go-live decision. The system must not make eligibility, prioritisation of people, enforcement, or other final service decisions.

## Start here

1. Read [Project charter and case](project-charter.md) for the problem, boundaries, outcomes and assumptions.
2. Read [Strategy and operating model](strategy-operating-model.md) for governance principles, roles, decision rights, risk tiers and measures.
3. Follow [A-to-Z delivery playbook](delivery-playbook.md) in order. It is the main implementation guide.
4. Use [Collibra build guide](collibra-build-guide.md) and [OneTrust build guide](onetrust-build-guide.md) for platform-specific setup, with tenant/version validation gates.
5. Review [AI assurance and UK context](ai-assurance-uk.md), [architecture and controls](architecture-and-controls.md), and [interview walkthrough](interview-walkthrough.md).
6. Populate `templates/` using synthetic or approved metadata only. Keep personal data, case records, credentials, prompts, and confidential client information out of this repository and out of unapproved catalog metadata.
7. Label every interview artefact honestly as **proposed**, **illustrative**, or **implemented and evidenced**.

## Deliverables

| Artefact | Use |
|---|---|
| [Project charter and case](project-charter.md) | Sponsor-ready brief, problem statement, scope, outcomes and explicit assumptions |
| [Strategy and operating model](strategy-operating-model.md) | Principles, governance forums, roles, RACI, risk tiers, lifecycle and KPIs |
| [A-to-Z delivery playbook](delivery-playbook.md) | Discovery-to-handover plan, stage gates, work products and acceptance criteria |
| [Collibra build guide](collibra-build-guide.md) | Data-domain, glossary, asset, ownership, lineage and AI asset configuration sequence |
| [OneTrust build guide](onetrust-build-guide.md) | AI intake, inventory, assessments, review workflow, evidence and monitoring setup |
| [AI assurance and UK context](ai-assurance-uk.md) | Risk assessment, DPIA screening, human oversight, testing, monitoring, incidents and legal-source boundaries |
| [Architecture and controls](architecture-and-controls.md) | Logical flow, system boundaries, integration questions and security guardrails |
| [Interview walkthrough](interview-walkthrough.md) | A 10-minute demo narrative, likely questions and honest claims |
| [Source register](sources.md) | Primary UK government/regulator and vendor documentation with evidence limits |
| [`templates/`](templates/) | Starter registers for AI, data assets, controls, decisions, risks and metrics |

## Important platform and legal boundaries

- Collibra and OneTrust capabilities, product names, workflows, integrations, licensing, permissions and user interface change. Verify current documentation and tenant entitlement before configuration. The product guides are build specifications, not proof that a feature is licensed or activated.
- A catalogue does not itself fix data quality, grant access, determine lawful basis, approve an AI use, enforce runtime safeguards, or replace source-system security.
- OneTrust records and coordinates governance evidence; operational controls may live in identity, cloud, application, model-serving, service-management and security tools.
- UK legal applicability depends on actual facts, data, actors, purpose, sector and territory. This pack identifies review questions, not legal conclusions or a compliance certification.
- The UK AI principles are a regulator-facing policy framework and do not replace applicable law or sector guidance. The EU AI Act is not assigned as applicable to this UK-only hypothetical; assess territorial scope if facts require it.
- No Collibra, OneTrust, council, NHS, HMRC, TCS, Accenture or other client tenant was accessed. No implementation, certification, procurement decision or real-world performance result is claimed.

## Portfolio use

Adapt the materials to your own experience and label the fictional case. In an interview, explain the evidence behind each design choice, call out what requires legal/privacy/security sign-off, and distinguish a proposed target state from a working configuration. This project is designed to demonstrate strategy, governance delivery, stakeholder leadership and practical tool fluency without claiming vendor certification.

