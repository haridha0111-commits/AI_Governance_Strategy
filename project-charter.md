# Project charter and case

## Executive brief

**Client persona:** Rivermere Council, a fictional composite English local authority.  
**Programme:** Establish a practical data and AI governance capability using Collibra and OneTrust.  
**Sponsor:** Director of Digital and Customer Services (proposed role; fictional).  
**Delivery lead:** Data & AI Governance Lead / Manager.  
**Duration:** 16-week initial discovery, design and pilot-readiness programme, followed by a 90-day controlled pilot only if every gate passes. This is a planning estimate for the case, not a vendor or sector benchmark.  
**Status:** Proposed portfolio design; not an actual client engagement or deployed implementation.

## Problem statement

Rivermere Council’s service teams receive missed-bin, street-scene, housing-repair and general customer requests through several channels. The supporting records and reference data are spread across service systems and shared reporting areas. Teams use overlapping labels for request type, urgency, location and completion; accountable owners and authoritative sources are not consistently recorded; and data-quality problems can surface late in reporting or service handoffs. The council has no single governed view that connects the data behind a proposed AI use with its purpose, model/provider, service owner, privacy and security reviews, approvals, human checks, monitoring evidence and change history.

The council is considering an AI assistant that could summarise an incoming service request and suggest a service category and queue for a trained member of staff to review. Without a governance strategy, staff may use inconsistent data, the system may expose unnecessary personal information, suggestions may be wrong or biased, and a draft recommendation may be treated as an authorised service decision. The council needs an accountable, risk-proportionate way to discover and govern data and AI throughout the lifecycle before deciding whether the pilot should proceed.

**Evidence boundary:** This is an invented, plausible composite scenario. No public source used in this pack establishes that any named council has these exact issues or plans. It is not a quotation or case study from a local authority, NHS organisation, consultancy or vendor.

## Proposed use case

**Working title:** Staff-assisted service-request classification and summarisation.  
**Purpose:** In a future, approved pilot, produce a short draft summary and candidate service category from an incoming request for staff review.  
**Decision authority:** A trained council employee checks the original request, edits or rejects the suggestion, selects the destination queue and remains accountable for the action.  
**Initial test data:** Synthetic examples only.  
**Production data:** Not authorised by this portfolio design; source, lawful processing, minimisation, retention, security, transparency and access decisions remain open until approved.

**Out of scope / prohibited for this case:** Automated eligibility or entitlement decisions; deciding whose request receives priority; enforcement; vulnerability scoring; profiling residents; sentiment or emotion inference; using protected characteristics to route or rank; automatic resident-facing replies; training a model on council requests without separate approval; or processing special-category data unless a separately justified, assessed and approved design explicitly permits it. These boundaries are proposed governance controls, not legal advice.

## Objectives and outcomes

| Objective | Evidence of outcome |
|---|---|
| Establish accountability for priority data and AI assets | Named owners and stewards, agreed decision rights and review dates in Collibra / OneTrust |
| Improve discoverability and shared meaning | Approved domain glossary and catalogued pilot data products with definitions, purpose, sensitivity and lineage references |
| Put AI use through consistent review | OneTrust intake and risk workflow with accountable reviewers, decisions, conditions and evidence |
| Prevent uncontrolled progression | No build, live data, production release or material change proceeds without its defined approval gate |
| Make monitoring actionable | Named measures, thresholds to agree, alert routes, incident owner and pause/withdraw authority |
| Create interview-ready delivery evidence | Redacted or synthetic artefacts, decision trail, demo narrative, clear proposed/implemented labels |

## Scope

**Included:** stakeholder discovery; current-state inventory; data and AI governance policies; target operating model; priority glossary; data asset register and lineage; OneTrust AI inventory/intake and risk review; Collibra metadata configuration plan; tool role design; DPIA screening and privacy-by-design workflow; supplier, security, equality/accessibility and records-management review points; synthetic evaluation plan; control evidence; pilot-readiness decision; measures and handover.

**Excluded:** procuring or configuring production software; real resident data; model development; legal advice; completed DPIA; formal equality impact assessment; security accreditation; council-wide data remediation; production go-live; assurance certification; claims that vendor workflows or integrations have been tested.

## Stakeholders to engage

Service owner and frontline staff; Director-level sponsor; data owners and stewards; Data Protection Officer / privacy team; information security; enterprise/data architect; procurement and supplier assurance; records-management / information governance; equality, accessibility and public involvement leads; legal counsel; service-design team; model/product owner; platform administrators; internal audit or assurance. Confirm local titles and statutory roles with the actual organisation.

## Assumptions and open questions

The case assumes a council has an intake channel, a service-management or case system, a reporting layer, and a potential AI-assisted routing proposal. Those are scenario assumptions to validate during discovery, not statements about a real council. Before design approval, establish: exact service and geography; controller/processor roles; data categories and volumes; lawful purpose and basis; accessibility needs; source-system authority; retention schedule; hosting and data residency; vendor/subprocessor terms; model/provider/version; integration architecture; staff workflow; affected residents; supplier exit; and applicable local policies.

## Acceptance criteria for the 16-week readiness phase

1. Sponsor signs the scope, objectives, non-negotiable prohibitions and governance decision rights.
2. Priority data and AI records have owners, stewards, status and review dates; unknowns are explicit.
3. Collibra terms and data assets have owner-approved definitions, classification/use metadata and traceable lineage references for the bounded pilot scope.
4. OneTrust record links use case, provider/model, data references, assessments, decisions, conditions and review triggers, using stable IDs and an agreed cross-reference method.
5. DPO/privacy, security, procurement, equality/accessibility, records and service leads have documented review outcomes or open actions.
6. Synthetic evaluation criteria and pause triggers are agreed before testing; test results are reproducible and reviewed by a human.
7. The sponsor makes an explicit proceed / revise / stop pilot-readiness decision. Readiness is not production approval.

