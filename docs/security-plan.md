# Security, Privacy & Responsible AI Safeguards
### Denhe reRuzivo AI — Intelligent Quality Management Copilot

This document outlines the security controls, data protection policies, and responsible AI safeguards engineered into the QMS system.

---

## 🔒 Security & Data Protection Controls

Quality Management Systems contain sensitive organizational procedures, operational audit reports, and employee details. The system adopts a **Medium-to-High Risk** security control posture:

### 1. Identity & Access Control (RBAC)
We enforce a strict Role-Based Access Control (RBAC) matrix:
* **Platform Administrator**: Configures the service and operational controls. Access to tenant content is time-bound, logged and only granted when required for support.
* **Tenant Administrator**: Manages organisational users, roles and retention settings; does not automatically receive all restricted content.
* **Quality Manager / Approver**: Drafts, edits and approves controlled QMS documents, risk registers and translations within the assigned organisation.
* **Auditor / Laboratory User**: Records evidence, prepares audit or readiness artefacts, and initiates RCA or corrective-action workflows; cannot change approved documents without authority.
* **Employee / Viewer**: Accesses approved content only, including approved Shona or Ndebele guidance where provided.

### 2. Encryption Standards
* **In-Transit**: All communication between the Web UI, API backend, and database is encrypted using TLS 1.3.
* **At-Rest**: Postgres database storage and uploaded files (PDFs, templates) are encrypted using AES-256.
* **Vector Database**: Vector data is tenant-isolated, accessed over secure connections and uses server-side secrets. Source documents and embeddings are deleted or retained according to the tenant agreement.

### 3. Secrets Management
* No credentials, passwords, or LLM API keys are committed to the code repository.
* Keys are injected by a managed secrets service or protected host environment; `.env` files, if used in development, are excluded from version control.

---

## 🛡️ Responsible AI & Guardrails

### 1. Human-in-the-Loop Gate
Because QMS documents can affect safety, quality, food safety, laboratory competence and regulatory compliance, **unreviewed AI output must never be treated as an approved requirement or directly published**.
* **Draft flagging**: Every generated document, audit suggestion, risk entry, translation and RCA hypothesis is labelled as AI-assisted draft content and retains its source references.
* **Approval step**: An appropriately authorised and competent user reviews the output, verifies sources and technical meaning, makes necessary edits and approves it through a controlled workflow.
* **Translation review**: Shona and Ndebele translations are reviewed by a competent bilingual reviewer before being issued as controlled training or operational material.

### 2. Context Grounding (RAG Guardrails)
To prevent hallucinations where the LLM might fabricate a standard requirement:
* Retrieval is restricted to content the user and organisation are permitted to access. The system provides references or identifies the source category used.
* If suitable, authorised evidence is not found, the system must say so and direct the user to the official standard, regulator, competent auditor or subject-matter expert.
* The product must not claim certification, accreditation, legal compliance or conformance based solely on generated output.

### 3. Data Minimisation & Compliance
* The system minimises personal data and collects only what is necessary for access, accountability and tenant-approved workflows. Audit evidence may contain sensitive personal or operational information and is protected accordingly.
* Organisations can choose local, regional or approved on-premise deployment based on their privacy, contractual and data-residency requirements.
* Before ingesting standards, legislation, templates or organisational documents, QMIZ and the tenant must confirm ownership, licence, permission, retention period and permitted AI processing.
