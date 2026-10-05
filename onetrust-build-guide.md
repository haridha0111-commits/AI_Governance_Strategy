# OneTrust build guide

This is a capability-led setup plan for **OneTrust AI Governance**. Product names, modules, packaging, assessment templates, field configuration, workflow routing, integrations and interfaces are subject to contract and tenant version. Confirm them with the OneTrust administrator/vendor before relying on them. Do not promise that the exact screen, template or connector exists in a particular subscription until verified.

## Intended role in the design

Use OneTrust as the central AI governance workflow record for use-case intake, AI inventory, ownership, lifecycle status, risk review, policy/control mapping, approval evidence and reassessment. OneTrust's published product material describes AI inventory/registry and risk/workflow capabilities. A product page is not proof of a specific council's entitlement, an independently validated control outcome, or compliance.

Collibra remains the business-facing governed data context and glossary/lineage record. Store stable Collibra asset IDs/URLs in OneTrust and the OneTrust AI record ID/URL in Collibra. Agree which system owns each field. Integration by API or connector is a discovery item; otherwise use controlled references and a reconciliation owner.

## Configure in sequence

### 1. Confirm product and environment

- Verify AI Governance product access, environment, tenant version, user roles, available templates and workflow rights with the administrator.
- Separate sandbox/test from production. Confirm SSO/MFA, roles, audit evidence, data residency, retention, backup, permitted integrations and supplier/subprocessor review.
- Use synthetic case content for initial setup. Do not place resident records, full prompts, credentials or confidential case evidence in the registry.

### 2. Define intake and required fields

Configure a short idea intake and fuller assessment record. Minimum proposed metadata: unique AI ID; name/description; intended purpose and excluded purposes; service and accountable owner; model/provider/version/status; deployment context; user groups and affected people; data assets and categories; data source IDs; output/action; human review; supplier; applicable location; lifecycle and review date; dependencies; known limitations; incidents; and links to evidence.

Use `templates/ai_use_case_register.csv` as the field specification. Unknown model/provider values stay “not selected” with an owner and due date; never invent values.

### 3. Set inventory lifecycle and coverage

Agree statuses such as Proposed, In review, Approved with conditions, Pilot, Production, Paused, Reassessment required, Rejected, Retired. Use only states the tenant can configure. Establish intake routes from project governance, procurement, privacy review, architecture, vendor renewal, model registry and periodic team attestation. Inventory AI embedded in SaaS as well as custom projects where in scope.

### 4. Configure risk triage and assessment

Start with the organisation's approved policy and questions. Example topics: service impact; affected people; purpose limitation; personal/special-category/criminal-offence data; data minimisation and provenance; rights/transparency; bias/fairness; reliability and robustness; explainability; human review; cybersecurity and prompt injection; third-party model and data terms; retention/logging; accessibility; incident handling; monitoring; change/retirement.

Route by context to privacy/DPO, security, service owner, data owner, procurement, legal, records and equality/accessibility review. Let the authorised specialist decide their own finding. Do not use a vendor risk score as a legal decision or automatic approval. A DPIA screening outcome and DPIA reference are recorded; DPO/privacy determines the organisation's process and whether a DPIA is required.

### 5. Approval workflow

Define gates: complete intake → initial screen → specialist assessments → evidence review → approval decision → conditions and expiry/review → pilot/production change control → periodic revalidation → retirement. Every decision captures who, when, scope, version, rationale, evidence, conditions, residual risk owner and triggers. Configure “return for evidence”, “reject”, “pause”, and “reassess” paths; verify that no incomplete or rejected case can be mistaken for approved.

### 6. Link Collibra and evidence

Create cross-references to Collibra data assets, glossary concepts, data products and lineage views. For an initial low-complexity portfolio demo, stable IDs and controlled URLs may be sufficient. If automating synchronisation, confirm supported API/connector, authentication, ownership, reconciliation, retry, deletion, audit and change-control behavior. Do not duplicate full lineage or sensitive metadata unnecessarily.

### 7. Monitoring, incidents and changes

Record each metric's definition, source system, owner, cadence, alert threshold, action and evidence link. Example signals: correction/override rate, misroute severity, recommendation omissions/additions, complaint/incident count, data quality, performance by relevant service context, model/provider version change, access anomalies, and failed human review. Agree thresholds before live use; values are not supplied by this template.

Change triggers include purpose, model/provider/version, prompt/context, retrieval source, data population, output/action, integration, user group, geography, supplier terms and observed impact. Material change moves the record to reassessment. Maintain incident, pause and retirement outcomes in the same record history.

### 8. Validate and release

In non-production test each lifecycle/workflow branch, role access, mandatory field, approval delegation, notification, evidence link, export, audit event and reassessment trigger. Validate that a rejected/paused item cannot pass as approved in dashboards. Obtain sign-off from business owner, governance process owner and system administrator before operational release.

## OneTrust record quality gate

A use-case record is review-ready only when intended and prohibited uses, owner, users/affected groups, data references, deployment context, provider/model status, human role, risk/impact screen, specialist review routing, test plan, monitoring plan, incident route, change triggers and decision authority are explicit. “Review-ready” is not “approved”.

## Tenant validation checklist

- SKU and module entitlement verified; official product name confirmed.
- Available AI inventory/registry objects and custom fields documented.
- Assessment framework templates reviewed for UK and local policy fit.
- Routing, approver delegation, rework, expiry and escalations tested.
- Evidence storage, access control, audit history and retention validated.
- Collibra reference method agreed; integration claims independently verified.
- Reporting calculations and dashboard definitions tested against sample records.

