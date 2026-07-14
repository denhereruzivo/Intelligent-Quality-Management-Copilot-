# Data Sources, Rights, Limitations and Quality
### Denhe reRuzivo AI — Intelligent Quality Management Copilot

## Purpose

This document defines the data categories proposed for Denhe reRuzivo AI, the conditions for using them, and their limitations. The platform is a concept-stage QMIZ initiative. It must not ingest, index or reproduce content until the relevant rights, permissions and controls have been confirmed.

## Data sources and permitted use

| Source category | Example use | Rights and access requirement | Quality controls |
| :--- | :--- | :--- | :--- |
| Licensed standards | ISO 9001, ISO 14001, ISO 22000, ISO 45001, ISO 27001, ISO 31000, ISO 19011, ISO/IEC 17025 and ISO 15189 | Use only excerpts or full text covered by a valid licence or written permission from the rights holder. The system records source version and licence scope. | QMIZ subject-matter experts verify scope, edition and metadata before indexing. |
| Zimbabwean laws, regulations and public guidance | Publicly available regulatory or sector guidance | Confirm that the source is official, current and permitted for the intended reuse. Link to the authoritative source rather than treating summaries as law. | Maintain publisher, publication date, jurisdiction and review date; retire superseded material. |
| QMIZ-approved templates and training materials | Procedures, checklists, audit tools, glossary entries and examples | QMIZ owns the content or has documented permission to use it. | Expert review, version control and approval history. |
| Tenant-provided documents and evidence | Existing procedures, audit notes, risk registers, records and uploaded templates | The tenant confirms it owns or is authorised to process the material and obtains any required employee, customer or third-party permissions. | Tenant isolation, file-type checks, access controls, retention rules and human review of outputs. |
| Local-language glossary and translation reference material | Shona and Ndebele terminology and plain-language explanations | Use materials created by QMIZ, contributors under written agreement, or sources with suitable rights. | Bilingual subject-matter review verifies technical meaning before controlled publication. |
| De-identified pilot feedback and evaluation data | Usability, source coverage, review acceptance and error analysis | Collect only with a documented pilot agreement and informed participant notice. | Remove direct identifiers where possible; restrict access and set deletion dates. |

## Data that must not be used without additional approval

* Full copyrighted standards, paid training material, customer files or third-party reports without an explicit licence or permission.
* Sensitive personal data, health information, national identifiers, employee disciplinary records or trade secrets unless necessary, contractually authorised and protected by additional controls.
* Unverified internet content as an authoritative source for an ISO, legal or accreditation requirement.
* Personal data or confidential tenant content for model training unless the tenant has explicitly opted in through a separate written agreement.

## Limitations and quality risks

* Standards and regulation change. Retrieved sources can become outdated, incomplete or jurisdictionally inapplicable.
* RAG can retrieve an incomplete or poorly matched source, and an LLM can still produce inaccurate, overconfident or ambiguous text.
* Translation may preserve literal wording while losing technical meaning, especially where equivalent quality-management terminology is not established.
* Historical audit records can reflect inconsistent practice or bias; they are examples, not proof of a requirement.
* The platform cannot grant certification, accreditation, legal compliance or conformance. Those judgements remain with competent professionals and relevant authorities.

## Quality assurance and governance

1. Maintain a source register with owner, edition, jurisdiction, rights basis, ingestion date, review date and retirement status.
2. Enforce tenant, role and rights filters before retrieval.
3. Show source references, version information and uncertainty flags with generated outputs where possible.
4. Test priority workflows against expert-reviewed cases before each pilot release, including Shona and Ndebele evaluation.
5. Require a qualified person to review and approve all controlled documents, audit findings, risk registers and translations.
6. Provide a route for users to flag incorrect, unsafe, outdated or rights-restricted content; QMIZ investigates, corrects and records the outcome.
