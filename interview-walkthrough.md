# Interview walkthrough

## 10-minute portfolio narrative

**0:00–1:00 — Why this project**  
“I created a fictional composite local-authority case to show how I would establish practical data and AI governance before a service team pilots AI. The problem is fragmented service data and no joined-up evidence from data ownership to AI approval and monitoring. I am clear that the case is invented and not a client engagement.”

**1:00–2:00 — Bound the use case**  
Show the charter. Explain that the candidate use is staff-assisted service-request summarisation and category suggestion. It cannot decide eligibility, urgency, enforcement or resident outcomes. Initial testing is synthetic; production remains gated.

**2:00–3:00 — Strategy and people**  
Show the federated model and RACI. Emphasise business ownership, DPO/privacy, security, procurement, equality/accessibility, data stewards and front-line staff. The governance lead enables the process but does not replace accountable owners or specialist decisions.

**3:00–5:00 — Collibra**  
Demonstrate the intended data domain, glossary and one vertical slice of assets, ownership, quality and lineage evidence. State which fields are illustrative and explain that source permissions and quality remediation remain in operational systems.

**5:00–7:00 — OneTrust**  
Walk through AI intake, inventory, intended/prohibited purpose, supplier/model status, assessment routing, evidence, approval conditions and reassessment triggers. Explain the stable-ID link to Collibra and that the cross-platform integration is a design question until tested.

**7:00–8:30 — Assurance gates**  
Show DPIA screening, security, procurement, equality/accessibility review, synthetic test plan, real human-review test, monitoring and stop triggers. The key leadership point is that an intake score or signed form is not proof of safe operation.

**8:30–10:00 — Measures and leadership**  
Show how to report inventory completeness, accountable data assets, review lead time, control evidence, correction/override, incidents and change-review timeliness. Explain how you would baseline, set targets with sponsors, escalate issues and decide stop/revise/proceed.

## Demo setup

Use a licensed sandbox, vendor demo or screenshots you are authorised to show. Populate only synthetic data. If no tenant is available, walk through the workbook as a target configuration design and state that no tenant configuration has been implemented. Do not imply certification or product expertise you have not earned.

## Likely interview questions

**Why both Collibra and OneTrust?**  
The design assigns distinct responsibilities: Collibra maintains business meaning, data ownership, catalogue and lineage context; OneTrust coordinates AI inventory and risk workflow. Two platforms create duplication risk, so the target has a defined system of record per field, stable IDs and an explicit integration/reconciliation decision. If an organisation already has a capable platform, I would assess fit before adding another.

**How did you avoid over-governance?**  
Short intake, reusable metadata, risk-proportionate evidence and specialist reviews routed by context. Low-impact administrative use can have a lighter path, while consequential decisions or unclear legal basis stop for escalation. Legal duties are never relaxed by a local tier.

**How do you prove human oversight is meaningful?**  
Observe the actual workflow, test whether a reviewer has source context, authority, time and training, measure edits/rejections, and verify staff can do the task without AI. Do not equate a human click with oversight.

**How do you handle poor data?**  
Assign an owner, document definitions and quality expectations, measure against agreed rules, trace the issue and remediation to the source/engineering team, and constrain or stop use if data is unfit. A catalogue records context; it does not correct the records.

**What if the model changes?**  
Treat a provider/version, prompt, source, purpose, population or action change as a reassessment trigger. Determine materiality with the model owner and assurance roles before release; record version and decision.

**What would you do first on a real client?**  
Confirm mandate and existing control environment, listen to service users and staff, inventory actual data/AI/procurement, validate system-of-record boundaries and legal/privacy/security requirements, then choose a small vertical slice with clear owners and evidence.

## Honest claims checklist

- Say **“fictional composite scenario”**, not “client project”.
- Say **“proposed configuration / build guide”** unless you have tenant evidence.
- Say **“synthetic example”** for template records.
- Say **“not yet verified”** for product integrations, entitlements, menus or current contract features.
- Describe the UK principles as an assurance lens and cite current official guidance.
- Do not state that OneTrust or Collibra alone ensures compliance, fairness, privacy or safe operation.

