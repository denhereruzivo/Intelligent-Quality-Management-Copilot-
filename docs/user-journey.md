# Denhe reRuzivo AI: User Journey Map
### Intelligent Quality Management Copilot

These journeys reflect the organisations QMIZ intends to support: SMEs, manufacturers, public institutions, laboratories, inspection and certification bodies, consultants and auditors. Generated output always requires qualified human review.

---

## 👥 User Personas

### 1. Tariro, SME Quality Manager
* **Role**: Quality manager at a Zimbabwean food-processing SME preparing for ISO 9001 and ISO 22000 certification.
* **Goals**: Create consistent policies, procedures, risk registers and staff-friendly training material without unaffordable consulting cycles.
* **Pain Points**: Limited access to ISO expertise, lengthy document development, and staff who need explanations in clear language.
* **System Need**: Grounded, editable templates and multilingual explanations that reduce effort without claiming to guarantee certification.

### 2. Ruvimbo, Internal Lead Auditor
* **Role**: Internal auditor working across a manufacturer or public institution.
* **Goals**: Build an audit programme, record evidence, write clear nonconformities and follow corrective actions through to effectiveness review.
* **Pain Points**: Audit documentation is inconsistent and teams often address symptoms rather than root causes.
* **System Need**: A workflow that structures evidence, cites the relevant authorised reference and supports robust corrective-action planning.

### 3. Nyasha, Laboratory Quality Officer
* **Role**: Quality officer at a testing laboratory preparing for ISO/IEC 17025 accreditation.
* **Goals**: Assess readiness, maintain controlled documentation and make procedures understandable to technical staff.
* **Pain Points**: Accreditation preparation requires specialised documentation and a clear link between evidence, competence and requirements.
* **System Need**: A guided gap-assessment and document workflow that preserves expert control and supports plain-language or local-language training material.

---

## 🗺️ Core User Journeys

### Journey 1: Creating a food-safety procedure and staff guide (Tariro)

```
[Define task] ──> [Select standard & language] ──> [Retrieve sources] ──> [Review] ──> [Approve & publish]
```

1. **Initiation**: Tariro needs a cleaning-and-sanitation procedure and employee guide for a food-processing line.
2. **Form Interaction**: She selects the document workflow, identifies ISO 22000 and the organisation's approved template, and requests a plain-English draft with a Shona explanation for employee training.
3. **Drafting Parameters**:
   * She enters the scope, process owners, hazards, controls and existing evidence.
   * She identifies the required source material and uploads only documents she is permitted to use.
   * She requests a risk-and-opportunity register for the process.
4. **Workflow Action**: The system retrieves authorised ISO guidance, approved templates and relevant organisational material, then produces labelled document and risk-register drafts.
5. **Review**: Tariro and the food-safety team verify the technical content. A competent bilingual reviewer checks the Shona guide before the Quality Manager approves it.

---

### Journey 2: Recording an audit finding and corrective action (Ruvimbo)

```
[Log Finding] ──> [Structured Audit Report] ──> [Request RCA] ──> [Corrective Action Suggestions] ──> [Log to CAPA DB]
```

1. **On-site logging**: Ruvimbo finds that required calibration records were not completed for three days.
2. **Input**: She records objective evidence, the affected process and the applicable authorised requirement using an offline-capable tablet form.
3. **Structured build**: The audit workflow proposes a nonconformity record, separating the evidence, requirement and finding. Ruvimbo checks the cited source and corrects the draft.
4. **RCA Assistance**: The system automatically prompts: *"Would you like to initiate a Root Cause Analysis?"*
5. **RCA generation**: The root-cause workflow guides a 5 Whys analysis. It offers hypotheses and a corrective-action plan for team validation:
   * *Correction*: Immediate calibration check.
   * *Corrective Action*: Implement a digital reminder system and retrain warehouse supervisors.
6. **Resolution**: The process owner accepts the plan, assigns actions and records effectiveness evidence in the corrective-action register.

---

### Journey 3: Preparing a laboratory for accreditation (Nyasha)

```
[Select scope] ──> [Gap assessment] ──> [Evidence & document plan] ──> [Expert review] ──> [Readiness dashboard]
```

1. **Scope**: Nyasha selects the laboratory's intended ISO/IEC 17025 scope and registers the available procedures, records and competence evidence.
2. **Assessment**: The system produces a traceable gap-assessment checklist and identifies missing evidence; it does not determine accreditation status.
3. **Improvement plan**: Nyasha assigns document, risk and corrective-action tasks to accountable owners.
4. **Review**: Laboratory leadership and a competent assessor review readiness evidence before engaging the accreditation body.
