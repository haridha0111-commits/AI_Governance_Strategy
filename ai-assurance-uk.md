# AI assurance and UK context

This is a governance checklist for the fictional case. It is not legal advice, a substitute for counsel or regulator guidance, or a claim that every item is legally required in every circumstance. The organisation must assess actual facts, current law, regulator remit, service and territory before approval.

## Assurance questions by lifecycle

| Area | Questions and evidence |
|---|---|
| Purpose and necessity | What service problem is being solved? Why AI? What non-AI alternative was considered? Is the proposed use limited to the stated task? |
| Data and provenance | Which source assets are used? Are they authoritative and suitable? What personal/special-category data may appear? Is the use compatible and minimised? Who approved access? |
| Privacy and rights | Who is controller/processor? What lawful basis and any additional condition apply? What transparency, rights, retention, data-subject request, and complaint routes are needed? Has the DPO/privacy team documented DPIA screening? |
| Fairness and equality | Could errors or routing patterns disadvantage people or groups? What data and test coverage support the evaluation? Is an equality impact analysis or engagement appropriate under local policy? What is not measurable? |
| Human oversight | Can staff see source text and uncertainty, correct or reject outputs, and complete work without AI? Are they trained, sufficiently resourced and authorised to challenge? Are decisions and corrections captured? |
| Accuracy and robustness | Does the system omit or add facts, misclassify, behave inconsistently, or fail on ambiguous, incomplete, multilingual or adversarial input? Are thresholds agreed before tests? |
| Security and resilience | Are threat model, access, secrets, prompt injection, data leakage, logging, supplier boundaries, service fallback, incident response and recovery addressed? |
| Transparency and contestability | Do staff and affected residents receive useful information about AI's role, limits and how to question/correct a service record or outcome? |
| Supplier and procurement | What model/provider/version and subprocessors are involved? Where is data processed? Can vendor terms permit retention or training? What change notice, audit, breach, deletion, exit and continuity terms apply? |
| Monitoring and change | Who watches performance, drift, incidents, complaints, override/correction and group/service context? Which changes trigger reassessment? Who may pause and resume? |
| Records and audit | Can the organisation reproduce the decision, data/model version, approval conditions, control evidence, action, incident and review history under an approved retention schedule? |

## DPIA and privacy decision path

1. Map processing, data subjects, purposes, sources, recipients, providers, retention and outputs.
2. Apply current ICO guidance and the organisation's privacy process to determine whether processing is likely to result in high risk and whether a DPIA is required. Do not infer “no DPIA” from a low portfolio tier or a vendor assessment score.
3. Record the DPO/privacy team's screening rationale and decision. If required, complete and consult on the DPIA before processing begins; resolve high residual risk through the organisation's lawful escalation route.
4. Revisit the assessment after material changes or new evidence.

ICO guidance states that AI processing will in the vast majority of cases involve a type of processing likely to result in high risk, with case-by-case assessment. This is a strong reason to make documented screening a hard gate; it is not an automatic determination for this fictional use case. The ICO also identifies specific Article 35(3) circumstances. Apply the current text and guidance to actual processing.

## Human oversight test

Before a pilot, observe representative staff using the workflow. Confirm the reviewer can: inspect the source; understand the AI output and uncertainty; detect omissions or additions; override without penalty; choose an alternative queue; stop and escalate; and provide a service without AI. Review whether workload, interface design, automation bias or management incentives undermine those abilities. Record observed findings and actions.

## Example pre-agreed stop triggers

Values and owners must be set by the sponsor before live use. Pause the AI function and use approved manual process if any trigger occurs:

- Personal/sensitive data reaches an unapproved recipient or is retained contrary to approved terms.
- A material purpose, model/provider/version, data source, prompt/context, output or user population changes without review.
- Harmful or systematically unequal error pattern, material misroute, or threshold breach is detected.
- Human review is bypassed, not meaningfully possible, or staff cannot complete the task safely.
- A serious incident, security event, complaint pattern, or unresolved legal/privacy concern is identified.
- Monitoring, audit logging, source lineage or incident response becomes unavailable.

The service owner and security incident process determine immediate containment; DPO/privacy, legal, communications and other roles are engaged under local procedures. Record root cause, affected scope, remediation, and authorised restart decision.

## UK context: sources and limits

- DSIT's published guidance explains five cross-cutting principles for regulators: safety/security/robustness; appropriate transparency/explainability; fairness; accountability/governance; contestability/redress. The cited guidance says the principles are voluntary guidance for regulators and do not displace existing law. Use them as an assurance lens, not a standalone compliance checklist.
- ICO AI and data protection guidance is relevant to public, private and third-sector organisations. Apply it alongside current UK GDPR, Data Protection Act 2018 as amended/commenced, other applicable law and local policies.
- The Data (Use and Access) Act 2025 is being commenced in stages. The GOV.UK commencement page and current ICO guidance should be rechecked at delivery; this pack does not state a complete commencement or legal position.
- Public-sector equality, accessibility, procurement, records and service obligations require specialist review against the actual authority, service and facts. No conclusion is made here that a particular assessment or statutory duty is triggered.
- The EU AI Act is not treated as applicable to this fictional domestic council case. If a provider, affected persons, establishment or deployment creates a territorial nexus, counsel must assess scope.

