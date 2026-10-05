# Collibra build guide

This is a tenant-neutral configuration sequence based on Collibra's published AI Governance and data governance documentation. Collibra documentation described an evolution from AI Governance to AI Command Center in 2026; product labels and screens can differ by release. Validate the current product name, edition, permissions, exact asset types, menus, feature entitlements and workflows in the target tenant. Product documentation cited here is versioned; a real build must use the documentation for the deployed release.

## Intended role in the design

Use Collibra as the governed business context for data: domain, glossary, catalogued assets, ownership/stewardship, relationships and lineage evidence. Where enabled and licensed, use Collibra AI Governance / AI Command Center assets and workflows to represent AI use cases, models and agents. In this dual-platform proposal, OneTrust remains the central AI review and risk-decision workflow record. Agree one authoritative home per attribute and link records; do not maintain conflicting duplicate approvals.

## Build sequence

### 1. Tenant and access readiness

- Confirm the deployed Collibra version, environment, product rights, latest UI requirement for AI Governance, enabled modules, available asset types and configured workflow engine with the Collibra administrator.
- Create named role groups for platform administration, domain governance, data steward, data owner, AI business user/model owner and read-only reviewers. Map to least privilege and separation of duties. Collibra's documented AI Governance setup references AI Business User and Data Scientist global roles; verify the current roles and permissions before assignment.
- Use non-production environment; verify SSO/MFA, audit logging, data residency, backup, retention and admin access under the organisation's controls.

### 2. Domain structure

Create or reuse a community such as **Resident Services**, then create a domain such as **Waste & Street Services** (final names approved by council). Keep domain ownership aligned to accountable service/data roles. Do not create an expansive taxonomy before the pilot slice is agreed.

### 3. Glossary

Load starter terms from `templates/glossary_seed.csv`. For each term define plain-language meaning, scope, exclusions, synonyms, domain, owner, steward, source of authority, classification/use note, status and review date. Proposed terms: Service Request, Service Category, Service Queue, Location Reference, Request Status, Resolution Timestamp, Human Review Outcome, AI Suggested Category. Business owners approve meanings; tool administrators do not adjudicate policy meaning.

### 4. Data asset catalogue

Use `templates/data_asset_register.csv` as intake. Add only approved technical/business metadata. Minimum fields: asset ID, display name, system, asset type, description, owner, steward, authoritative status, sensitivity/classification, permitted/prohibited purpose, source reference, refresh cadence, quality expectations, lineage parent/child, access route and review date. Use synthetic values in a portfolio demo. Never copy resident text or record-level samples into descriptions.

### 5. Data product and lineage

Select a vertical slice: **Service Request Intake** → approved staging/normalisation → proposed service-category suggestions → staff-reviewed destination queue → service reporting. Verify each hop with source owner, architecture diagrams, ETL/job metadata or system evidence. Record whether lineage is automated, manually asserted or incomplete and its evidence date. Where connector/harvesting support is not confirmed, record relationships manually and flag the limitation.

Set data-quality expectations with the domain owner: completeness of required routing fields; valid category values; consistency of status transitions; duplicate detection appropriate to the source; and freshness. Store measurement method, numerator, denominator, threshold owner, frequency, result and issue reference in `templates/data_quality_controls.csv`. Collibra metadata is a context/coordination layer; actual profiling and remediation may occur in source/engineering tools.

### 6. AI Governance assets (only if entitled and in scope)

The current Collibra documentation describes AI Governance records for AI Use Cases, AI Models and AI Agents and lifecycle/assessment features; exact asset model and labels vary by release. Register the bounded use case with owner and purpose. Link the relevant data assets, model/provider and agent only once selected and verified. Set status to proposed/review as supported by the tenant, and link to the authoritative OneTrust use-case ID, assessment and decision record.

If the organisation chooses to maintain only a cross-reference in Collibra, say so explicitly. Avoid starting parallel approval workflows that result in two apparent authoritative decisions.

### 7. Workflow and evidence

Configure any Collibra assessment, task, lifecycle or sign-off only after mapping required fields, owners, permissions, workflow triggers, evidence retention and failure handling. Test a positive, returned-for-information, rejected, material-change and retirement path in non-production. Confirm lifecycle status transition permissions. Capture screenshots or exported configuration evidence with secrets and personal data removed.

### 8. Release and stewardship

Obtain asset owner approval, test permissions with representative roles, review search visibility and metadata leakage, confirm import/export and rollback, train stewards, then publish approved metadata to intended users. Set quarterly or risk-based review date; remove or archive stale items according to policy.

## Minimum record quality gate

No priority asset is “approved/published” for this portfolio unless it has a confirmed owner, approved meaning, source reference, sensitivity/use note, lineage evidence or explicit gap, quality expectations, access route and review date. These fields are a proposed governance standard, not mandatory Collibra defaults.

## Tenant validation checklist

- Exact Collibra version/product label and licensed modules confirmed.
- AI Governance enabled and required UI / role permissions verified.
- Asset type, relation type and attribute names checked in current tenant.
- Source connectors, lineage support, scan scope and harvesting limits confirmed.
- Assessment/workflow availability, customisation limits and notifications tested.
- Search visibility, roles, audit trail, retention, APIs and exports checked.
- Platform record links to OneTrust resolve to the correct authoritative record.

