# Architecture and controls

## Logical architecture

```text
Resident / staff request channels
              |
              v
Authoritative service / case system ---- approved identity, access and audit controls
              |                                    |
       approved minimum data                        | staff workflow
              v                                    v
Controlled AI service (proposed) ----------> Draft summary + category suggestion
              |                                    |
              +------------------------------> Trained staff review / correction
                                                   |
                                                   v
                                      Authorised service queue / reporting

Collibra: definitions, owners, data assets/products, quality context and lineage references
   <---- stable IDs / approved links; any automated sync is separately validated ---->
OneTrust: AI inventory, intake, risk reviews, approval record, conditions and monitoring evidence
```

The drawing is conceptual, not a deployment topology. It makes no claim about any specific council system, hosting provider, connector or integration.

## System-of-record boundaries

| Information | Proposed authoritative record | Other references |
|---|---|---|
| Business term, data owner/steward, data asset meaning, lineage context | Collibra | OneTrust stores stable data asset IDs/links needed for AI review |
| AI use-case inventory and risk-review workflow | OneTrust | Collibra AI Governance asset may reference OneTrust record ID if used |
| Source records and permissions | Source service/data platform | Collibra documents metadata and access route, not source authority or enforcement |
| DPIA / privacy approval evidence | Organisation's approved privacy record process/tool | OneTrust stores reference and workflow state if permitted |
| Security incident and service event | Approved incident/service-management system | OneTrust AI record links incident ID and status |
| Model artifact, endpoint, version and runtime controls | Approved model/platform registry and production platform | OneTrust / Collibra carry metadata and governance references |

The council must approve final system-of-record ownership. If an integration is not supported or permitted, use governed IDs/URLs, named update owners, and periodic reconciliation. Do not copy sensitive evidence just to make the record look complete.

## Control points

1. **Ingestion:** source owner approves data scope, legal/privacy basis, access, minimisation and retention before any AI processing.
2. **Catalog and metadata:** scan only approved sources; inspect extracted metadata exposure and search permissions; do not index resident text into Collibra.
3. **AI request:** approved endpoint, identity, network and secrets controls; block unapproved public tools for service data under organisation policy.
4. **Human review:** staff see original source, can amend/reject, and make the actual queue decision; capture outcome according to approved logs/retention.
5. **Access:** least privilege, service role segregation, no broad administrator or shared accounts, periodic access reviews.
6. **Logging and retention:** record what is necessary to investigate and demonstrate operation; avoid storing complete prompts/outputs unless justified and approved.
7. **Change:** model/provider/prompt/source/workflow changes enter change control and material changes trigger reassessment before deployment.
8. **Fallback:** manual routing remains usable; define continuity and rollback steps.
9. **Monitoring:** measure output quality, corrections, adverse outcomes, subgroup/service differences where appropriate, data quality, security and incidents.
10. **Retirement:** disable endpoint and credentials, withdraw staff access, handle retained data/logs under schedule, archive governance records, document lessons.

## Integration discovery questions

- Does the current Collibra and OneTrust subscription permit the needed APIs, integration tooling and workflow customisation?
- Which asset/assessment fields can be exchanged, by which supported mechanism, and under which identity/authentication method?
- How are stable IDs mapped? Who resolves duplicates, field conflicts and failed updates?
- Are source content and sensitive attributes excluded from sync by design?
- How are consent/notice, residency, supplier terms, audit, rate limits, retries, deletion and retention handled?
- How is the integration tested, monitored, versioned, supported and rolled back?

No integration has been built or verified in this portfolio pack. Do not represent a cross-reference diagram as a working connector.

