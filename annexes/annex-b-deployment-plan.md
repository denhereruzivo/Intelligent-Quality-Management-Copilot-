# Annex B: Deployment & Operational Plan
### Denhe reRuzivo AI — Intelligent Quality Management Copilot

This document contains the completed deployment and operations plan requested in Annex B of the AI4I Product Readiness guidelines.

---

| Field | Participant Response |
| :--- | :--- |
| **Deployment Environment** | **Hybrid / Institutional System**:<br>• The web frontend and database are hosted on a localized Zimbabwean cloud instance.<br>• Metadata databases can also run on local servers within target organizations to comply with data privacy policies regarding internal procedures. |
| **Hosting Provider or Site** | • **Zimbabwean cloud deployment**: evaluate TelOne Cloud, Liquid Intelligent Technologies or another suitable regional provider for low-latency access and data-residency needs.<br>• **Alternative/on-premise option**: deploy in a participating organisation's controlled environment where policy requires it. |
| **Operator** | • QMIZ is the product steward and leads quality content, pilot governance and user training.<br>• The technical operator manages the platform, monitoring, releases and incident response.<br>• Each tenant's administrator manages authorised users, local backups and their organisational documents. |
| **Pilot Site** | • A QMIZ-selected SME, public institution, manufacturer or laboratory representing a priority QMS or accreditation-readiness use case. Pilot selection will confirm consent, data rights, connectivity and a qualified reviewer. |
| **Users to Onboard** | • **Initial batch**: 15–20 users including quality managers, internal auditors, process owners, laboratory staff where applicable, and at least one authorised approver. |
| **Training & Support** | • **Onboarding**: a QMIZ-led workshop covering responsible use, source verification, document approval and local-language review.<br>• **In-app support**: guided workflows, an accessible technical guide and feedback capture.<br>• **Support**: defined email/WhatsApp Business support channel with escalation for data or safety incidents. |
| **Monitoring** | • **Application Health**: Uptime Kuma for checking system availability.<br>• **Usage Logs**: Audit trails recording user actions, document creation stats, and system latency metrics. |
| **Backup & Recovery** | • **PostgreSQL Database**: Automated daily incremental backups stored in an isolated, encrypted S3 bucket.<br>• **Recovery Point Objective (RPO)**: 24 hours.<br>• **Recovery Time Objective (RTO)**: Under 2 hours. |
| **Connectivity Plan** | • **Zimbabwe Context Optimization**:<br>1. **Offline Mode**: Local storage cache stores audit logging forms. Users can record audit findings on their tablets in connectivity-dead zones; data auto-syncs when reconnecting to Wi-Fi/4G.<br>2. **Payload Reduction**: Images uploaded during audits are compressed client-side before submission. |
| **Scale Pathway** | • **Phase 1**: QMIZ-led pilot for priority workflows such as QMS documents, audit support, risk registers and local-language explanation.<br>• **Phase 2**: add validated templates and workflows for ISO 9001, 14001, 22000, 45001, 27001, 31000, 19011, ISO/IEC 17025 and ISO 15189, subject to data rights and expert review.<br>• **Phase 3**: expand to multi-tenant deployments for partners across Zimbabwe's quality ecosystem. |
| **Milestones** | • **30-Day**: select pilot, establish governance and data-rights agreements, define evaluation metrics, and test retrieval on authorised source material.<br>• **60-Day**: launch a controlled prototype; validate document, audit, risk and translation workflows with qualified reviewers and pilot users.<br>• **90-Day**: measure usability and output quality, complete security testing, address findings, and decide whether to extend the pilot. |
