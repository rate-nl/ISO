# AI Management System (AIMS) 

**Standard:** ISO/IEC 42001:2023 (with EU AI Act readiness)
**Organization:** DineRate B.V. group (operating identity: Rate / Rate.nl)
**Document version:** 3.0
**Date of issue:** 6 July 2026
**AIMS Owner (accountable):** Inge Proost (CEO / Managing Director)
**AI Technical Lead (responsible):** Firas Kassoumeh
**Approved by:** Inge Proost (CEO) — recorded in the [AIMS Review & Approval Log](#aims-review--approval-log); signed evidence held in Manager Approvals (Google Drive).
**Supersedes:** AIMS.md v2.0 (30 June 2026); full history in Appendix C
**Integration:** Extends the certified ISO/IEC 27001:2022 / NEN 7510:2022 ISMS

> **Audit note:** This document is the complete, standalone AIMS. It contains all required policies, procedures, registers, impact assessments, model cards, evidence structures, and record templates. All controls are addressed. Items marked [RECORD] are operational records to be populated. The DPIA is a standalone document referenced in Section 9. The EU AI Act compliance mapping is in Section 15.

---

## Document Control

| Field | Value |
|---|---|
| Document | AI Management System Manual (AIMS_Complete_Implementation.md) |
| Version | 3.0 |
| Date of issue | 6 July 2026 |
| Owner | Inge Proost (AIMS Owner) |
| Author | Firas Kassoumeh (AI Technical Lead) |
| Approval | Approved by the CEO — recorded in the AIMS Review & Approval Log |
| Review cycle | Annual minimum; triggered by: significant AI system change, incident, new regulatory requirement, audit finding |
| Related documents | ISMS manual (readme.md); ISMS Logs (Logs.md); AI Evidence Log (AI_Evidence_Log.md); DPIA (standalone); Supplier DPAs (Google Drive) |
| Repository | rate-nl/ISO |
| Classification | Internal — Confidential |

### AIMS Review & Approval Log

Approval is recorded here (approver + date). **A single CEO sign-off covers this AIMS and all embedded records** (policies, procedures, AISIAs, model cards, SoA, risk register, risk acceptances). Signed evidence is held in the [Manager Approvals folder (Google Drive)](https://drive.google.com/drive/folders/16uO9oefcut5vRY9nUq_CJkapfcTSJ2Vb). No inline signature blocks are used in this document.

| Version | Date | Approved by | Change summary |
|---|---|---|---|
| 1.0 | 18 Jun 2026 | Inge Proost (CEO) | Initial AIMS issued |
| 2.0 | 30 Jun 2026 | Inge Proost (CEO) | Gap-analysis remediation: added standalone procedures, record templates, EU AI Act mapping, training framework, risk acceptance records, complete Annex A evidence |
| 3.0 | 6 Jul 2026 | Pending — Inge Proost (CEO) | Format & governance revision: removed inline signature blocks (single sign-off via this log + Manager Approvals); added the Governance Records section; reformatted to ISMS-style numbered sections with a linked Table of Contents and Introduction. No change to policy, risk, AISIA, DPIA or control content. |

---

## Table of Contents

- [1. Introduction](#1-introduction)
- [2. AIMS Governance Records](#2-aims-governance-records)
- [3. AI Management System (ISO/IEC 42001 Clauses 4–10)](#3-ai-management-system-isoiec-42001-clauses-410)
- [4. AI Risk Management (Register & Risk Acceptance)](#4-ai-risk-management-register--risk-acceptance)
- [5. Statement of Applicability (ISO/IEC 42001 Annex A)](#5-statement-of-applicability-isoiec-42001-annex-a)
- [6. AI System Impact Assessments (AISIA)](#6-ai-system-impact-assessments-aisia)
- [7. Registers (Resources, Data, Suppliers, Models)](#7-registers-resources-data-suppliers-models)
- [8. AI Lifecycle & Operational Controls](#8-ai-lifecycle--operational-controls-a6-a8-a9)
- [9. Data Protection Impact Assessment (DPIA)](#9-data-protection-impact-assessment-dpia)
- [10. Model Cards](#10-model-cards)
- [11. AI Policies](#11-ai-policies)
  - AI Policy (full text)
  - AI Use Policy (employees & contractors)
  - AI Incident Response Policy
  - AI Supplier Management Policy
  - AI Data Governance Policy
  - AI Training & Competence Policy
- [12. Procedures](#12-procedures)
  - AI Risk Assessment
  - AI System Impact Assessment
  - AI Incident Response
  - AI Change Management
  - AI Monitoring & Performance Review
  - AIMS Internal Audit
  - AIMS Management Review
- [13. Record Templates](#13-record-templates)
  - Competence & Training Records
  - Internal Audit Checklist
  - Management Review Record
  - Risk Acceptance Record
  - Nonconformity & Corrective Action Log
  - Model Validation Record
  - Consent & Transparency Log
  - Model Monitoring & Drift Log
  - Change Request Record
  - Supplier AI Risk Assessment Record
- [14. Integrated Evidence Log](#14-integrated-evidence-log)
- [15. EU AI Act Compliance Mapping](#15-eu-ai-act-compliance-mapping)

**Appendices**
- [Appendix A — Continual Improvement Plan](#appendix-a--continual-improvement-plan)
- [Appendix B — Cross-Reference: AIMS ↔ ISMS](#appendix-b--cross-reference-aims--isms)
- [Appendix C — Document History](#appendix-c--document-history)

---

# 1. Introduction

## Purpose and Objectives of the AIMS

Rate is committed to developing and operating artificial-intelligence systems responsibly, lawfully, safely and transparently. This AI Management System (AIMS) manages AI-specific risks across the full lifecycle of the organization's AI systems, in accordance with **ISO/IEC 42001:2023** and the **EU AI Act**, and extends the certified **ISO/IEC 27001:2022 / NEN 7510:2022** ISMS. Its objectives are to ensure human oversight, fairness, transparency, data protection, security and continual improvement of the AI systems in scope.

## Scope of the AIMS

The AIMS covers the development, provision and operation of AI systems for **voice-driven collection and structuring of care information** and for **voice-based emotion recognition** — **iVessy** and **Vess360** (and **Vera** upon operational launch) — within **DineRate B.V.**, operated by **CareRate B.V.** and **Vess B.V.** The CareRate / Rate.nl platform (no AI of its own) and the EAGLE project are excluded. The full scope statement is in **Section 3 (Clause 4.3)**.

## Relationship to the ISMS

The AIMS is integrated with the certified ISO/IEC 27001:2022 / NEN 7510:2022 Information Security Management System, reusing its risk methodology, document control, internal audit, management review, competence, supplier and incident-management processes, and extending them with AI-specific controls.

## Definitions and Abbreviations

- **AIMS** — AI Management System (ISO/IEC 42001)
- **AI system** — a machine-based system that infers, from input, how to generate outputs
- **AISIA** — AI System Impact Assessment
- **DPIA** — Data Protection Impact Assessment (GDPR Art. 35)
- **SoA** — Statement of Applicability (Annex A controls)
- **LLM / ASR / SER** — Large Language Model / Automatic Speech Recognition / Speech Emotion Recognition
- **HITL** — Human-in-the-loop
- **UBO** — Ultimate Beneficial Owner

---

# 2. AIMS Governance Records

Single-file governance index (mirrors the ISMS Governance Records section). Approval and audit records live in this document and are linked below.

* [AIMS Review & Approval Log](#aims-review--approval-log)
* [AIMS Annual Audit Calendar 2026](#aims-annual-audit-calendar-2026)
* [Risk Acceptance Register (Section 4 §5)](#5-risk-acceptance-records)
* [Statement of Applicability (Section 5)](#5-statement-of-applicability-isoiec-42001-annex-a)
* [AI System Impact Assessments — AISIA (Section 6)](#6-ai-system-impact-assessments-aisia)
* [AI Evidence Log (AI_Evidence_Log.md)](https://github.com/rate-nl/ISO/blob/main/AI_Evidence_Log.md)
* [ISMS Evidence & Logs (Logs.md)](https://github.com/rate-nl/ISO/blob/main/Logs.md)

**Approval & signatures:** A single CEO sign-off in the [AIMS Review & Approval Log](#aims-review--approval-log) approves this AIMS and every embedded record. Signed evidence is held in the [Manager Approvals folder (Google Drive)](https://drive.google.com/drive/folders/1LVJoKFKQxtZmwX9v2lCjW-83h3gsYwyN). No inline signature blocks are used.

### AIMS Annual Audit Calendar 2026

| Activity | Scope | Planned | Lead | Status |
|---|---|---|---|---|
| Initial AIMS internal audit | All clauses 4–10 + Annex A | Q3 2026 | AI Technical Lead (independent review by AIMS Owner) | Planned |
| Initial AIMS management review | Full AIMS review | Q3 2026 | Inge Proost (CEO) | Planned |
| Pre-certification readiness review | Gap-closure verification | Q4 2026 | AI Technical Lead (+ external reviewer) | Planned |
| Annual AIMS internal audit | All clauses + Annex A | June 2027 | AI Technical Lead | Scheduled |

---

# 3. AI Management System (ISO/IEC 42001 Clauses 4–10)

## Clause 4 — Context of the Organization

### 4.1 Understanding the Organization and Its Context

**Internal issues relevant to AI:**

| Issue | Type | Relevance |
|---|---|---|
| Small team (2 principals) — limited segregation of duties | Internal | Risk governance requires compensating controls |
| Sensitive health-data domain — vulnerable users | Internal | High-impact AI failures; stringent requirements |
| Multi-entity structure (DineRate/CareRate/Vess) | Internal | AIMS must coordinate across legal boundaries |
| R&D / pilot stage (iVessy TRL 4–5) | Internal | Evidence gaps are expected; controlled environment required |
| In-house AI expertise concentrated in AI Technical Lead | Internal | Key-person risk; succession and knowledge-management needed |
| GPU/compute dependency for Vess360 training | Internal | Resource constraint affects retraining frequency |

**External issues relevant to AI:**

| Issue | Type | Relevance |
|---|---|---|
| EU AI Act (in force; application phased 2024–2027) | Regulatory | Transparency, consent, prohibited-use compliance required |
| GDPR / Wkkgz / Wabvpz | Regulatory | Special-category health data processing constraints |
| Healthcare sector trust in AI — adoption barriers | Market | Must demonstrate safety and explainability to clients |
| OpenAI/US-provider transfer exposure (CLOUD Act) | Political/Legal | Transitional risk; migration to EU-hosted models mitigates |
| Rapid advancement of AI models (obsolescence risk) | Technology | Versioning, drift monitoring, and migration planning required |
| Academic partnership (Avans, Erasmus MC) | Stakeholder | Validation, inclusion research, responsible-AI scrutiny |

**Context review:** This context analysis is reviewed at each annual management review and after any significant change to the external or internal environment. The next scheduled review is June 2027.

### 4.2 Interested Parties and Their Requirements

| Interested party | Key AI-related requirement | How addressed |
|---|---|---|
| Clients / patients (incl. vulnerable groups) | Safety, dignity, transparency, consent, fairness, privacy, ability to review/correct | Pre-session disclosure; consent logging; review/edit loop; no-storage of audio; DPIA |
| Informal caregivers | Reduced burden; clarity; not repeating information | iVessy FHIR-structured output; human-in-the-loop confirmation |
| Healthcare professionals / organizations | Reliable, explainable support; human oversight; data quality; integration | Schema-only output; confirmation loop; FHIR/HL7 output; DPAs |
| Regulators / supervisors (AP, market surveillance) | GDPR, EU AI Act, Wkkgz, Wabvpz compliance; auditability | DPIA; AIMS; consent records; 72h breach reporting; EU AI Act mapping |
| Knowledge partners (Avans, Erasmus MC) | Responsible AI; ethical validation; evidence | AISIA; fairness monitoring; pilot evidence; open engagement |
| AI/model/cloud suppliers | Clear data-use limits; security; incident responsibilities | Supplier DPAs; SCCs; supplier risk assessments; contractual obligations |
| Owners / management | Lawful, trustworthy, commercially viable AI | AI Policy; governance oversight; risk management; objectives |
| Employees / contractors | Clear guidelines; safe environment to raise concerns | AI Use Policy; awareness training; incident-reporting channel |

**Review:** Interested-party requirements are reviewed at each annual management review.

### 4.3 Scope of the AIMS

> The AIMS covers the **development, provision and operation of AI systems for voice-driven collection and structuring of care information, and for voice-based emotion recognition** — specifically **iVessy** and **Vess360** (and **Vera** upon operational launch) — within **DineRate B.V.** (KvK 55058590), operated by **CareRate B.V.** (KvK 61419214) and **Vess B.V.** (KvK 86159097). It includes all supporting people, processes, models, data and infrastructure; the organization's roles as **AI developer/provider** and **AI deployer**; current third-party AI use; and the planned migration of iVessy to EU/self-hosted models.

**AI systems in scope:**

| System | Description | Org role | AI stack | Stage | EU AI Act class |
|---|---|---|---|---|---|
| **iVessy** | Voice-driven assistant replacing care forms with multilingual dialogue; FHIR/HL7 output; no decisions; human-in-the-loop | Provider/developer + deployer | LLM: OpenAI (current, transitional) → Mixtral 8x7B (planned); ASR: local Whisper (planned); Emotion: Vess360 | Pilot (TRL 4→5) | Limited-risk + transparency obligations |
| **Vess360** | In-house voice-emotion model (6 Ekman emotions; wav2vec2-based); supportive context only; confidence ≥ 0.70 threshold | Provider/developer | Azure STT + Google Translate/Cloud Run/Vertex AI (EU regions) | Production / API | Emotion recognition — Art. 50 transparency obligations |
| **Vera** | Low-threshold patient app for spoken care information; planned Vess360 integration | Provider + deployer | To be finalized at launch | Planned — enters scope at first real-user-data processing | TBD at launch |

**Scope-entry trigger for Vera:** First processing of real user data (non-test). At that point, the AI Technical Lead immediately initiates: AISIA (Section 6 template), model card (Section 10), DPIA update (Section 9), SoA review (Section 5), and risk register update (Section 4).

**Not in AIMS scope:** CareRate/Rate.nl measurement platform (no AI/ML); EAGLE joint venture (separate governance); education/non-healthcare segments; fully anonymized data; corporate HR/finance.

**Exclusions from Annex A:** None — all controls are applicable.

### 4.4 The AI Management System

The organization establishes, implements, maintains and continually improves the AIMS in accordance with ISO/IEC 42001:2023. The AIMS is **integrated** with the existing ISO 27001:2022 ISMS, sharing: risk methodology, document control, internal audit programme, management review process, competence and training process, supplier management, and incident management — each extended with AI-specific requirements documented in this manual.

---

## Clause 5 — Leadership

### 5.1 Leadership and Commitment

Top management (CEO / AIMS Owner: Inge Proost) demonstrates commitment to the AIMS by:

| Commitment | Evidence |
|---|---|
| Approving the AI Policy, objectives, and risk treatment | CEO approval recorded in the AIMS Review & Approval Log and the Risk Acceptance Register (Section 4 §5) |
| Providing resources (people, compute, tooling) | Resource register (Section 7); budget allocation decisions |
| Integrating AIMS into business processes | AIMS is integrated with the ISMS; operational AI controls embedded in development process |
| Promoting responsible AI culture | AI Use Policy communicated to all staff; AI awareness included in training |
| Ensuring AIMS performance is reviewed | Annual management review (Section 12 procedure; Section 13 template) |
| Supporting AI Technical Lead in their role | Appointment documented in §5.3; resources provided |

**Review of leadership commitment:** Confirmed at each annual management review. Next due: June 2027.

### 5.2 AI Policy

**Full text of AI Policy — DineRate B.V. / Rate.nl**

*Version: 2.0 | Approved by: Inge Proost (CEO) | Date: 30 June 2026 | Review: Annual*

**Purpose and scope**

This policy governs the responsible development, provision and operation of all AI systems by DineRate B.V. and its entities (CareRate B.V., Vess B.V.). It applies to all employees, contractors, and third parties involved in AI activities within the AIMS scope.

**Our commitment**

The group develops and operates AI handling sensitive health information for vulnerable people. We are committed to doing so responsibly, lawfully, safely and transparently.

**Principles**

1. **Lawfulness & compliance** — All AI activities comply with GDPR, EU AI Act, Wkkgz, Wabvpz, ISO 27001, NEN 7510, and this AIMS. Voice/health data is special-category data and is treated with the highest level of protection.

2. **Human oversight — no autonomous decisions** — AI supports human professionals; it never makes autonomous decisions affecting individuals. iVessy collects and structures data; humans review and confirm before committing to records. Vess360 provides supportive emotional context only. No AI system in scope performs diagnosis, triage, profiling or behavioural steering.

3. **Transparency** — Users are informed before each session: (a) that they are interacting with AI; (b) the purpose of the AI; (c) the data processed (speech, content, emotion); (d) that audio is transient and not stored; (e) that emotion context may be shown to the professional; and (f) their GDPR rights including the right to withdraw consent. This disclosure is logged. Explicit consent is obtained and logged for each session. EU AI Act Art. 50 obligations are met for emotion recognition.

4. **Fairness & non-discrimination** — iVessy is monitored for performance differences across language, accent, dialect, and level of assistance. Vess360 is trained on diverse corpora and monitored at aggregate level. Observed performance gaps are investigated and addressed. No demographic data is stored by Vess360.

5. **Safety, robustness & reliability** — Deterministic guardrails are applied: schema-only output; rejection of extra text; clarification questions for ambiguous input; user confirmation before data commit. Vess360 emotion is displayed only at confidence ≥ 0.70; otherwise labelled "uncertain".

6. **Privacy & data governance** — Privacy by design. Audio is transient and not stored. Only structured output is retained. Tenant isolation is enforced. Inference is stateless. Patient data is not used to train models. Data provenance and consent for training data are documented.

7. **Security** — AI assets are protected under ISMS controls. AI-specific security threats (adversarial inputs, model poisoning, inference attacks) are assessed and controlled.

8. **Accountability & governance** — Clear roles and responsibilities (§5.3). Risk assessment, SoA, impact assessments, and this policy are maintained and reviewed. Non-conformities and AI incidents are logged and corrected.

9. **Lifecycle management** — Model cards are maintained for each AI model. Models are validated before deployment. Performance is monitored in operation. Significant changes (including the iVessy migration) follow the AI change management procedure.

10. **Supplier management** — AI suppliers are assessed for security posture, data-use terms, transfer exposure, and incident responsibilities. DPAs and SCCs are in place.

11. **Continual improvement** — The AIMS is monitored, audited, reviewed and improved. Lessons from incidents, audits, and pilots are incorporated.

**Prohibited uses**

The following uses of AI are explicitly prohibited within this organization:
- Real-time remote biometric identification in publicly accessible spaces
- Emotion recognition in workplace or education settings (EU AI Act Art. 5 prohibition)
- Social scoring systems
- AI that exploits vulnerabilities of individuals (age, disability, social situation)
- Any autonomous clinical decision-making (diagnosis, triage, prescribing)
- Using patient data to train models without explicit consent

**Policy ownership and review**

This policy is owned by the AIMS Owner (CEO). It is reviewed at least annually and after any significant change. Updates are approved by the CEO. All relevant personnel are informed of updates.

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

### 5.3 Organizational Roles, Responsibilities and Authorities

#### Role Assignment Record

| AIMS Role | Appointed person | Appointed by | Date | Scope of authority |
|---|---|---|---|---|
| **AIMS Owner** (accountable) | Inge Proost (CEO) | Board / Self | 18 Jun 2026 | Approves AI Policy, risk treatment, risk acceptance, objectives, SoA; provides resources; chairs management review |
| **AI Technical Lead** (responsible) | Firas Kassoumeh | CEO | 18 Jun 2026 | Implements and operates the AIMS; maintains risk register, SoA, model cards, registers; conducts risk assessments and impact assessments; leads incident response; reports to AIMS Owner |
| **All staff & contractors** | All personnel | CEO | Ongoing | Follow AI Policy and AI Use Policy; complete AI awareness training; report AI concerns via incident channel |

#### RACI Matrix

| Activity | AIMS Owner | AI Technical Lead | Staff |
|---|---|---|---|
| AI Policy & objectives | A | R | I |
| AI risk assessment & treatment | A | R | C |
| AI System Impact Assessment | A | R | C |
| SoA approval | A | R | I |
| Model cards & validation | I | A/R | — |
| Data governance | A | R | C |
| Supplier management | A | R | C |
| Internal audit | A | R (lead) | I |
| Incident response | A | R | C |
| Training & awareness | A | R | R (attend) |
| Management review | A/chair | R (prepare) | I |
| Change management (AI) | A | R | C |

**Segregation of duties note:** Rate is a small organization; AIMS roles are concentrated between two individuals. Compensating controls: (1) CEO independently approves all risk treatment, policy, and change decisions; (2) annual internal audit with independent review; (3) all privileged AI-system actions are logged; (4) external AI governance review planned at certification stage. This arrangement is formally accepted and reviewed annually.

---

## Clause 6 — Planning

### 6.1 Actions to Address Risks and Opportunities

#### 6.1.1 General

The AIMS uses the ISMS risk methodology extended with AI-specific risk sources and the AI System Impact Assessment. The process is documented in the AI Risk Assessment Procedure (Section 12).

**Opportunities identified:**
- Improved inclusion for low-literacy and non-native-speaking patients (iVessy)
- Reduced administrative burden on care professionals
- Standardized, structured FHIR data improving care continuity
- Emotional-context support improving professional awareness
- Positioning as responsible-AI leader in Dutch healthcare sector

**Opportunities are** tracked in the continual-improvement plan (Appendix A) and reviewed at each management review.

#### 6.1.2 AI Risk Assessment — Criteria

**Impact scale:**

| Level | Criteria |
|---|---|
| **High** | Serious harm to individuals (health, dignity, rights, privacy); legal non-compliance with significant penalty; reputational damage threatening business continuity |
| **Medium** | Moderate harm to individuals (distress, inconvenience, data quality error); regulatory finding without immediate enforcement; recoverable reputational impact |
| **Low** | Minimal harm; easily correctable error; no individual impact; minor operational disruption |

**Likelihood scale:**

| Level | Criteria |
|---|---|
| **High** | Will occur or has occurred; control environment weak; external threat active |
| **Medium** | May occur under specific circumstances; some controls in place |
| **Low** | Unlikely; strong controls; no active threat indicator |

**Risk matrix:**

| Impact ↓ / Likelihood → | Low | Medium | High |
|---|---|---|---|
| **High** | Medium 🟡 | High 🔴 | High 🔴 |
| **Medium** | Low 🟢 | Medium 🟡 | High 🔴 |
| **Low** | Low 🟢 | Low 🟢 | Medium 🟡 |

**Risk appetite:**
- **Low tolerance** for risks to safety, health, fundamental rights, legal compliance — must be treated to Low, or CEO-accepted with documented justification and monitoring
- **Moderate tolerance** for performance/accuracy risks during the pilot phase, provided human oversight and transparency are in place
- **Risk acceptance threshold:** Residual risks rated High are never accepted without CEO approval and a time-bound remediation plan

#### 6.1.3 AI Risk Treatment Options

| Option | Description | When used |
|---|---|---|
| Modify (mitigate) | Apply controls to reduce likelihood and/or impact | Preferred option |
| Retain (accept) | Document and formally accept the residual risk | Only for Low or, exceptionally, Medium risks with CEO approval |
| Avoid | Discontinue or change the activity causing the risk | When mitigation is not feasible or cost-effective |
| Share/Transfer | Transfer to a third party (DPA, insurance, contract) | For supplier-related risks |

All retained/accepted residual risks are recorded in the Risk Acceptance Register (Section 4 §4) and approved by the AIMS Owner (CEO).

#### 6.1.4 AI System Impact Assessment (AISIA) Process

The AISIA process follows ISO/IEC 42005. An AISIA is conducted:
- Before initial deployment of any AI system
- Before any significant change (new use case, new data, new model, hosting migration)
- After any material AI incident
- At least annually as part of management review

The AISIA assesses:
1. Purpose, intended use, and affected individuals
2. EU AI Act risk classification
3. Impacts: privacy, fairness, safety, autonomy, dignity, societal effects
4. Mitigations for each identified impact
5. Residual impact and acceptability
6. Decision: proceed / proceed with conditions / do not proceed

AISIAs are documented in Section 6, signed by the AI Technical Lead and approved by the AIMS Owner.

### 6.2 AI Objectives and Planning

| Objective | Metric | Target | Measurement method | Frequency | Owner | Status |
|---|---|---|---|---|---|---|
| Administrative efficiency | Intake-time reduction | ≥ 20% reduction vs. paper/traditional | Time-motion logs + EPD timestamps (WP2 pilot) | Per pilot cohort | AI Technical Lead | ⬜ Pending WP2 |
| Field extraction quality | Field accuracy / clarification rate | Field accuracy ≥ 90%; clarification rate trend ↓ | Validation set results | Per model version + pilot | AI Technical Lead | ⬜ Pending pilot |
| Emotion reliability | Confidence display; accuracy improvement | Confidence ≥ 0.70 maintained; accuracy > 0.48 baseline | Model evaluation report | Semi-annually | AI Technical Lead | 🔄 In progress |
| Fairness | Performance gap across monitored groups | No material gap (> 5% difference triggers review) | Subgroup performance analysis | Semi-annually | AI Technical Lead | ⬜ Pending |
| Model monitoring | Drift detection | Drift check conducted; retrain triggered on defined accuracy drop | Monitoring log (Section 13) | Semi-annually | AI Technical Lead | ⬜ Pending |
| Governance maturity | AIMS completeness | All evidence items ≥ 80% collected; internal audit clean | Evidence log (Section 14) | Annually | AI Technical Lead | 🔄 In progress |
| EU AI Act readiness | Compliance mapping | All applicable articles mapped and controlled | EU AI Act mapping (Section 15) | Annually | AI Technical Lead | 🔄 In progress |

**Objective measurement review:** AI objectives are reviewed at each management review. Where targets are not met, root cause analysis and corrective action are documented.

### 6.3 Planning of Changes

Any significant change to an AI system — including the iVessy migration OpenAI → EU → self-hosted — follows the AI Change Management Procedure (Section 12). Significant changes require:
1. Formal change request (Section 13 template)
2. Updated AI risk assessment (§6.1.2)
3. Updated AISIA (§6.1.4) if impact profile changes
4. Updated DPIA (Section 9) if data processing changes
5. Model validation before deployment (Section 12 validation procedure)
6. CEO approval for production deployment
7. SoA review if new controls are implicated

**iVessy migration change record:** See Section 13 — Change Request Record CR-2026-001.

---

## Clause 7 — Support

### 7.1 Resources

The AIMS Owner ensures the following resources are provided:

| Resource type | Resources allocated | Owner |
|---|---|---|
| Personnel | AIMS Owner (Inge Proost, 20% AIMS capacity); AI Technical Lead (Firas Kassoumeh, primary AIMS responsibility) | AIMS Owner |
| Compute (training) | GPU resources for Vess360 training (Azure Vertex AI EU); planned self-hosted GPU for Mixtral | AI Technical Lead |
| Compute (inference) | Hetzner EU (iVessy); Azure STT EU, Google Cloud Run EU (Vess360) | AI Technical Lead |
| Tooling | PyTorch, Hugging Face, Docker, GitHub, FastAPI, Whisper, FHIR libraries | AI Technical Lead |
| External expertise | External security review (ISMS); planned external AI governance review (AIMS certification) | AIMS Owner |
| Certification | ISO 42001 certification (DNV, planned); NEN 7510 certification (planned) | AIMS Owner |

### 7.2 Competence

**Competence criteria for AIMS roles:**

| Role | Required competencies | Verification method |
|---|---|---|
| AIMS Owner (CEO) | AI governance principles; EU AI Act overview; ISO 42001 scope; risk appetite setting; management review leadership | Annual AI governance training; external briefing |
| AI Technical Lead | ISO 42001:2023 detailed requirements; AI/ML engineering; responsible AI (bias, fairness, explainability); EU AI Act technical requirements; GDPR/healthcare data; AI security (adversarial ML); model evaluation and monitoring | Training records; certifications; demonstrated work product |
| All staff | Responsible AI principles; prohibited AI uses; how to identify and report AI concerns; basic data protection for AI | Annual AI awareness training |

**AIMS Owner (CEO) competence — compensating rationale:** The CEO's accountable role is governance, resource allocation and risk acceptance — not technical operation. Detailed technical execution (model validation, monitoring, security) sits with the AI Technical Lead under the documented RACI. The CEO's competence requirement (annual AI-governance briefing/course; ISO 42001 and EU AI Act executive overview; management-review leadership) is proportionate to this governance role and is reinforced by (a) the AI Technical Lead's detailed technical competence, (b) independent periodic review, and (c) management-review reporting that surfaces technical risk to the CEO in governance terms. This mirrors the ISMS segregation-of-duties compensating-control approach for a small organization.

**Training records:** See Section 13 — AI Competence & Training Records.

**Competence gaps:** Identified during the gap analysis conducted 30 June 2026. Remediation actions are in Appendix A items 1–2.

### 7.3 Awareness

All personnel within the AIMS scope are made aware of:
- The AI Policy and its key principles
- Their individual responsibilities under the AIMS
- The risks of using AI irresponsibly (bias, hallucination, over-reliance)
- Prohibited AI uses
- How to identify and report an AI concern or incident
- Consequences of non-compliance with the AI Policy

Awareness is delivered through:
- Annual AI awareness training session (combined with ISMS awareness where appropriate, with AI-specific content module)
- Onboarding briefing for new personnel
- This AIMS document (available in the repository)
- AI Use Policy (Section 11)

### 7.4 Communication

| Communication | Audience | Channel | Frequency | Owner |
|---|---|---|---|---|
| AI Policy updates | All staff | Email + repository | On update | AIMS Owner |
| AI performance reports | AIMS Owner | Management review | Annual | AI Technical Lead |
| AI incident notifications | Affected parties | Per incident procedure (Section 12) | As needed | AI Technical Lead |
| Transparency disclosure to users | Patients/clients | In-session disclosure (iVessy interface) | Per session | AI Technical Lead |
| Supplier communication | AI suppliers | DPA + contractual channels | As needed | AI Technical Lead |
| External transparency | Public / clients | AI transparency notice (to be published) | Annual | AI Technical Lead |
| Regulatory reporting | AP (GDPR breach); EU AI Act authorities | Per legal obligations | As triggered | AIMS Owner |

### 7.5 Documented Information

**Controlled documents (this AIMS):**

| Document | Location | Format | Review |
|---|---|---|---|
| AIMS manual (this document) | rate-nl/ISO repository | Markdown | Annual |
| AI Policy (Section 11) | rate-nl/ISO repository | Markdown (embedded) | Annual |
| AI Use Policy (Section 11) | rate-nl/ISO repository | Markdown (embedded) | Annual |
| All procedures (Section 12) | rate-nl/ISO repository | Markdown (embedded) | Annual |

**Operational records:**

| Record | Location | Retention | Owner |
|---|---|---|---|
| AI Evidence Log | rate-nl/ISO repository | 3 years | AI Technical Lead |
| Risk register | This document (Section 4) | 3 years | AI Technical Lead |
| SoA | This document (Section 5) | 3 years | AI Technical Lead |
| AISIAs | This document (Section 6) | 3 years | AI Technical Lead |
| DPIA | Google Drive (standalone) | Duration of processing + 3 years | AI Technical Lead |
| Supplier DPAs/SCCs | Google Drive | Duration of contract + 3 years | AIMS Owner |
| Training records | Google Drive | 3 years | AI Technical Lead |
| Audit records | Google Drive | 3 years | AI Technical Lead |
| Incident records | Google Drive + AI Evidence Log | 3 years | AI Technical Lead |
| Model cards | This document (Section 10) + GitHub | Per model lifecycle | AI Technical Lead |
| Consent logs | Application logs (encrypted) | Per session; meta-logs 1 year | AI Technical Lead |

---

## Clause 8 — Operation

### 8.1 Operational Planning and Control

All AI systems are operated within their documented intended use (§4.3, Section 6 AISIAs). Operational controls include:
- Pre-session disclosure and consent (per AI Policy §5.2, Principle 3)
- Human-in-the-loop confirmation before data is committed
- Schema-only output with guardrails
- Confidence thresholds for Vess360
- Tenant isolation and stateless inference
- Event logging (meta-information only; no audio stored)
- Monitoring against the objectives in §6.2

Operational deviations are treated as potential nonconformities per §10.1.

### 8.2 Operational AI Risk Assessment

The AI risk assessment (Section 4) is re-run when:
- A significant change is planned (new model, new hosting, new use case)
- An AI incident occurs
- A new regulatory requirement applies
- A supplier relationship changes materially
- At least annually as part of management review

Re-assessments are documented in the risk register with date, trigger, and assessor.

### 8.3 Operational AI Risk Treatment

Controls identified in the SoA (Section 5) are applied and verified. The AI Technical Lead confirms control effectiveness at each monitoring review and internal audit.

### 8.4 Operational AISIA/DPIA

AISIAs and the DPIA are updated before each new deployment or material change and reviewed at management review. The DPIA is a standalone signed document maintained in Google Drive (reference: Section 9).

---

## Clause 9 — Performance Evaluation

### 9.1 Monitoring, Measurement, Analysis and Evaluation

**What is monitored:** AI objectives (§6.2); Annex A control effectiveness; EU AI Act compliance indicators; incident trends; supplier performance.

**How monitored:**

| Indicator | Method | Frequency | Owner |
|---|---|---|---|
| Intake-time reduction | EPD log analysis vs. baseline | Per pilot cohort | AI Technical Lead |
| Field accuracy | Validation set testing | Per model release | AI Technical Lead |
| Emotion confidence rate | Inference log analysis | Monthly (when operational) | AI Technical Lead |
| Vess360 overall accuracy | Model evaluation | Semi-annually | AI Technical Lead |
| Fairness (subgroup analysis) | Per-group performance metrics | Semi-annually | AI Technical Lead |
| Model drift | Drift metric vs. baseline | Semi-annually | AI Technical Lead |
| AI incidents | Incident log review | Each incident + monthly summary | AI Technical Lead |
| Control effectiveness | Internal audit | Annually | AI Technical Lead |
| Supplier performance | DPA compliance review | Annually | AI Technical Lead |

**Results are** reviewed at management review and documented in the AI Evidence Log (Section 14).

### 9.2 Internal Audit

The AIMS internal audit is added to the ISMS audit programme. The audit covers all ISO 42001:2023 Clauses 4–10 and all Annex A controls using the AIMS Internal Audit Checklist (Section 13).

**Audit programme:**

| Audit | Scope | Frequency | Lead auditor | Next due |
|---|---|---|---|---|
| AIMS full audit | All clauses + Annex A | Annual | AI Technical Lead (with independent review) | Q3 2026 [FIRST AUDIT DUE] |
| AIMS focused audit | High-risk areas + open findings | Post-incident or before external assessment | AI Technical Lead | As triggered |

**Independence:** Given the small team size, the AI Technical Lead leads the audit with the AIMS Owner conducting independent review of findings. For the first certification audit, an external reviewer is recommended.

**Audit records:** See Section 13 — Internal Audit Checklist; records retained 3 years in Google Drive.

### 9.3 Management Review

The AIMS Owner (CEO) conducts an annual management review of the AIMS. The review uses the Management Review Record template (Section 13).

**Required inputs:**
- Internal and external issues relevant to AI (§4.1/4.2 changes)
- AI Policy and objectives status
- Risk register status and residual risks
- Annex A SoA control status
- AI incidents and nonconformities
- Internal audit results
- Supplier/partner performance
- Changes in legal/regulatory requirements (EU AI Act updates, GDPR)
- Continual improvement plan progress
- Resource adequacy

**Required outputs (documented decisions):**
- AIMS continuing suitability, adequacy and effectiveness
- Improvement actions (with owners and deadlines)
- Resource decisions
- Policy and objectives updates
- Risk acceptance decisions

**Management review records:** See Section 13 template; Google Drive; retained 3 years.

**Scheduled management reviews:**

| Date | Type | Chair | Record |
|---|---|---|---|
| [FIRST REVIEW DUE — Q3 2026] | Initial AIMS management review | Inge Proost | [To be completed] |
| June 2027 | Annual management review | Inge Proost | [Future] |

---

## Clause 10 — Improvement

### 10.1 Nonconformity and Corrective Action

When a nonconformity occurs (from audit, incident, monitoring, or other source):

1. **Contain** — take immediate action to contain the impact
2. **Record** — log in the Nonconformity & Corrective Action Log (Section 13)
3. **Investigate** — determine root cause
4. **Treat** — implement corrective action to eliminate root cause
5. **Verify** — confirm effectiveness of corrective action
6. **Close** — mark as closed when verified

**AI-specific nonconformity categories:**
- Bias/unfair outcome detected in monitoring
- Hallucination or incorrect structuring of care data causing patient-safety concern
- Consent not obtained or not logged
- Model drift exceeding the retrain threshold
- Supplier DPA breach
- EU AI Act or GDPR non-compliance finding
- Prohibited AI use detected

**Corrective action records:** See Section 13 — Nonconformity & Corrective Action Log.

### 10.2 Continual Improvement

The AIMS is continually improved through:
- Monitoring results → new improvement actions
- Audit findings → corrective and improvement actions
- Management review → strategic improvement decisions
- Incident lessons learned → process updates
- External developments (regulatory, technology) → policy and control updates

See Appendix A for the current continual improvement plan.

---

---

# 4. AI Risk Management (Register & Risk Acceptance)

**Method:** ISO/IEC 23894 / ISO 31000-aligned, integrated with ISMS risk process.
**Last reviewed:** 30 June 2026 | **Reviewed by:** Firas Kassoumeh | **Approved by:** Inge Proost (CEO)
**Next scheduled review:** June 2027 (or triggered by significant change/incident)

## 1. Risk Matrix (reference)

| Impact ↓ / Likelihood → | Low | Medium | High |
|---|---|---|---|
| **High** | Medium 🟡 | High 🔴 | High 🔴 |
| **Medium** | Low 🟢 | Medium 🟡 | High 🔴 |
| **Low** | Low 🟢 | Low 🟢 | Medium 🟡 |

## 2. iVessy Risk Register

| ID | Risk description | Likelihood | Impact | Inherent | Treatment option | Controls | Residual | Accepted by | Notes |
|---|---|---|---|---|---|---|---|---|---|
| iV-1 | Hallucination / incorrect structuring of care data committed to patient record | Medium | High | High 🔴 | Modify | Schema-only JSON output; reject extra text → clarification loop; FHIR field validation; mandatory human review and confirmation before commit to EPD | Low 🟢 | N/A — treated to Low | Guardrails confirmed in model card §8.1 |
| iV-2 | OpenAI (US) processing of identifiable health speech → GDPR transfer / CLOUD Act exposure | Medium | High | High 🔴 | Modify + planned Avoid | DPA + EU Standard Contractual Terms; minimize identifiable special-category data in prompts; transient processing only; migration to EU/self-hosted Mixtral planned (CR-2026-001) | Medium 🟡 | CEO accepted — see Risk Acceptance Record RA-AI-001 | Residual falls to Low after migration |
| iV-3 | ASR error / poor audio quality → incorrect transcription entered into care record | Medium | Medium | Medium 🟡 | Modify | ASR confidence score check; re-ask prompt if confidence low; slot/format validation; user review and confirmation | Low 🟢 | N/A — treated to Low | Whisper word-error-rate < 5% target |
| iV-4 | Performance bias across language / accent / level of assistance → unfair outcomes for subgroups | Medium | High | High 🔴 | Modify | Multilingual testing before deployment; fairness monitoring (semi-annual subgroup analysis); Avans inclusion research; plain-language design; multilingual ASR | Medium 🟡 | CEO accepted — see RA-AI-002 | iVessy in pilot; full monitoring activated at scale |
| iV-5 | Automation bias / over-reliance by professionals → patient safety risk | Medium | High | High 🔴 | Modify | 'Supportive only' framing in UI; mandatory human validation before record commit; professional training; no decision-making UI elements; contractual use restrictions | Medium 🟡 | CEO accepted — see RA-AI-003 | Training requirement for deploying healthcare org |
| iV-6 | Use beyond intended purpose (triage, diagnosis, behavioural profiling) by deploying organisation | Low | High | Medium 🟡 | Modify | Intended-use controls in product design; contractual use restrictions in DPAs; no decision-making features; professional onboarding | Low 🟢 | N/A — treated to Low | Contractual controls are primary |
| iV-7 | Tenant data leakage across sessions or organizations | Low | High | Medium 🟡 | Modify | Tenant isolation (separate encryption keys + namespaces); stateless inference; no audio stored; access controls; penetration test (ISMS) | Low 🟢 | N/A — treated to Low | Verified in ISMS security controls |
| iV-8 | Vulnerable users (low literacy, cognitive impairment, elderly) misunderstand or cannot engage with the AI | Medium | Medium | Medium 🟡 | Modify | Plain-language pre-session disclosure; multilingual support; review/edit/confirm interface; caregiver co-session option; AISIA social impact assessment | Low 🟢 | N/A — treated to Low | Avans inclusive-design research |
| iV-9 | iVessy migration (OpenAI → Mixtral) introduces new failure modes or regressions | Medium | High | High 🔴 | Modify | Formal change management (CR-2026-001); full model validation before deployment; parallel run testing; updated AISIA and DPIA; CEO approval before production switch | Low 🟢 | N/A — mitigated via process | Migration not yet executed |
| iV-10 | Adversarial input / prompt injection via user speech | Low | Medium | Low 🟢 | Modify | Schema-only output; prompt hardening; input sanitization; system-prompt not exposed; monitoring for anomalous outputs | Low 🟢 | N/A — treated to Low | Enhanced at Mixtral migration |

## 3. Vess360 Risk Register

| ID | Risk description | Likelihood | Impact | Inherent | Treatment | Controls | Residual | Accepted by | Notes |
|---|---|---|---|---|---|---|---|---|---|
| Ve-1 | Low emotion accuracy (~0.48 Dutch baseline) misleads professionals into incorrect clinical interpretation | High | High | High 🔴 | Modify | Supportive-only framing (no autonomous decision); confidence ≥ 0.70 threshold — below shown as "uncertain"; mandatory professional interpretation; accuracy-improvement objective (§6.2); never used for decisions | Medium 🟡 | CEO accepted — see RA-AI-004 | Accuracy improvement is tracked KPI |
| Ve-2 | Emotion misclassification bias (atypical expression, dialect, cultural variation) affects minority or vulnerable groups disproportionately | Medium | High | High 🔴 | Modify | Diverse training corpus (MSP-Podcast + DUTCHDES/DUTCHESS + own Dutch corpus); aggregate-level fairness review; documented limitation in model card; human interpretation required; no demographic data stored | Medium 🟡 | CEO accepted — see RA-AI-005 | Aggregate review; individual demographics not stored |
| Ve-3 | EU AI Act Art. 50 / emotion-recognition regulatory non-compliance | Low | High | Medium 🟡 | Modify | Explicit consent + disclosure before each session (Art. 50); medical context only; no workplace/education use (Art. 5 prohibition); no profiling; AIMS SoA Art. 50 mapping (Section 15) | Low 🟢 | N/A — treated to Low | Compliance mapped in Section 15 |
| Ve-4 | Azure/Google EU-region but US-headquartered provider → residual CLOUD Act / transfer exposure | Medium | Medium | Medium 🟡 | Modify | DPA + SCCs with Microsoft Azure and Google Cloud; EU regions specified contractually; transfer impact assessment (Section 9 §7); access controls; Azure/Google compliance certifications reviewed | Medium 🟡 | CEO accepted — see RA-AI-006 | Azure/Google regularly publish compliance reports |
| Ve-5 | MSP-Podcast training-data licence breach (reconstruction / raw-data redistribution) | Low | Medium | Low 🟢 | Modify | No raw-data redistribution policy; no model-reconstruction capability published; strict access control to training dataset; licence terms tracked in data register | Low 🟢 | N/A — treated to Low | Licence documented in Section 7 |
| Ve-6 | Model drift over time reduces reliability below acceptable threshold | Medium | Medium | Medium 🟡 | Modify | Semi-annual performance check against baseline; defined accuracy-drop retrain trigger; model versioning; rollback capability | Low 🟢 | N/A — treated to Low | First check due at 6 months post-launch |

## 4. Organizational / Cross-Cutting Risks

| ID | Risk description | Likelihood | Impact | Inherent | Controls | Residual | Accepted by |
|---|---|---|---|---|---|---|---|
| Org-1 | Key-person risk — AI Technical Lead unavailable → AIMS operation disrupted | Medium | High | High 🔴 | Knowledge documented in AIMS; model cards; procedures; CEO can access all systems; succession plan to be documented | Medium 🟡 | CEO accepted — see RA-AI-007 |
| Org-2 | GDPR personal data breach via AI system | Low | High | Medium 🟡 | Audio not stored; structured output only; encryption; access controls; ISMS incident process + 72h AP notification | Low 🟢 | N/A |
| Org-3 | EU AI Act classification error — iVessy retrospectively classified as high-risk | Low | High | Medium 🟡 | Intended-use controls; no decision features; monitoring regulatory developments; legal review at significant change | Low 🟢 | N/A |

## 5. Risk Acceptance Records

> These records formally document CEO acceptance of residual risks rated Medium. Per §6.1.3, accepted risks are monitored and reviewed at each management review.

### RA-AI-001 — iV-2: OpenAI US Transfer Exposure

| Field | Value |
|---|---|
| Risk ID | iV-2 |
| Risk | OpenAI (US) processing of health speech — GDPR/CLOUD Act transfer exposure |
| Residual risk | Medium 🟡 |
| Justification for acceptance | DPA and EU SCTs are in place. Data minimization applied. Migration to EU/self-hosted models is planned and in progress (CR-2026-001). This is a transitional risk with a defined remediation path. |
| Conditions | Monthly DPA compliance check; migration to EU/self-hosted Mixtral to be completed per roadmap; any new identifiable data type must be reviewed before processing |
| Accepted by | Inge Proost (CEO / AIMS Owner) |
| Date | 30 June 2026 |
| Next review | June 2027 or at migration completion |

### RA-AI-002 — iV-4: Language/Accent Bias

| Field | Value |
|---|---|
| Risk ID | iV-4 |
| Risk | Performance bias across language / accent / assistance level |
| Residual risk | Medium 🟡 |
| Justification for acceptance | iVessy is in a controlled pilot phase. Multilingual testing has been conducted. Avans inclusion research is ongoing. Human confirmation loop prevents incorrect data commitment. Fairness monitoring activated at scale. |
| Conditions | Semi-annual fairness subgroup analysis; any material gap (> 5%) triggers immediate investigation and remediation |
| Accepted by | Inge Proost (CEO / AIMS Owner) |
| Date | 30 June 2026 |
| Next review | June 2027 |

### RA-AI-003 — iV-5: Automation Bias

| Field | Value |
|---|---|
| Risk ID | iV-5 |
| Residual risk | Medium 🟡 |
| Justification | Mandatory human validation is a hard control. Training for deploying organizations is required contractually. Risk is that professional culture may still over-rely; residual medium accepted given human-in-the-loop architecture. |
| Conditions | Professional training is contractually required; monitoring of over-reliance complaints via incident channel |
| Accepted by | Inge Proost (CEO) |
| Date | 30 June 2026 |

### RA-AI-004 — Ve-1: Vess360 Low Accuracy

| Field | Value |
|---|---|
| Risk ID | Ve-1 |
| Residual risk | Medium 🟡 |
| Justification | Confidence threshold (≥ 0.70) and "uncertain" labelling reduce misleading outputs. Supportive-only framing prevents autonomous use. Accuracy improvement is a tracked objective. |
| Conditions | Confidence threshold maintained at ≥ 0.70; accuracy reviewed semi-annually; any decrease in accuracy below 0.40 triggers immediate suspension pending investigation |
| Accepted by | Inge Proost (CEO) |
| Date | 30 June 2026 |

### RA-AI-005 — Ve-2: Vess360 Bias

| Field | Value |
|---|---|
| Risk ID | Ve-2 | Residual risk | Medium 🟡 |
| Justification | Diverse corpus; aggregate fairness review. No individual demographic data stored — individual-level fairness analysis not possible by design. |
| Conditions | Corpus-level fairness review semi-annually; documented limitation disclosed to professionals |
| Accepted by | Inge Proost (CEO) |
| Date | 30 June 2026 |

### RA-AI-006 — Ve-4: Azure/Google Transfer Exposure

| Field | Value |
|---|---|
| Risk ID | Ve-4 | Residual risk | Medium 🟡 |
| Justification | EU regions specified; DPA + SCCs in place; EU-only data residency contractually guaranteed. US-headquartered provider is the residual concern. |
| Conditions | Annual DPA/SCC review; monitor Azure/Google compliance status; TIA on file |
| Accepted by | Inge Proost (CEO) |
| Date | 30 June 2026 |

### RA-AI-007 — Org-1: Key-Person Risk

| Field | Value |
|---|---|
| Risk ID | Org-1 | Residual risk | Medium 🟡 |
| Justification | Full AIMS documentation maintained. CEO has system access. For a 2-person organization this is inherent and accepted. |
| Conditions | AIMS documentation kept current; succession plan to be documented (Appendix A item 8) |
| Accepted by | Inge Proost (CEO) |
| Date | 30 June 2026 |

---

---

# 5. Statement of Applicability (ISO/IEC 42001 Annex A)

**SoA version:** 2.0 | **Date:** 30 June 2026 | **Approved by:** Inge Proost (CEO)
**Basis:** All Annex A controls are applicable; no exclusions.
**Status key:** ✅ Implemented | 🔄 Partially implemented (remediation in progress) | ⬜ Planned

## A.2 — Policies for AI

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.2.2 | AI policy | Yes | ✅ | AI Policy in Section 11 (§5.2); CEO approved v2.0 30 Jun 2026 | AIMS Owner | CEO approval recorded in the AIMS Review & Approval Log |
| A.2.3 | Alignment with other policies | Yes | ✅ | AIMS integrates with ISMS (readme.md); cross-reference in Appendix B | AI Technical Lead | None |
| A.2.4 | Review of AI Policy | Yes | ✅ | Annual review cycle defined; v2.0 reviewed 30 Jun 2026; documented in §5.2 | AIMS Owner | First review complete; next June 2027 |

## A.3 — Internal Organization

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.3.2 | Roles, responsibilities and authorities | Yes | ✅ | §5.3 RACI; role assignment record; SoD compensating controls; CEO approval of all policy/risk decisions | AIMS Owner | None |
| A.3.3 | Reporting of concerns | Yes | ✅ | ISMS incident channel (email to Managing Director); AI-specific categories added to incident log; AI Use Policy (Section 11) explains how to report; E-11 | AI Technical Lead | Ensure AI-specific categories communicated at training |

## A.4 — Resources for AI Systems

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.4.2 | Resource documentation | Yes | ✅ | AI Resource Register (Section 7 §1); updated 30 Jun 2026 | AI Technical Lead | None |
| A.4.3 | Data resources | Yes | ✅ | AI Data Register (Section 7 §2); MSP-Podcast licence; consent records; provenance documented | AI Technical Lead | None |
| A.4.4 | Tooling resources | Yes | ✅ | Tooling listed in Section 7 §1 | AI Technical Lead | None |
| A.4.5 | System and computing resources | Yes | ✅ | Hosting documented (Hetzner EU, Azure EU, Google EU) in Section 7 §1 | AI Technical Lead | None |
| A.4.6 | Human resources | Yes | 🔄 | Roles defined (§5.3); **GAP: AI competence criteria and training records — remediation: Section 13 training records; Appendix A items 1–2** | AIMS Owner | Complete training records per Section 13; due Q3 2026 |

## A.5 — Assessing Impacts of AI Systems

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.5.2 | Impact assessment process | Yes | ✅ | Process documented §6.1.4 and Section 12 (AISIA procedure) | AI Technical Lead | None |
| A.5.3 | Documentation of impact assessments | Yes | 🔄 | AISIAs in Section 6; approval recorded in the AIMS Review & Approval Log | AI Technical Lead | AISIA approval recorded in the AIMS Review & Approval Log |
| A.5.4 | Impact on individuals | Yes | ✅ | Section 6 AISIA — individual impact tables for iVessy and Vess360 | AI Technical Lead | None |
| A.5.5 | Societal impacts | Yes | ✅ | Section 6 AISIA — societal impact assessed for both systems | AI Technical Lead | None |

## A.6 — AI System Life Cycle

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.6.1 | Management guidance for responsible AI development | Yes | ✅ | AI Policy (§5.2); Section 8 lifecycle controls; model cards (Section 10) | AIMS Owner | None |
| A.6.2 | AI system life cycle (design→operation→monitoring; technical docs; event logs) | Yes | 🔄 | Controls documented Section 8; model cards Section 10; **GAP: validation records (E-8), monitoring logs (E-5), change records — remediation templates in Section 13** | AI Technical Lead | Complete before any live-patient-data processing |

## A.7 — Data for AI Systems

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.7.2 | Data for development and testing | Yes | ✅ | Data register (Section 7 §2); training/test split documented in model cards | AI Technical Lead | None |
| A.7.3 | Acquisition of data | Yes | ✅ | MSP-Podcast: licensed (non-exclusive, perpetual, commercial use); DUTCHDES/DUTCHESS: public terms; Own corpus: consented, anonymized | AI Technical Lead | None |
| A.7.4 | Quality of data | Yes | 🔄 | Multi-rater labelling described in model cards; **GAP: no documented quality metrics or records — remediation: data quality procedure and records in Section 12/XI** | AI Technical Lead | Complete data quality checks and records; due Q3 2026 |
| A.7.5 | Data provenance | Yes | ✅ | Full provenance in Section 7 data register; licence and consent chain documented | AI Technical Lead | None |
| A.7.6 | Data preparation | Yes | ✅ | Preprocessing procedure documented (Section 12 — PROC-DP-001); records via E-20 | AI Technical Lead | Complete data-quality records in pilot |

## A.8 — Information for Interested Parties

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.8.2 | Documentation and information for users | Yes | 🔄 | Consent/transparency flow described Section 8; **GAP: no user information sheet or consent form template — remediation: Section 13 user documentation** | AI Technical Lead | Create user information sheet and consent form template; due before pilot |
| A.8.3 | External reporting of adverse impacts | Yes | 🔄 | Public AI transparency notice + responsible-disclosure channel **drafted (Section 15)**; to publish on Rate.nl | AI Technical Lead | Publish notice on Rate.nl |
| A.8.4 | Communication of incidents affecting interested parties | Yes | ✅ | ISMS incident process extended for AI; Section 12 AI incident procedure; communication steps defined | AI Technical Lead | None (procedure in Section 12) |
| A.8.5 | Legal reporting obligations | Yes | ✅ | AP 72h GDPR breach notification; EU AI Act serious incident reporting (when applicable); Section 9 §6 | AIMS Owner | None |

## A.9 — Use of AI Systems

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.9.2 | Processes for responsible use | Yes | ✅ | Section 8 operational controls; AI Use Policy (Section 11); intended-use enforcement | AI Technical Lead | Evidence of operation required (E-9 consent logs, E-8 validation) |
| A.9.3 | Objectives for responsible use | Yes | ✅ | §6.2 objectives table; EU AI Act Art. 13 mapping (Section 15) | AIMS Owner | Measurement data required (E-1 to E-5) |
| A.9.4 | Intended use | Yes | ✅ | §4.3 scope; model cards (Section 10); contractual restrictions; no-decision-making design | AI Technical Lead | None |

## A.10 — Third-Party and Customer Relationships

| Ref | Control title | Applicable | Status | Implementation evidence | Owner | Gap/Action |
|---|---|---|---|---|---|---|
| A.10.2 | Allocating responsibilities in AI ecosystems | Yes | ✅ | Controller/processor roles defined Section 9 §1; DPAs allocate responsibilities | AIMS Owner | None |
| A.10.3 | Suppliers and third-party AI | Yes | 🔄 | Supplier register (Section 7 §3); **GAP: DPA evidence and supplier AI risk assessments not yet confirmed/documented — remediation: Section 13 supplier risk assessment template** | AI Technical Lead | Confirm DPAs; complete supplier risk assessments; due Q3 2026 |
| A.10.4 | Customers | Yes | ✅ | Customer DPAs define responsibilities; healthcare org is controller; CareRate/Vess B.V. are processors | AIMS Owner | Sample DPA to be filed as evidence |

---

---

# 6. AI System Impact Assessments (AISIA)

**Process basis:** ISO/IEC 42005; ISO 42001 Annex A.5
**Conducted by:** Firas Kassoumeh (AI Technical Lead)
**Approved by:** Inge Proost (CEO / AIMS Owner)
**Review trigger:** Before deployment, before significant change, after material incident, annually

---

## AISIA-001 — iVessy

| Field | Value |
|---|---|
| Assessment ID | AISIA-001 |
| System | iVessy |
| Version | 2.0 |
| Date | 8 July 2026 |
| Prepared by | Firas Kassoumeh (AI Technical Lead) |
| Approval | Recorded in the AIMS Review & Approval Log |
| Date | 30 June 2026 |
| Assessed by | Firas Kassoumeh (AI Technical Lead) |
| Approved by | Inge Proost (CEO / AIMS Owner) — recorded in the AIMS Review & Approval Log |
| Previous version | 1.0 (18 June 2026) |
| Trigger for this version | Gap-analysis remediation |
| Next review | Before iVessy OpenAI → Mixtral migration; or June 2027 (whichever first) |

**System description:**
iVessy is a multilingual, voice-driven assistant that replaces paper care-intake forms. A patient/client speaks; iVessy transcribes, structures, and populates FHIR/HL7 care-record fields via a dialogue interface. Output is reviewed and confirmed by a healthcare professional before committing to the EPD. iVessy does not diagnose, triage, profile, or make any decision affecting a patient. The professional remains fully in control.

**Current AI stack:** OpenAI LLM (transitional, US-based) + Whisper ASR (planned self-hosted) + Vess360 emotion (separate AISIA-002).

**Intended use:** Administrative intake data collection in healthcare settings. Not for clinical decision support, diagnosis, or autonomous action.

**Affected individuals:**
- Patients/clients (including elderly, low-literacy, cognitively impaired, non-native speakers)
- Informal caregivers (may co-participate in session)
- Healthcare professionals (receive and review output)

**Provisional EU AI Act classification:** Limited-risk + transparency obligations (Art. 13, Art. 50 for emotion component). Rationale: No decision-making capability; human-in-the-loop architecture; not in Annex III high-risk categories (not critical infrastructure, not employment, not access to services with autonomous decision). Classification reviewed at Mixtral migration.

**Decision:** Proceed in pilots with controls as documented. Do not proceed with live patient data until validation records (E-8) and consent logging (E-9) are operational.

**Impact assessment:**

| Impact area | Potential adverse impact | Severity (without controls) | Controls applied | Residual severity | Acceptable? |
|---|---|---|---|---|---|
| **Privacy** | Exposure of special-category health speech during OpenAI API call; potential US transfer | High | Transient processing (audio not stored); DPA + SCTs with OpenAI; structured output only; migration to EU/self-hosted planned | Medium (transitional) | Yes — CEO accepted RA-AI-001 |
| **Fairness** | Worse ASR/LLM performance for non-native speakers, dialects, or cognitively impaired users | High | Multilingual testing; Avans inclusion research; confirmation loop catches errors; monitored semi-annually | Medium | Yes — CEO accepted RA-AI-002 |
| **Safety / Data integrity** | Incorrect care field committed to EPD causing clinical error | High | Schema-only output; validation guardrails; mandatory human review and confirmation; no autonomous commit | Low | Yes |
| **Autonomy / Dignity** | Patient feels pressured or unable to correct AI output | Medium | Review/edit/confirm interface; user can stop at any time; plain-language explanation; multilingual | Low | Yes |
| **Transparency** | User unaware they are interacting with AI or that emotion is being analyzed | High | Pre-session disclosure (scripted); logged explicit consent; emotion disclosure per Art. 50; GDPR rights communicated | Low | Yes |
| **Societal** | Over-reliance leading to reduction in human skill; systemic bias at scale | Medium | Human-in-the-loop required; professional training required; pilot monitoring for systemic effects | Low | Yes |
| **Net societal benefit** | Improved inclusion for low-literacy/non-native patients; reduced admin burden; standardized data quality | Positive | Measured in WP2 pilot (E-1, E-2) | Positive | Yes |

**Conditions for deployment:**
1. Model validation record (E-8) completed and signed before any live patient data
2. Consent logging infrastructure operational and tested (E-9)
3. Professional training delivered at each deploying organization
4. DPIA signed (Section 9)
5. DPA with OpenAI confirmed and on file

---

## AISIA-002 — Vess360

| Field | Value |
|---|---|
| Assessment ID | AISIA-002 |
| System | Vess360 |
| Version | 2.0 |
| Date | 8 July 2026 |
| Prepared by | Firas Kassoumeh (AI Technical Lead) |
| Approval | Recorded in the AIMS Review & Approval Log |
| Date | 30 June 2026 |
| Assessed by | Firas Kassoumeh (AI Technical Lead) |
| Approved by | Inge Proost (CEO / AIMS Owner) — recorded in the AIMS Review & Approval Log |
| Next review | After first accuracy improvement iteration; or June 2027 |

**System description:** Vess360 is an in-house wav2vec2-based voice-emotion model classifying speech into 6 Ekman emotions (happy, sad, angry, fear, disgust, surprise) plus neutral. It outputs a predicted emotion label and a confidence score. Results are shown to healthcare professionals only when confidence ≥ 0.70; below this threshold the display reads "uncertain". Vess360 is used exclusively as supportive emotional context — never as the basis for clinical decisions.

**Intended use:** Supportive emotional context for healthcare professionals in sessions involving patient/client voice data, with prior explicit consent and disclosure.

**Prohibited uses (per AI Policy and EU AI Act):** Workplace emotion recognition; education setting emotion recognition; emotion recognition for social scoring or profiling; autonomous clinical decisions based on emotion; use without consent and disclosure.

**Affected individuals:** Patients/clients whose voice is analyzed for emotion.

**Provisional EU AI Act classification:** Emotion recognition system — Art. 50 transparency obligations apply. Not prohibited (medical context with professional oversight and consent). Not high-risk (no autonomous decision). Classification reviewed at scale-up.

**Decision:** Proceed in production with controls as documented.

**Impact assessment:**

| Impact area | Potential adverse impact | Severity (without controls) | Controls applied | Residual severity | Acceptable? |
|---|---|---|---|---|---|
| **Reliability** | Low accuracy (~0.48 baseline) misleads professional into incorrect clinical interpretation | High | Supportive-only framing; confidence ≥ 0.70 threshold; "uncertain" label; mandatory professional interpretation; accuracy-improvement objective | Medium | Yes — CEO accepted RA-AI-004 |
| **Fairness** | Bias for atypical expression, dialect, or cultural emotion expression | High | Diverse training corpus; aggregate fairness review; documented limitation disclosed to professionals | Medium | Yes — CEO accepted RA-AI-005 |
| **Privacy** | Inference of sensitive emotional state without awareness | High | Explicit consent and Art. 50 disclosure before each session; no demographic data stored; audio transient | Low | Yes |
| **Transparency** | Professional unaware of accuracy limitations | Medium | Documented in professional training; "uncertain" label; model card limitations section | Low | Yes |
| **Transfer** | Azure/Google EU-region but US-headquartered (CLOUD Act) | Medium | DPA + SCCs; EU regions; transfer impact assessment (Section 9 §7) | Medium | Yes — CEO accepted RA-AI-006 |
| **Autonomy** | Professional defers to AI emotion label without critical judgment | Medium | Supportive-only UI design; training; no decision UI elements | Low | Yes |
| **Societal** | Misuse for profiling or decisions at scale | High | No-decision rule enforced in design; contractual restrictions; no workplace/education use | Low | Yes |

---

## AISIA-003 — Vera (Preliminary pre-assessment — to be finalized at operational launch)

| Field | Value |
|---|---|
| Assessment ID | AISIA-003 |
| System | Vera |
| Status | PRELIMINARY — completed at pre-development stage; to be finalized, dated and approved before Vera processes real user data |
| Trigger | Vera scope-entry trigger: first processing of real user data |
| Prepared by | Firas Kassoumeh (AI Technical Lead) |
| Approval | To be recorded in the AIMS Review & Approval Log before launch |

### Preliminary assessment
| Item | Preliminary assessment |
|---|---|
| Intended use | Low-threshold patient app to record and listen back to spoken care information; planned voice-to-text and (later) Vess360 emotion support. Supportive/self-service; not a decision system; no diagnosis or triage. |
| Likely architecture | Mobile app (iOS/Android) + EU-hosted backend; ASR via self-hosted Whisper (group standard); optional Vess360 emotion (supportive-only, ≥ 0.70 threshold). To confirm at design. |
| Affected individuals | Patients/clients (incl. vulnerable groups); possibly informal caregivers. |
| Data categories | Voice recordings, transcribed content, possibly inferred emotion — special-category health data. |
| Provisional EU AI Act class | Limited-risk (self-service documentation) + transparency; emotion feature under Art. 50. Confirmed in final AISIA. |

### Preliminary impact & mitigation (to confirm at launch)
| Impact area | Potential impact | Preliminary mitigation | Provisional residual |
|---|---|---|---|
| Privacy | Vera may **store** voice recordings (unlike iVessy's transient audio) | Define retention + legal basis; encryption; user delete control; DPIA update | To assess |
| Transparency | User unaware of AI / emotion analysis | Pre-use disclosure + consent (Art. 50) | Low |
| Autonomy | Self-service use without professional oversight | Clear scope; no advice/decisions; signpost to care team | To assess |
| Fairness | ASR accuracy varies by accent/language | Multilingual testing; monitoring | To assess |
| Security | App-store distribution attack surface | ISMS mobile controls; store compliance | To assess |

### Known unknowns (resolve before launch)
- Whether recordings are stored (and if so, retention + legal basis) — the key difference from iVessy.
- Final architecture and hosting.
- Whether Vess360 emotion is enabled at launch or later.
- Controller/processor split (self-service vs. via healthcare org).

**On launch, this preliminary assessment is completed to full AISIA-001 depth, dated, and approved via the AIMS Review & Approval Log.**

---

---

# 7. Registers (Resources, Data, Suppliers, Models)

## 1. AI Resource Register (A.4.2, A.4.4, A.4.5, A.4.6)

**Last updated:** 30 June 2026 | **Owner:** Firas Kassoumeh

### AI models

| Model ID | Model | System | Description | Hosting | Status |
|---|---|---|---|---|---|
| MOD-001 | OpenAI LLM (gpt-4o-mini or equivalent) | iVessy | Dialogue + structuring (transitional) | OpenAI API (US) | Active — transitional |
| MOD-002 | Mixtral 8x7B Instruct | iVessy | Dialogue + structuring (planned replacement) | Self-hosted Hetzner EU | Planned |
| MOD-003 | Whisper (OpenAI, open-source) | iVessy | ASR — speech to text | Self-hosted (planned) | Planned |
| MOD-004 | Vess360 (wav2vec2-based) | Vess360 | Voice-emotion classification | Azure/Google EU | Production |

### Compute and infrastructure

| Resource | Provider | Region | Purpose | ISMS asset |
|---|---|---|---|---|
| Production server | Hetzner | EU (Germany) | iVessy API hosting | Yes |
| ASR/Whisper runtime | Hetzner EU (planned) | EU | Speech-to-text processing | Planned |
| Vess360 inference | Google Cloud Run | EU | Emotion model inference | Yes |
| Vess360 STT | Microsoft Azure | EU | Speech-to-text for Vess360 | Yes |
| Training compute | Google Vertex AI | EU | Vess360 model training | Yes |
| NAS backup | CEO home office (locked) | Netherlands | Backup storage | Yes (ISMS) |
| Development server | CEO home office (locked) | Netherlands | Development environment | Yes (ISMS) |

### Tooling

| Tool | Purpose | Licence |
|---|---|---|
| PyTorch | Model training | BSD |
| Hugging Face Transformers | Model library | Apache 2.0 |
| Docker | Container runtime | Apache 2.0 |
| GitHub (rate-nl/ISO) | AIMS document control | Commercial |
| FastAPI / Flask | API framework | MIT |
| FHIR libraries | Healthcare data structuring | Open-source |

### Human resources

| Role | Person | AI competence areas | Training status |
|---|---|---|---|
| AIMS Owner | Inge Proost | AI governance; EU AI Act overview; management review leadership | See Section 13 — Training Records |
| AI Technical Lead | Firas Kassoumeh | AI/ML engineering; ISO 42001; responsible AI; GDPR; EU AI Act technical; model evaluation | See Section 13 — Training Records |

## 2. AI Data Register (A.4.3, A.7.2–A.7.6)

**Last updated:** 30 June 2026 | **Owner:** Firas Kassoumeh

| Dataset ID | Dataset name | System | Source | Rights / Licence | Consent basis | Data type | Retention | Notes |
|---|---|---|---|---|---|---|---|---|
| DS-001 | MSP-Podcast (2,000-sample subset) | Vess360 training | UT Dallas (licensed) | Non-exclusive, perpetual; commercial model use permitted; no raw-data redistribution; no model reconstruction | Licence agreement | English-language emotional speech; 6 Ekman emotion labels | Model lifecycle | Licence document in Google Drive |
| DS-002 | DUTCHDES | Vess360 fine-tuning | Public (crowd-sourced) | Per dataset publication terms | Public dataset terms | Dutch emotional speech | Model lifecycle | Citation required in publications |
| DS-003 | DUTCHESS | Vess360 fine-tuning | Public | Per dataset publication terms | Public dataset terms | Dutch emotional speech | Model lifecycle | Citation required |
| DS-004 | Own Dutch corpus | Vess360 training/validation | In-house recordings | Informed consent; anonymized; technical metadata only | Explicit informed consent per participant | Dutch emotional speech (3 intensity variants × 6 emotions); multi-rater consensus labels | Model lifecycle + 5 years | Consent forms in Google Drive |
| DS-005 | Care protocols (anonymized) | iVessy RAG | Internal | Internal | N/A — no personal data | Dutch healthcare protocol text | Indefinite (public domain source) | No personal data |
| DS-006 | iVessy pilot dialogue (anonymized) | iVessy improvement | Pilot healthcare orgs | Explicit patient consent + DPIA | Art. 9(2)(a) + Art. 9(2)(h) | Structured FHIR fields + dialogue metadata (no audio) | 3 years | Only with explicit pilot consent; separate from production data |

**Data quality standards:**
- DS-004 (own corpus): multi-rater labelling (minimum 3 raters per sample); inter-rater agreement ≥ 0.70 Krippendorff's α required; quality check documented in model card §8.3
- DS-001–003: quality per source dataset documentation; verified at acquisition

## 3. AI Supplier Register (A.10.3)

**Last updated:** 30 June 2026 | **Owner:** Firas Kassoumeh

| Supplier ID | Supplier | Service | Data processed | Processing location | DPA status | SCC/transfer safeguard | Risk assessment | Review date | Status |
|---|---|---|---|---|---|---|---|---|---|
| SUP-001 | OpenAI Inc. | iVessy LLM API | Voice transcript text (health content, potentially identifiable) | US | 🔄 DPA confirmation required — file in Drive | OpenAI EU SCTs | 🔄 SAR drafted (due diligence begun); confirmation pending (Section 13 template) | Q3 2026 | Active — transitional |
| SUP-002 | Microsoft Azure | Vess360 STT | Voice audio (transient; EU region) | EU (Netherlands/Germany) | 🔄 Confirmation required | Azure DPA + SCC | 🔄 SAR drafted (due diligence begun); confirmation pending | Q3 2026 | Active |
| SUP-003 | Google Cloud | Vess360 Translate, Cloud Run, Vertex AI | Transcribed text; model inference (EU region) | EU | 🔄 Confirmation required | Google Cloud DPA + SCC | 🔄 SAR drafted (due diligence begun); confirmation pending | Q3 2026 | Active |
| SUP-004 | Mistral AI (Mixtral 8x7B) | iVessy LLM (planned self-hosted) | Model weights only (self-hosted; no API calls) | EU / on-prem | N/A — self-hosted | N/A — no data transfer | Licence review completed | At migration | Planned |
| SUP-005 | Hetzner | Hosting | Application data (encrypted) | EU (Germany) | ✅ ISMS DPA on file | EU-based; adequacy | Reviewed under ISMS | Annual | Active |
| SUP-006 | GitHub (Microsoft) | Code/AIMS repository | AIMS documents; code (no personal data) | EU | ✅ ISMS DPA on file | Reviewed under ISMS | Annual | Active |

**Supplier review process:** Supplier risk assessments are conducted using the template in Section 13. Results are reviewed at management review. Material changes to supplier terms trigger immediate re-assessment.

## 4. AI Model Register

| Model ID | Model name | Version | Training date | Validation date | Deployed date | Status | Model card |
|---|---|---|---|---|---|---|---|
| MOD-001 | OpenAI LLM | API (version per OpenAI release) | N/A | [To be completed — E-8] | Pilot use | Active | Section 10 §8.1 |
| MOD-002 | Mixtral 8x7B Instruct | TBD | TBD | TBD — pre-deployment | Not deployed | Planned | Section 10 §8.1 |
| MOD-003 | Whisper | TBD | N/A | TBD — pre-deployment | Not deployed | Planned | Section 10 §8.2 |
| MOD-004 | Vess360 v[X] | [current version] | [date] | [To be completed — E-8] | Production | Active | Section 10 §8.3 |

---

---

# 8. AI Lifecycle & Operational Controls (A.6, A.8, A.9)

## 1. AI Development Lifecycle Phases

All AI systems in scope follow this lifecycle. At each gate, the AI Technical Lead confirms completion and the AIMS Owner approves progression.

| Phase | Key activities | Gate criteria | Evidence required |
|---|---|---|---|
| **1. Concept & scoping** | Define intended use; identify affected individuals; initiate AISIA; check EU AI Act classification | AIMS Owner approves concept | AISIA initiated; risk assessment drafted |
| **2. Data acquisition & preparation** | Acquire/consent data; document provenance; preprocessing; quality check | Data quality criteria met; provenance documented | DS register entry; quality check record; consent documents |
| **3. Model development** | Training; architecture design; hyperparameter tuning; version control | Model card drafted; version tagged in Git | Model card (Section 10); Git tag |
| **4. Validation & testing** | Accuracy evaluation; fairness analysis; guardrail testing; adversarial testing | Validation targets met; fairness check complete; validation record signed | Model Validation Record (Section 13 — MVR) |
| **5. Impact, ethics & compliance review** | Finalize AISIA; **AI ethics review** (vulnerable-user & fairness checklist; optional external input from Avans / Erasmus MC); DPIA review; SoA check; EU AI Act check | AISIA and DPIA signed; **ethics review recorded**; SoA updated | Signed AISIA; DPIA sign-off; **Ethics Review Record (Section 13)**; SoA v update |
| **6. Deployment approval** | CEO approves production deployment | CEO approval documented | Change request (Section 13) with CEO approval |
| **7. Production operation** | Human-in-the-loop enforcement; consent logging; tenant isolation; event logging | All operational controls active | Consent logs; event logs |
| **8. Monitoring** | Semi-annual drift check; fairness review; incident monitoring; objective measurement | Monitoring log populated | Monitoring log (Section 13 — MML) |
| **9. Retrain / update** | Triggered by drift detection or accuracy drop; follows change management | Retrain criteria met; revalidated | Change request; new MVR |
| **10. Retirement** | Decommission model; archive model card; data deletion per schedule | Data securely deleted/archived | Decommission record |

## 2. Operational Controls — iVessy

### 2.1 Pre-session disclosure and consent (A.8.2, A.9.2)

Before each iVessy session begins, the following disclosure is presented to the user (patient/client) in the appropriate language:

---
*"This session uses an AI assistant to help record your care information. The AI will ask you questions and record your answers as structured data for your care team. Your voice is processed in real time and is not stored. If emotion analysis is used, your care professional may see an indication of your emotional tone — this is for context only and does not affect your care. You have the right to review, edit, and confirm all information before it is saved. You can stop at any time. For more information about how your data is processed, ask your care professional or contact us at [privacy contact]. By saying 'yes' or clicking Agree, you give consent to this AI-assisted session."*

---

The following items are logged per session (no audio stored):
- Session ID (pseudonymized)
- Tenant / healthcare organization ID
- Date and time
- Language used
- Consent given (yes/no) and timestamp
- Emotion analysis disclosed (yes/no)
- Session outcome (completed / abandoned / confirmation declined)

**Consent log location:** Application event logs (encrypted); meta-logs only; retained 1 year; accessible to AI Technical Lead for audit purposes.

### 2.2 Guardrails and output controls (A.9.2)

| Control | Implementation | Verification |
|---|---|---|
| Schema-only output | LLM constrained to JSON schema matching FHIR fields; any non-schema text rejected | Unit test suite; validation record |
| Clarification on ambiguity | If confidence is low or input is ambiguous → LLM generates clarification question | Test suite |
| User review and confirmation | Structured output presented to user before professional sees it; user can edit any field | UX design review |
| Professional confirmation | Professional reviews confirmed output before EPD commit | Process design; training |
| Tenant isolation | Separate encryption keys and namespaces per healthcare organization | Architecture review; pen test (ISMS) |
| Stateless inference | No conversation history persisted between sessions | Architecture review |
| Audio not stored | Audio stream processed in real time; no audio file written | Architecture review; code review |

### 2.3 Monitoring (A.6.2)

| Metric | Target | Method | Frequency |
|---|---|---|---|
| Field accuracy | ≥ 90% | Validation set testing | Per model release |
| Clarification rate | Trend ↓ | Inference log analysis | Monthly |
| Session completion rate | Trend ↑ | Event log analysis | Monthly |
| Consent rate | 100% (no session without consent) | Consent log | Each session |
| Tenant isolation verification | No cross-tenant data | Security log review | Quarterly |

## 3. Operational Controls — Vess360

### 3.1 Confidence threshold enforcement (A.9.2)

| Confidence score | Display action |
|---|---|
| ≥ 0.70 | Display predicted emotion label to professional |
| < 0.70 | Display "Uncertain — emotional context not available for this response" |
| Any score | Display: "This is AI-generated supportive context only. Use professional judgment." |

Threshold is hard-coded and logged. Any change to this threshold requires a formal change request, AISIA update, and CEO approval.

### 3.2 Consent and disclosure (A.8.2, EU AI Act Art. 50)

Before any session where Vess360 analyzes emotion, the user is informed:
- That voice-emotion analysis is being performed
- That results are supportive context for the professional only
- That results are based on AI with limited accuracy
- That they can decline emotion analysis (session continues without it)

Disclosure is logged with session ID and timestamp.

### 3.3 Monitoring (A.6.2)

| Metric | Target | Method | Frequency |
|---|---|---|---|
| Overall accuracy | > 0.48 (baseline) | Model evaluation on held-out test set | Semi-annually |
| Per-emotion F1 | Trend ↑ | Model evaluation | Semi-annually |
| Confidence distribution | ≥ 70% of predictions at threshold or above | Inference log analysis | Semi-annually |
| Fairness (corpus-level) | No material group gap | Subgroup accuracy analysis | Semi-annually |
| Drift vs. previous version | < defined threshold | Accuracy comparison | Semi-annually |

**Retrain trigger:** If overall accuracy drops more than 5 percentage points vs. the validated baseline, the AI Technical Lead initiates retraining per the change management procedure.

## 4. AI Incident Handling (A.8.4)

AI incidents are handled per the AI Incident Response Procedure (Section 12). AI-specific incident categories:

| Category | Examples | Initial response |
|---|---|---|
| Bias / unfair outcome | Systematic underperformance for a language group | Immediately log; assess scope; suspend affected use if patient safety at risk |
| Drift | Accuracy drop below retrain threshold | Log; initiate retraining; notify AIMS Owner |
| Hallucination / incorrect output | Care field populated with clearly wrong data | Log; review human-confirmation logs; assess if any erroneous data was committed |
| Adversarial input | Attempt to manipulate LLM via patient speech | Log; assess; patch prompt defenses |
| Privacy / data breach | Cross-tenant data exposure; audio retention error | Log; follow GDPR breach process (72h AP notification if required) |
| Consent failure | Session run without consent logged | Log; investigate; correct consent infrastructure; assess data subject notification |
| Supplier incident | OpenAI/Azure/Google reports breach | Log; follow DPA incident notification clause; assess data subject impact |

---

---

# 9. Data Protection Impact Assessment (DPIA)

> **Important:** This section contains the full DPIA text. For operational use, this DPIA should be extracted into a standalone signed PDF and stored in Google Drive. A signed standalone version supersedes this embedded version. Reference the standalone document as "DPIA-iVessy-Vess360-v2.0-[date].pdf" in the evidence log.

**DPIA version:** 2.0
**Date:** 30 June 2026
**Conducted under:** GDPR Art. 35; processing of special-category health data via AI
**Covers:** iVessy and Vess360
**Prepared by:** Firas Kassoumeh (AI Technical Lead)
**Reviewed and approved by:** Inge Proost (CEO / AIMS Owner) — recorded in the AIMS Review & Approval Log.
**Next review:** Before processing real patient data; before iVessy Mixtral migration; on any material change; annually

## §1 Roles — Controller / Processor

| Processing context | Data controller | Data processor(s) | Sub-processors |
|---|---|---|---|
| iVessy in clinical deployment (patient data) | Healthcare organization (client of Rate) | CareRate B.V. (KvK 61419214) — processes on behalf of controller | OpenAI Inc. (US) — transitional; Microsoft Azure (EU); Hetzner (EU) |
| Vess360 own-corpus model training | Vess B.V. (KvK 86159097) | Vess B.V. (self) | Google Cloud (EU); Microsoft Azure (EU) |
| iVessy model development (anonymized dialogue) | CareRate B.V. | CareRate B.V. (self) | N/A — anonymized data only |

**Processor obligations:** CareRate B.V. and Vess B.V. act as processors for healthcare organization clients. They process only on documented instructions in the DPA. No patient data is used to train models without explicit separate consent.

## §2 Description of Processing

### iVessy

| Item | Detail |
|---|---|
| Nature of processing | Real-time voice capture → ASR transcription → LLM structuring → FHIR field output → professional review → EPD commit |
| Data categories | Special-category health data (speech content describing health condition, care needs); voice audio (transient, not stored); structured FHIR/HL7 care fields |
| Data subjects | Patients and clients (including vulnerable groups: elderly, low-literacy, cognitively impaired, non-native speakers) |
| Scale | Pilot phase: ~100 clients per participating organization; scale-up post-WP2 |
| Recipients | Healthcare organization (controller receives FHIR output); AI sub-processors during processing only |
| Retention | Audio: NOT retained (transient real-time processing only); Structured FHIR output: per controller's EPD retention policy; Session meta-logs: 1 year |
| International transfers | OpenAI API (US) — transitional; DPA + SCTs in place; migration to EU/self-hosted planned |
| Automated decision-making | None — all decisions require human review and confirmation |

### Vess360

| Item | Detail |
|---|---|
| Nature of processing | Voice audio → Azure STT → text; text → Google Translate → English; transcribed text → Vess360 inference → emotion label + confidence; label shown to professional if confidence ≥ 0.70 |
| Data categories | Voice audio (transient); transcribed voice content; inferred emotional state (sensitive inference) |
| Data subjects | Patients/clients participating in iVessy sessions where emotion analysis is enabled |
| Automated inference | Emotion inference is automated; display is automated at threshold — but professional interpretation is mandatory |
| Retention | Audio: transient (not stored); transcription: transient (not stored); emotion label: displayed per session, not stored independently |
| International transfers | Microsoft Azure STT: EU region (Netherlands/Germany); Google Cloud: EU region; US-headquartered providers — SCCs in place |

### Vess360 training (own corpus)

| Item | Detail |
|---|---|
| Nature | Training of wav2vec2 emotion model on consented voice recordings |
| Data subjects | Volunteer participants (informed consent; adult; no patient data) |
| Retention | Training data retained for model lifecycle; participants informed of retention period at consent |
| No patient data | Patient data is never used to train or fine-tune any model |

## §3 Lawful Basis

| Processing | Lawful basis (Art. 6) | Special-category basis (Art. 9) | Notes |
|---|---|---|---|
| iVessy in clinical deployment | Art. 6(1)(b) — performance of contract; or Art. 6(1)(c) — legal obligation (Wkkgz) | Art. 9(2)(h) — healthcare provision; and/or Art. 9(2)(a) — explicit consent | Controller (healthcare org) determines basis; CareRate as processor processes on controller's instructions |
| AIMS-level processing (pre-session consent for AI use) | Art. 6(1)(a) — consent | Art. 9(2)(a) — explicit consent | Explicit logged consent obtained before each session |
| Vess360 own-corpus training | Art. 6(1)(a) — consent | Art. 9(2)(a) — explicit consent | Participant consent obtained at recording |

## §4 Necessity and Proportionality

The processing is limited to what is strictly necessary to achieve the purpose:
- **Data minimization:** Only care-relevant speech is processed; audio is not stored; only structured output (FHIR fields) is retained
- **Purpose limitation:** Data is used solely for the intake structuring session; not for any secondary purpose, marketing, or model training without separate consent
- **Storage limitation:** Audio = zero retention; structured output = per controller EPD policy
- **Accuracy:** Human confirmation loop ensures accuracy of stored data
- **Security:** Encryption in transit and at rest; tenant isolation; access controls per ISMS
- **Proportionality:** Administrative AI processing in healthcare is a proportionate use given the significant reduction in administrative burden and potential improvement in data quality and patient inclusion

## §5 Risks to Data Subjects and Measures

| Risk | Likelihood | Severity | Measures | Residual risk |
|---|---|---|---|---|
| Exposure of special-category health speech during OpenAI processing | Medium | High | DPA + SCTs; data minimization in prompts; transient processing; migration to EU/self-hosted planned | Medium → Low after migration |
| US-provider CLOUD Act exposure (OpenAI) | Low | High | DPA + SCTs; US government request would be resisted by OpenAI per their terms; migration planned | Medium |
| US-provider CLOUD Act exposure (Azure/Google EU) | Low | Medium | DPA + SCCs; EU-only data residency; contractual restrictions; Azure/Google compliance programs | Medium |
| Cross-tenant data leakage | Low | High | Tenant isolation (separate keys + namespaces); stateless inference; architecture review | Low |
| Incorrect care data committed to EPD | Medium | High | Human confirmation loop; schema guardrails; validation; user review | Low |
| Lack of informed consent | Low | High | Pre-session disclosure; explicit consent logging; user can withdraw at any time | Low |
| Profiling / re-identification via emotion data | Low | High | No demographic data stored; no cross-session tracking; supportive context only | Low |
| Training data breach (own corpus) | Low | Medium | Access controls; pseudonymization; consent; no raw-data redistribution | Low |

## §6 Breach Notification and Reporting

- Personal data breaches are handled per the ISMS incident process (readme.md §9, Incident Response Log)
- **Autoriteit Persoonsgegevens (AP):** Notified within **72 hours** of becoming aware of a breach where the breach is likely to result in a risk to rights and freedoms
- **Data subjects:** Informed without undue delay if the breach is likely to result in a high risk to their rights and freedoms
- **EU AI Act serious incidents:** Reported to market surveillance authority when the regulation applies to serious incidents or malfunctions (provisions phasing in)
- **Processor → Controller notification:** CareRate B.V. / Vess B.V. notify the controller (healthcare organization) without undue delay upon discovering a breach affecting controller's data (per DPA clause)

## §7 Transfer Impact Assessment (TIA)

### OpenAI (US)

| Item | Assessment |
|---|---|
| Transfer mechanism | EU Standard Contractual Terms (SCTs) — Controller-to-Processor |
| Processing location | OpenAI US data centers |
| Data minimization | Prompts are designed to minimize identifiable information; audio not transmitted (text only) |
| OpenAI data-use terms | OpenAI API terms: data not used to train models (per current API agreement); verify at each annual DPA review |
| CLOUD Act risk | US government could compel disclosure; OpenAI commits to legal challenge; cannot be eliminated |
| Compensating measures | SCTs; data minimization; migration to EU/self-hosted (eliminates risk) |
| TIA conclusion | Transfer is proportionate for the transitional period; risk is accepted (RA-AI-001); must be eliminated by migration |

### Microsoft Azure (EU regions)

| Item | Assessment |
|---|---|
| Transfer mechanism | Azure DPA + SCCs; EU data boundary commitment |
| Processing location | Netherlands/Germany Azure regions |
| Supplementary measures | EU data boundary; contractual restrictions on government access; Azure compliance attestations (ISO 27001, SOC 2) |
| CLOUD Act risk | Residual risk exists for US-headquartered provider; EU regions and DPA reduce but do not eliminate |
| TIA conclusion | Transfer is acceptable; residual risk accepted (RA-AI-006); annual review |

### Google Cloud (EU regions)

*Same assessment structure as Azure; TIA conclusion: acceptable with annual review and DPA.*

## §8 DPIA Conclusion

With the measures documented above, the residual risk is acceptable for pilot deployment. The DPIA must be:
1. **Reviewed and re-signed** before any processing of real patient data in production
2. **Updated** before the iVessy migration to Mixtral (new data-flow assessment required)
3. **Updated** when Vera enters scope
4. **Reviewed annually** as part of management review

**DPIA Controller consultation:** For deployments with healthcare organizations, the controller's own DPO/privacy officer should review and accept this DPIA or conduct their own assessment.

**Prior consultation with AP:** Not required at this stage — residual risk is not assessed as high after controls. If risk assessment changes, prior consultation will be initiated.

---

---

# 10. Model Cards

## 8.1 iVessy Dialogue LLM

| Field | Value |
|---|---|
| Model card ID | MC-001 |
| Version | 2.0 |
| Date | 30 June 2026 |
| Author | Firas Kassoumeh (AI Technical Lead) |
| Approved by | Inge Proost (CEO) — recorded in the AIMS Review & Approval Log |
| System | iVessy |
| Production status | Pilot — OpenAI (current); Mixtral (planned) |

### Model description

| Item | Current (OpenAI) | Planned (Mixtral 8x7B Instruct) |
|---|---|---|
| Architecture | Transformer (GPT-4 family) | Sparse Mixture-of-Experts Transformer |
| Parameters | Undisclosed | ~47B (active ~13B per token) |
| Access | OpenAI API | Self-hosted (Hetzner EU) |
| Quantization | N/A | GPTQ 4-bit (planned for efficiency) |

### Intended use

**In scope:**
- Generating natural, multilingual clarification questions based on care-intake schemas
- Structuring free-speech answers into FHIR/HL7 JSON fields
- Handling incomplete or ambiguous responses via clarification loops

**Out of scope (prohibited):**
- Diagnosis, triage, or clinical decision support
- Generating free-text clinical notes beyond defined schema fields
- Processing data outside the defined healthcare intake context
- Any use without prior user consent and disclosure

### Training and adaptation

| Item | Detail |
|---|---|
| Base model training data | OpenAI: undisclosed. Mixtral: public web corpus (Common Crawl, etc.) |
| Domain adaptation | RAG over Dutch care protocols; LoRA/QLoRA fine-tuning on: care-protocol Q/A; intake→FHIR extraction; safe-refusal examples; Dutch multilingual examples |
| Training data — patient data | NOT used. Only anonymized protocol documents and consented dialogue examples (DS-005, DS-006) |
| Fine-tuning record | [To be completed at Mixtral training — link to training run in GitHub] |

### Performance targets and validation

| Metric | Target | Baseline | Validation method |
|---|---|---|---|
| FHIR field accuracy | ≥ 90% | [To be measured — E-2] | Held-out test set with ground-truth FHIR annotation |
| Missing fields rate | Trend ↓ | [Baseline TBD] | Validation set |
| Contradiction rate | < 5% | [Baseline TBD] | Validation set |
| "Needs clarification" rate | Trend ↓ (but not zero — clarification is a feature) | [Baseline TBD] | Validation set |
| Safe refusal rate (out-of-scope input) | > 95% | [Baseline TBD] | Adversarial test set |

**Pre-deployment validation record:** See Section 13 — Model Validation Record MVR-001 (to be completed).

### Limitations

| Limitation | Mitigation |
|---|---|
| May mis-phrase or mis-structure low-frequency medical terms | Schema guardrails; clarification loop; human confirmation |
| Performance varies by language/accent | Multilingual testing; fairness monitoring; ASR confidence-based re-ask |
| Context window limit — long sessions may truncate | Session structured into defined schema; no long-form narrative required |
| Hallucination risk in high-uncertainty inputs | Schema-only output eliminates free-form hallucination; clarification loop handles uncertainty |

### Guardrails

1. **Schema-only JSON output** — any text outside the defined FHIR field schema is rejected by the output parser
2. **Clarification prompt** — low-confidence or ambiguous inputs trigger a re-ask
3. **User confirmation** — all structured output shown to the user for review/edit before professional sees it
4. **System prompt isolation** — system prompt not exposed to user; injection attempts captured in anomaly log
5. **Tenant isolation** — separate prompt namespaces per healthcare organization

### Rollback

Previous validated model version is retained in model registry for 90 days. Rollback decision is made by AI Technical Lead with CEO notification.

---

## 8.2 ASR — Whisper

| Field | Value |
|---|---|
| Model card ID | MC-002 |
| Version | 2.0 |
| Date | 30 June 2026 |
| System | iVessy |

| Item | Detail |
|---|---|
| Model | OpenAI Whisper (open-source; planned self-hosted) |
| Architecture | Transformer encoder-decoder |
| Intended use | Real-time multilingual speech-to-text transcription for iVessy input |
| Languages | Dutch (primary); French, German, English (secondary) |
| Hosting | Self-hosted on Hetzner EU (planned) — audio processed locally; not transmitted to external API |
| Audio retention | Audio is NOT stored — processed in real-time; transcript only is passed to LLM |
| Privacy benefit | Self-hosting eliminates third-party audio API exposure |

**Performance targets:**

| Metric | Target | Method |
|---|---|---|
| Word Error Rate (WER) — Dutch | < 10% | Benchmark on Dutch speech test set |
| WER — non-native Dutch | < 15% | Subgroup evaluation |
| Confidence scoring | Confidence score used to trigger re-ask below threshold | Per-token confidence analysis |

**Limitations:** Accuracy reduces with heavy accent, background noise, or speech impairment. Mitigated by: confidence-score-based re-ask; user confirmation of interpreted text; option to type instead of speak.

---

## 8.3 Vess360 Voice-Emotion Model

| Field | Value |
|---|---|
| Model card ID | MC-003 |
| Version | 2.0 |
| Date | 30 June 2026 |
| Author | Firas Kassoumeh (AI Technical Lead) |
| Approved by | Inge Proost (CEO) — recorded in the AIMS Review & Approval Log |
| System | Vess360 |

### Model description

| Item | Detail |
|---|---|
| Architecture | wav2vec2-base encoder (Facebook/Meta, open-source) + classification head |
| Output | 7 classes: happy, sad, angry, fear, disgust, surprise, neutral + per-class confidence scores |
| Operating rule | Display emotion only if top-class confidence ≥ 0.70; otherwise show "Uncertain" |

### Training data

| Dataset | Contribution | Quality assurance |
|---|---|---|
| MSP-Podcast subset (DS-001) | English-language cross-emotion pre-training | Licensed; multi-rater labels; no raw redistribution |
| DUTCHDES / DUTCHESS (DS-002, DS-003) | Dutch emotion fine-tuning | Public; per publication terms |
| Own Dutch corpus (DS-004) | Dutch validation and domain adaptation | Informed consent; 3 raters per sample; Krippendorff's α ≥ 0.70; anonymized |
| **No patient data** | Patient data is never used | N/A |

### Data quality record (DS-004)

| Quality criterion | Standard | Status |
|---|---|---|
| Raters per sample | ≥ 3 | ✅ Applied |
| Inter-rater agreement | Krippendorff's α ≥ 0.70 | [Record result here — E-3] |
| Consent documentation | Informed consent per participant | ✅ On file (Google Drive) |
| Anonymization | No identifying metadata retained | ✅ Technical metadata only |

### Performance

| Metric | Baseline | Latest result | Date | Model version | Target |
|---|---|---|---|---|---|
| Overall accuracy (Dutch) | ≈ 0.48 | [To be measured] | [Date] | [Version] | > 0.48 and improving |
| F1 — happy | — | [TBM] | — | — | — |
| F1 — sad | — | [TBM] | — | — | — |
| F1 — angry | — | [TBM] | — | — | — |
| F1 — fear | — | [TBM] | — | — | — |
| F1 — disgust | — | [TBM] | — | — | — |
| F1 — surprise | — | [TBM] | — | — | — |
| F1 — neutral | — | [TBM] | — | — | — |

**Note:** All performance metrics to be completed at first semi-annual evaluation (E-3). Results link to evidence log.

### Limitations

| Limitation | Impact | Mitigation |
|---|---|---|
| ~0.48 overall accuracy (Dutch baseline) | Significant risk of incorrect emotion display | Confidence threshold ≥ 0.70; "Uncertain" label; supportive-only framing; professional judgment required |
| Atypical expression (cognitive impairment, cultural variation) | Reduced reliability for some user groups | Corpus diversity; disclosed limitation; professional training |
| No individual demographic data stored | Cannot perform individual-level fairness analysis | Aggregate fairness review; corpus-level diversity |
| Training data not representative of all Dutch dialects | Possible dialect bias | Ongoing data collection; DUTCHDES/DUTCHESS inclusion |

### Operating rules (non-negotiable)

1. **Confidence threshold:** Display only at ≥ 0.70 — hardcoded; requires change request to modify
2. **Supportive context only:** Results are never the basis for autonomous action or clinical decision
3. **Disclosure required:** Art. 50 consent and disclosure before every session
4. **No profiling:** Results not stored against individual identifiers
5. **No workplace/education use:** Contractually prohibited; product design enforces
6. **Human judgment required:** UI communicates "professional interpretation required" with every result

### Prohibited uses

- Workplace emotion monitoring
- Education setting emotion monitoring
- Social scoring or profiling
- Autonomous clinical decision-making
- Use without explicit consent and disclosure

---

---

# 11. AI Policies

## AI Use Policy (for employees and contractors)

**Policy ID:** AUP-001
**Version:** 1.0 | **Date:** 30 June 2026 | **Approved by:** Inge Proost (CEO)
**Applies to:** All employees, contractors, and third parties working for or on behalf of DineRate B.V. / Rate.nl group

### Purpose

This policy defines the acceptable use of AI tools — including the organization's own AI systems (iVessy, Vess360) and external AI tools (e.g., ChatGPT, Copilot, Claude, Gemini) — by personnel. It complements the AI Policy (§5.2) and the ISMS Acceptable Use Policy.

### Scope

Applies to AI tool use in all work contexts: product development, administration, communication, research, data analysis.

### Permitted Uses

| Use | Conditions |
|---|---|
| iVessy and Vess360 in their documented intended use | Follow all operational controls in Section 8; user consent must be obtained |
| External AI tools (ChatGPT, Copilot, Claude, Gemini, etc.) for productivity | **No personal data, no health data, no confidential client data** may be entered into external AI tools |
| External AI tools for public-domain research and drafting | Verify all AI-generated output before use; cite as AI-assisted |
| External AI tools for code assistance | No patient data, no API keys, no proprietary algorithms entered; all AI-generated code reviewed by a developer before use |
| Approved internal tools | Per tool-specific guidance from AI Technical Lead |

### Prohibited Uses

The following are **strictly prohibited**:

1. Entering patient/client personal data, health data, or special-category data into any external AI tool (ChatGPT, Copilot, etc.)
2. Entering confidential business information, trade secrets, or unreleased product details into external AI tools
3. Using AI to make autonomous decisions affecting individuals without human review (automation bias)
4. Using AI for workplace emotion monitoring (EU AI Act Art. 5)
5. Using AI to generate content that impersonates real individuals without their consent
6. Bypassing security controls or review requirements by using AI tools
7. Using personal or unauthorized AI accounts for work purposes (only company-approved accounts and configurations)
8. Using AI to generate misleading, discriminatory, or harmful content
9. Using iVessy or Vess360 outside their documented intended use (see Section 6 AISIAs)

### Reporting

If you believe an AI tool has been misused, has produced harmful output, or you are uncertain whether a use is permitted — report immediately to Firas Kassoumeh (AI Technical Lead) via the standard incident-reporting channel.

Do not use judgment alone on borderline cases — ask first.

### Consequences

Violation of this policy may result in disciplinary action up to and including termination of employment or contract, and may involve legal liability.

### Acknowledgment

All personnel confirm acknowledgment of this policy as part of their annual AI awareness training. Training record is evidence of acknowledgment. [See Section 13 — Training Records]

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

---

## AI Incident Response Policy

**Policy ID:** AIRP-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Purpose

Ensure that AI incidents are detected, reported, contained, investigated, and corrected in a timely and structured manner that protects data subjects and the integrity of the AIMS.

### AI Incident Definition

An AI incident is any event, near-miss, or concern related to an AI system in scope that:
- Causes or could cause harm to a data subject (patient, user, professional)
- Indicates bias, unfairness, or discriminatory output
- Involves AI making autonomous decisions it is not authorized to make
- Constitutes a violation of the AI Policy or EU AI Act
- Involves a personal data breach via an AI system
- Indicates model drift beyond the retrain threshold
- Involves a supplier AI security incident

### Procedure

See Section 12 — AI Incident Response Procedure for the full step-by-step process.

### Reporting Obligation

All personnel who observe or suspect an AI incident **must report immediately** to the AI Technical Lead (Firas Kassoumeh) using the standard ISMS incident-reporting channel. Do not investigate alone. Do not attempt to fix AI output without reporting first.

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

---

## AI Data Governance Policy

**Policy ID:** ADGP-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Principles

1. **No patient data for training:** Patient or client health data is never used to train, fine-tune, or evaluate AI models without explicit separate consent from the data subject and approval from the controller. iVessy operational data is not used for model training.
2. **Audio not stored:** Voice audio is processed in real time and never written to persistent storage. Only structured text output is retained.
3. **Provenance documentation:** Every training dataset has documented provenance, licence, consent basis, and quality record in the data register (Section 7 §2).
4. **Licence compliance:** Licensing terms for all training data are tracked and complied with. The MSP-Podcast restriction (no raw-data redistribution; no model reconstruction) is enforced by access control and contractual obligation.
5. **Data minimization:** Only the minimum necessary data is processed. Identifiable information in iVessy prompts is minimized.
6. **Retention limits:** Audio: zero retention. Session meta-logs: 1 year. AIMS records: 3 years. Patient EPD data: per controller's policy.
7. **Quality standards:** Training data quality is checked and documented per the quality standards in model cards (Section 10) before use.
8. **Consent chain:** Consent for training data is documented in the data register. Consent for AI-session processing is obtained and logged per session.

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

---

## AI Training and Competence Policy

**Policy ID:** ATCP-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Required training — by role

| Role | Training content | Frequency | Delivery | Evidence |
|---|---|---|---|---|
| AIMS Owner (CEO) | AI governance; ISO 42001 overview; EU AI Act executive summary; AIMS management review responsibilities; risk acceptance | Annual | Internal session or external course | Training record in Section 13 |
| AI Technical Lead | ISO 42001:2023 detailed requirements; responsible AI (bias, fairness, explainability); EU AI Act technical requirements; GDPR for AI; AI security; model evaluation and monitoring; AI incident response | Annual + on significant regulatory change | External course + internal sessions | Training record in Section 13; certificates |
| All staff | AI Policy principles; prohibited AI uses; AI Use Policy; how to identify and report AI concerns; basic GDPR for AI; EU AI Act transparency obligations | Annual (combined with ISMS awareness) | Annual awareness session | Training record in Section 13 |
| New personnel | All-staff content above + role-specific content | At onboarding | Onboarding session | Onboarding training record |

### Competence assessment

AI Technical Lead competence is assessed by the AIMS Owner annually through:
- Review of work products (model cards, risk assessments, AISIAs, incident handling)
- Discussion of current regulatory and technical developments
- Review of any external training certificates

### Training records

Retained in Google Drive for 3 years. Template in Section 13.

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

---

## AI Supplier Management Policy

**Policy ID:** ASMP-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Requirements for AI suppliers

All suppliers providing AI models, AI APIs, or compute for AI processing must meet:

1. **DPA/SCC in place** — signed Data Processing Agreement (and SCCs for non-EU providers) before processing personal data
2. **EU data residency** — personal data of EU data subjects processed only in EU data centers (or with adequate safeguards documented)
3. **No model training on customer data** — contractual prohibition on using our data to train their models
4. **Security controls** — ISO 27001 certification or equivalent; SOC 2 Type II
5. **Incident notification** — contractual obligation to notify us of security incidents affecting our data within 24 hours
6. **Access controls** — documented access restrictions to our data; no broader access than required
7. **Audit rights** — we retain the right to audit or receive audit reports

### Supplier assessment process

Before engaging a new AI supplier:
1. Complete Supplier AI Risk Assessment (Section 13 template)
2. Confirm DPA/SCC in place
3. Review security certifications
4. Record in supplier register (Section 7 §3)
5. CEO approval for suppliers processing special-category health data

**Annual review:** Existing suppliers reviewed annually; any material change to supplier terms or security status triggers immediate reassessment.

*Approval recorded in the [AIMS Review & Approval Log](#aims-review--approval-log).*

---

---

# 12. Procedures

## AI Risk Assessment Procedure

**Procedure ID:** PROC-RA-001 | **Version:** 1.0 | **Date:** 30 June 2026

**Steps:**

1. **Trigger** — risk assessment is triggered by: new AI system; significant change; incident; annual review; new regulatory requirement
2. **Identify risks** — review the AI-specific risk sources listed in §6.1.2; interview relevant stakeholders; review incident log and audit findings
3. **Assess likelihood and impact** — use the scales in §6.1.2; document justification for each rating
4. **Calculate inherent risk** — apply the risk matrix
5. **Identify treatment** — select modify / retain / avoid / share per §6.1.3
6. **Apply controls** — reference Annex A controls (Section 5); document specific controls
7. **Calculate residual risk** — re-apply matrix post-controls
8. **Accept or escalate** — residual Low: AI Technical Lead accepts; residual Medium: AIMS Owner (CEO) signs Risk Acceptance Record (Section 13); residual High: must be re-treated or formally escalated with remediation deadline
9. **Update risk register** — add/update entry in Section 4 with date and assessor
10. **Communicate** — inform AIMS Owner of new Medium/High residual risks; schedule monitoring

**Record:** Section 4 — AI Risk Register; Section 13 — Risk Acceptance Record (for Medium/High accepted risks)

---

## AI System Impact Assessment Procedure

**Procedure ID:** PROC-AISIA-001 | **Version:** 1.0 | **Date:** 30 June 2026

**Steps:**

1. **Trigger** — new AI system; significant change; annual review; post-material-incident
2. **Describe the system** — purpose; intended use; affected individuals; EU AI Act classification
3. **Identify potential impacts** — use the impact areas from Section 6 as minimum: privacy, fairness, safety, autonomy, dignity, societal
4. **Rate severity without controls** — High / Medium / Low / Positive
5. **Document controls** — link to specific controls in Section 8, Section 5 (SoA), Section 9 (DPIA)
6. **Rate residual severity** — apply controls and re-rate
7. **Assess acceptability** — is the residual severity acceptable given the benefit?
8. **Decision** — Proceed / Proceed with conditions / Do not proceed
9. **Sign and date** — AI Technical Lead signs; AIMS Owner approves
10. **Update Section 6** — create or update the AISIA entry; update version history

---

## AI Incident Response Procedure

**Procedure ID:** PROC-IR-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Step 1 — Detect and Report (any personnel, immediately)
- Any AI concern or anomaly reported to AI Technical Lead via ISMS incident channel (email to managing director)
- Include: what was observed; when; which system; who was affected; what data was involved

### Step 2 — Initial triage (AI Technical Lead, within 2 hours)
- Log incident in AI Incident Log (Section 13 — E-11) with: ID, date/time, category, initial description
- Assess severity: Critical (patient safety; GDPR breach; system-wide bias) / High / Medium / Low
- If Critical: immediately notify AIMS Owner (CEO); consider system suspension

### Step 3 — Containment (AI Technical Lead, within 4 hours for Critical)
- Isolate affected component if patient safety is at risk
- Preserve logs and evidence (do not overwrite)
- If GDPR personal data breach: start the 72-hour AP notification clock

### Step 4 — Investigation (AI Technical Lead, 24–72 hours depending on severity)
- Determine root cause: model failure / data issue / process failure / supplier failure / adversarial input
- Assess scope: how many data subjects affected; what data; what time period
- Assess whether harm occurred or could occur

### Step 5 — GDPR breach assessment (if personal data involved)
- Is the breach likely to result in risk to rights and freedoms? If YES → notify AP within 72h of becoming aware
- Is risk HIGH? → also notify affected data subjects without undue delay
- Document assessment regardless of outcome

### Step 6 — Corrective action (AI Technical Lead)
- Implement immediate fix (hotfix; model rollback; process update)
- Document corrective action in Nonconformity & Corrective Action Log (Section 13)
- Update relevant controls, procedures, or model cards

### Step 7 — Communication
- Internal: AIMS Owner briefed; management review agenda item added
- External (if required): data subjects; AP; healthcare organization controller; EU AI Act authority (when applicable)
- Supplier: if supplier-caused, notify per DPA clause

### Step 8 — Close and learn
- Verify corrective action effectiveness
- Close incident in log with date and verified-by
- Document lessons learned; update risk register if new risk identified; update AIMS if process gap found
- Report at next management review

### AI Incident categories and initial response

| Category | Examples | Severity guidance | Key action |
|---|---|---|---|
| Patient safety | Incorrect care data committed without human review | Critical | Suspend; investigate; notify AIMS Owner immediately |
| GDPR breach | Cross-tenant exposure; audio retained in error | Critical | 72h AP clock starts; legal assessment |
| Consent failure | Session without logged consent | High | Investigate scope; assess notification |
| Bias detected | Systematic underperformance for a language group | High | Document; assess affected data; remediation |
| Hallucination | Care field with clearly wrong AI output | High | Review confirmation logs; assess if committed |
| Drift | Accuracy below retrain threshold | Medium | Initiate retraining; notify AIMS Owner |
| Adversarial input | Prompt injection attempt detected | Medium | Log; patch; monitor |
| Supplier incident | Supplier reports security event | High | Assess data impact; follow DPA notification clause |

---

## Data Preparation Procedure (Vess360 training)

**Procedure ID:** PROC-DP-001 | **Version:** 1.0 | **Date:** 8 July 2026

Applies to preparing voice data for Vess360 training/fine-tuning (A.7.4, A.7.6).

**Steps:**
1. **Source & consent check** — confirm dataset licence/consent (MSP-Podcast licence; DUTCHDES/DUTCHESS terms; own-corpus consent). Record in the Data Register.
2. **Ingestion** — import audio; verify integrity/format; pseudonymize identifiers.
3. **Cleaning** — noise reduction; normalise sample rate/loudness; remove unusable segments.
4. **Segmentation & diarization** — split into utterances; separate speakers where relevant.
5. **Labelling** — psychologists label emotion; multi-rater consensus voting; record inter-rater agreement (Krippendorff's α ≥ 0.70 target).
6. **Quality check** — class balance and label distribution; re-review low-agreement items; document metrics.
7. **Split** — train/validation/test split; prevent speaker leakage across splits.
8. **Versioning** — version the dataset; link to model card and Data Register (DS-004).
9. **Record** — complete the data-quality record (evidence E-20).

**Outputs:** versioned prepared dataset; data-quality record; inter-rater agreement record.

---

## AI Change Management Procedure

**Procedure ID:** PROC-CM-001 | **Version:** 1.0 | **Date:** 30 June 2026

**Significant changes requiring this procedure:** new AI model version; change of hosting/cloud provider; new use case; new data type processed; change to guardrails or confidence thresholds; new AI system entering scope.

**Steps:**

1. **Initiate** — AI Technical Lead submits Change Request (Section 13 — CR template) with description, justification, and proposed timeline
2. **Risk assessment** — re-run AI risk assessment (PROC-RA-001); document changes to residual risks
3. **AISIA update** — if impact profile changes, update or re-run AISIA (PROC-AISIA-001)
4. **DPIA update** — if data processing changes, update DPIA (Section 9); re-sign
5. **SoA review** — confirm no new Annex A controls are implicated; update SoA if needed
6. **Validation** — complete the Model Validation Record (MVR) for any new model version and apply the **Model Deployment Decision Rule** (Section 13): deploy only on a **Go**, or a CEO-approved **Conditional Go** with an improvement plan and enhanced monitoring; a **No-Go** blocks deployment
7. **EU AI Act review** — confirm risk classification remains appropriate
8. **CEO approval** — AIMS Owner approves before any production deployment
9. **Deploy** — implement change; update model register (Section 7 §4)
10. **Post-deployment monitoring** — enhanced monitoring for 30 days post-deployment; log results

**Current active change request:** CR-2026-001 — iVessy migration OpenAI → Mixtral (see Section 13)

---

## AI Monitoring and Performance Review Procedure

**Procedure ID:** PROC-MON-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Monthly monitoring (AI Technical Lead)
- Review consent logs — confirm 100% consent rate; no sessions without consent
- Review inference anomaly log — flag any unusual output patterns
- Review AI incident log — confirm all incidents closed or in progress
- Review clarification rate trend (iVessy)

### Semi-annual monitoring (AI Technical Lead, report to AIMS Owner)
- **Model drift check** — compare current accuracy metrics against validated baseline
  - If drift > 5 percentage points: initiate retraining per CR procedure
  - Document in Monitoring Log (Section 13 — MML)
- **Vess360 accuracy evaluation** — run full evaluation on held-out test set; document per-emotion F1
- **Fairness analysis** — subgroup analysis for iVessy (language, accent, assistance level) and Vess360 (corpus-level)
- **Confidence threshold review** — confirm ≥ 0.70 threshold is still appropriate given current accuracy
- **Supplier compliance check** — confirm supplier DPAs remain current; review any supplier security disclosures
- Report to AIMS Owner; update evidence log (Section 14)

### Annual monitoring (AIMS Owner + AI Technical Lead, at management review)
- Full review of all AI objectives (§6.2) — have targets been met?
- Full evidence log review (Section 14) — are all evidence items collected?
- Internal audit results review (Section 13 — audit checklist)
- SoA review — all controls still applicable and implemented?
- Risk register review — residual risks still appropriate?
- EU AI Act regulatory developments — any new requirements?
- Continual improvement plan progress (Appendix A)

---

## AIMS Internal Audit Procedure

**Procedure ID:** PROC-AUDIT-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Audit programme

| Audit | Frequency | Lead | Scope |
|---|---|---|---|
| Annual AIMS audit | Annual | AI Technical Lead (AI Technical Lead performs; AIMS Owner reviews for independence) | All ISO 42001 Clauses 4–10; all Annex A controls |
| Pre-certification audit | Before external assessment | External reviewer (recommended) | Full scope |
| Focused audit | Post-incident or post-significant-change | AI Technical Lead | Relevant clauses/controls |

### Audit steps

1. **Plan** — define scope, criteria (this AIMS; ISO 42001:2023), schedule, auditor
2. **Prepare** — review previous audit findings; review evidence log; prepare audit checklist (Section 13)
3. **Conduct** — interview AIMS Owner and AI Technical Lead; review documented information; verify evidence; test controls
4. **Record findings** — document each finding as: Conforming / Nonconformity (major/minor) / Observation / OFI
5. **Report** — issue audit report to AIMS Owner within 5 working days of completion
6. **Corrective actions** — for each nonconformity, AI Technical Lead defines corrective action and timeline; AIMS Owner approves
7. **Follow-up** — verify corrective action effectiveness within agreed timeline
8. **Close** — mark findings closed in audit record; update Nonconformity Log (Section 13)

**Audit records retained:** 3 years in Google Drive.

---

## AIMS Management Review Procedure

**Procedure ID:** PROC-MR-001 | **Version:** 1.0 | **Date:** 30 June 2026

### Frequency: Annual minimum; extraordinary review triggered by significant incident or regulatory change

### Inputs (AI Technical Lead prepares, AIMS Owner reviews)

1. Status of actions from previous management review
2. Changes in external/internal issues (§4.1/4.2)
3. AI objectives status and measurement data (§6.2)
4. AI incidents and nonconformities (Section 13)
5. Internal audit results (Section 13 — audit records)
6. SoA and risk register status (Section 4/III)
7. Supplier performance (Section 7 §3)
8. EU AI Act and regulatory developments
9. Resource adequacy
10. Continual improvement plan progress (Appendix A)

### Outputs (documented in Management Review Record — Section 13)

1. AIMS suitability, adequacy, and effectiveness conclusion
2. Improvement actions — owner, deadline, priority
3. Resource decisions
4. Policy or objective updates
5. Risk acceptance decisions
6. Changes to scope or SoA (if needed)

### Record

Management Review Record (Section 13 template) completed and signed by AIMS Owner. Retained 3 years in Google Drive. Referenced in evidence log (Section 14 — E-12).

---

---

# 13. Record Templates

## AI Competence Criteria and Training Records

**Record ID:** TR-AIMS | **Retention:** 3 years | **Owner:** AI Technical Lead

### Competence criteria

| Role | Competence area | Evidence standard | Assessment method |
|---|---|---|---|
| AIMS Owner | ISO 42001 overview; EU AI Act executive; AIMS management review | Annual briefing or external course ≥ 2 hours | Training record; attendance confirmation |
| AI Technical Lead | ISO 42001 detailed; responsible AI; EU AI Act technical; GDPR; AI security; model evaluation | Formal course or equivalent experience evidenced; annual update | Certificate or training record; work-product review |
| All staff | AI Policy; AI Use Policy; prohibited uses; incident reporting | Annual 30-min awareness session | Attendance record |

### Training register — [RECORD — complete for each session]

| Date | Participant | Role | Training topic | Delivery method | Duration | Trainer/Provider | Evidence link | Status |
|---|---|---|---|---|---|---|---|---|
| [Date] | Inge Proost | AIMS Owner | ISO 42001 overview + EU AI Act executive + AIMS management review responsibilities | Internal session | [duration] | Firas Kassoumeh | [Google Drive link] | ⬜ |
| [Date] | Firas Kassoumeh | AI Technical Lead | ISO 42001:2023 requirements + responsible AI + EU AI Act technical + GDPR for AI + AI security | [Course/internal] | [duration] | [Provider] | [Google Drive link] | ⬜ |
| [Date] | All staff | All | AI awareness: AI Policy, AI Use Policy, prohibited uses, incident reporting | Annual awareness session | 30 min | Firas Kassoumeh | [MoM link] | ⬜ |

**Next training due:** Q3 2026 (first AI-specific training session — Appendix A item 1)

---

## Model Validation Record

**Template ID:** MVR | **Retention:** 3 years

### Model Deployment Decision Rule (Go / Conditional Go / No-Go)

Applies to every Model Validation Record (MVR) below. The AI Technical Lead records the outcome; the CEO approves any **Conditional Go** in the AIMS Review & Approval Log.

**Gate types**
- **Hard gates (safety & rights)** — any FAIL = automatic **No-Go**, no override, no conditional deployment. These are: schema-only output = 100%; tenant isolation = no cross-tenant data; safe-refusal ≥ 95%; (Vess360) confidence-threshold enforcement = 100% and "uncertain" labelling = 100%.
- **Performance gates** — measured against a target, a conditional band, and a floor.

**Performance gate thresholds — iVessy**

| Metric | Go (≥ target) | Conditional Go (CEO-approved) | No-Go (below floor) |
|---|---|---|---|
| FHIR field accuracy | ≥ 90% | 85.0–89.9% | < 85% |
| Missing-fields rate | < 10% | 10–15% | > 15% |
| Contradiction rate | < 5% | 5–8% | > 8% |
| Multilingual accuracy (each language) | ≥ 85% | 80–84.9% | < 80% |

**Overall decision logic**
1. Any **hard gate FAIL** → **No-Go** (do not deploy; remediate and re-validate).
2. All hard gates pass **AND** all performance metrics ≥ target → **Go**.
3. All hard gates pass **AND** one or more performance metrics in the conditional band → **Conditional Go**, permitted only with: (a) CEO approval recorded in the Review & Approval Log; (b) a documented improvement plan with a re-test date; (c) enhanced monitoring; and (optionally) a restricted/supervised pilot scope.
4. Any performance metric **below its floor** → **No-Go**.

**Worked example (answers "what if accuracy is 87%?"):** FHIR field accuracy = 87% with all hard gates passing → **Conditional Go** — deploy only in a supervised pilot with CEO approval, an improvement plan, and enhanced monitoring; production scale-up requires ≥ 90%.

**Vess360 note:** Vess360 is supportive-only and never drives a decision, so its deployment gate is the **safety controls** (confidence-threshold enforcement, "uncertain" labelling, disclosure/consent, no-autonomous-use) — not raw accuracy. Emotion accuracy is a tracked **improvement objective** (§6.2), not a deployment floor. Vess360 deployment is **No-Go** only if a safety gate fails.

### MVR-001 — iVessy LLM (OpenAI current / Mixtral planned)

| Field | Value |
|---|---|
| Record ID | MVR-001 |
| Model | iVessy LLM |
| Version | [Complete at validation] |
| Validated by | Firas Kassoumeh (AI Technical Lead) |
| Validation date | [To be completed before live deployment] |
| Approved by | Inge Proost (CEO) — recorded in the AIMS Review & Approval Log |

| Test | Target | Result | Pass/Fail |
|---|---|---|---|
| FHIR field accuracy (held-out test set, n≥50) | ≥ 90% | [TBM] | [TBM] |
| Missing fields rate | < 10% | [TBM] | [TBM] |
| Contradiction rate | < 5% | [TBM] | [TBM] |
| Safe refusal (out-of-scope adversarial inputs, n≥20) | > 95% refusal rate | [TBM] | [TBM] |
| Schema-only output enforcement (no free text) | 100% | [TBM] | [TBM] |
| Multilingual (Dutch, French, German, English) | ≥ 85% accuracy each | [TBM] | [TBM] |
| Tenant isolation test | No cross-tenant data in output | [TBM] | [TBM] |

**Deployment decision:** Go / Conditional Go / No-Go — per the Model Deployment Decision Rule above; Conditional Go and final approval recorded in the AIMS Review & Approval Log.
**Evidence link:** [Google Drive / GitHub]

---

### MVR-002 — Vess360

| Field | Value |
|---|---|
| Record ID | MVR-002 |
| Model | Vess360 |
| Version | [Complete at validation] |
| Validation date | [To be completed] |

| Test | Target | Result | Pass/Fail |
|---|---|---|---|
| Overall accuracy (Dutch test set) | > 0.48 baseline | [TBM] | [TBM] |
| F1 per emotion (all 7 classes) | Documented | [TBM] | [TBM] |
| Confidence threshold enforcement (≥ 0.70 gate) | 100% correct | [TBM] | [TBM] |
| "Uncertain" label when confidence < 0.70 | 100% correct | [TBM] | [TBM] |
| Fairness (subgroup analysis — corpus level) | No material gap | [TBM] | [TBM] |
| Inter-rater agreement (DS-004) | Krippendorff's α ≥ 0.70 | [TBM] | [TBM] |

**Deployment decision:** Go / Conditional Go / No-Go — per the Model Deployment Decision Rule above; Conditional Go and final approval recorded in the AIMS Review & Approval Log.

---

## Consent and Transparency Log

**Record ID:** CTL | **Retention:** 1 year (meta-logs) | **Owner:** AI Technical Lead

> Note: This log captures aggregate and audit-sample data. Individual session consent is logged in the application event log (encrypted). This register provides the audit trail.

| Log ID | Date | System | Pilot / Org | Total sessions | Consent obtained (%) | Emotion disclosure shown (%) | Sessions abandoned before consent (%) | Sample export link | Audited by | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| CTL-001 | [Date] | iVessy | [Org name] | [n] | [%] | [%] | [%] | [Google Drive] | Firas Kassoumeh | ⬜ |

**Consent infrastructure status:** ⬜ To be implemented before live pilot

---

## Model Monitoring and Drift Log

**Record ID:** MML | **Retention:** 3 years | **Owner:** AI Technical Lead

| Log ID | Date | System | Model version | Metric checked | Baseline value | Current value | Drift (pp) | Drift threshold | Retrain triggered? | Notes | Evidence link |
|---|---|---|---|---|---|---|---|---|---|---|---|
| MML-001 | [Date] | Vess360 | [Version] | Overall accuracy | 0.48 | [TBM] | [TBM] | −5 pp | Yes/No | [Notes] | [Link] |
| MML-002 | [Date] | iVessy | [Version] | Field accuracy | [Baseline] | [TBM] | [TBM] | −5 pp | Yes/No | [Notes] | [Link] |

**Cadence:** Semi-annually; next due: [6 months from first deployment]

---

## Change Request Record

**Template ID:** CR | **Retention:** 3 years

### CR-2026-001 — iVessy Migration OpenAI → Mixtral 8x7B (self-hosted)

| Field | Value |
|---|---|
| Change ID | CR-2026-001 |
| Date initiated | 30 June 2026 |
| Requested by | Firas Kassoumeh |
| System | iVessy |
| Change description | Replace OpenAI LLM API with self-hosted Mixtral 8x7B Instruct on Hetzner EU. Also replace cloud-based ASR with self-hosted Whisper. |
| Business justification | Eliminates US data-transfer risk (iV-2); reduces operational cost; aligns with EU AI Act readiness; reduces supplier dependency |
| Risk impact | Reduces iV-2 from Medium to Low. New risks: model performance regression (mitigated by validation); hosting security (mitigated by ISMS controls) |
| AISIA update required | Yes — to be completed before deployment |
| DPIA update required | Yes — data flow changes; EU-only processing eliminates transfer concern |
| SoA update required | Review — no new Annex A controls but iV-2 treatment changes |
| Validation required | Yes — MVR-001 to be completed for Mixtral before production |
| EU AI Act re-classification | Review at deployment — classification expected to remain Limited-risk |
| Target date | Per migration roadmap (TBD) |
| CEO approval | Inge Proost — recorded in the AIMS Review & Approval Log |
| Status | 🔄 In progress — awaiting Mixtral training and validation |

---

## Risk Acceptance Record Template

*(Individual records in Section 4 §5 for all current accepted risks)*

| Field | Value |
|---|---|
| Record ID | RA-AI-[NNN] |
| Risk ID | [From Section 4] |
| Risk description | [Brief description] |
| Inherent risk | [H/M/L] |
| Residual risk | [H/M/L] |
| Justification | [Why this risk is acceptable at this residual level] |
| Conditions | [What monitoring/conditions are required] |
| Accepted by | [Name, role] |
| Date | [Date] |
| Next review | [Date or trigger] |

---

## Nonconformity and Corrective Action Log

**Record ID:** NC | **Retention:** 3 years | **Owner:** AI Technical Lead

| ID | Date raised | Source | Category | Description | Severity | Immediate containment | Root cause | Corrective action | Owner | Due date | Date closed | Verified by | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| NC-AI-001 | 30 Jun 2026 | Gap analysis | Evidence — Training | No AI-specific training records exist (Clause 7.2) | Major | N/A — not yet operational | AIMS v1.0 did not include AI-specific training programme | Implement AI training programme per ATCP-001; deliver first session; document records in Section 13 | Firas Kassoumeh | Q3 2026 | [TBM] | Inge Proost | 🔄 Open |
| NC-AI-002 | 30 Jun 2026 | Gap analysis | Audit — AIMS audit | No AIMS internal audit conducted (Clause 9.2) | Major | N/A | AIMS is newly established | Schedule and conduct first AIMS internal audit using checklist in Section 13 | Firas Kassoumeh | Q3 2026 | [TBM] | Inge Proost | 🔄 Open |
| NC-AI-003 | 30 Jun 2026 | Gap analysis | Management review | No AIMS management review conducted (Clause 9.3) | Major | N/A | AIMS is newly established | Schedule first AIMS management review; document using Section 13 template | Inge Proost | Q3 2026 | [TBM] | — | 🔄 Open |
| NC-AI-004 | 30 Jun 2026 | Gap analysis | DPIA | DPIA not finalized or signed (GDPR Art. 35; A.5.3) | Major | N/A | DPIA embedded in AIMS without sign-off | Extract as standalone document; CEO signs; file in Google Drive | Firas Kassoumeh | Q3 2026 | [TBM] | Inge Proost | 🔄 Open |
| NC-AI-005 | 30 Jun 2026 | Gap analysis | Supplier | Supplier DPAs not confirmed/evidenced (A.10.3) | Major | N/A | Evidence not collected and filed | Confirm DPA status with OpenAI, Azure, Google; file copies in Drive | Firas Kassoumeh | Q3 2026 | [TBM] | Inge Proost | 🔄 Open |
| NC-AI-006 | 30 Jun 2026 | Gap analysis | Lifecycle | No model validation records (A.6.2, E-8) | Major | Suspend live patient processing until complete | Validation not yet performed | Complete MVR-001 and MVR-002 before any live patient data processing | Firas Kassoumeh | Before pilot | [TBM] | Inge Proost | 🔄 Open |
| NC-AI-007 | 30 Jun 2026 | Gap analysis | Consent | Consent logging infrastructure not operational (A.8.2, E-9) | Major | Suspend live patient processing until complete | Not yet implemented | Implement consent logging per Section 8 §2.1; test with sample | Firas Kassoumeh | Before pilot | [TBM] | Inge Proost | 🔄 Open |

---

## AIMS Internal Audit Checklist

**Template ID:** IAC-AIMS-001 | **Version:** 1.0 | **Use for:** Annual AIMS internal audit

**Audit details:**
- Audit ID: [AUDIT-AIMS-001]
- Date: [Date]
- Auditor: [Name]
- Reviewed by: [AIMS Owner — Name]
- Scope: ISO/IEC 42001:2023 Clauses 4–10 + Annex A

| Clause | Requirement | Evidence reviewed | Finding | Severity | Action required |
|---|---|---|---|---|---|
| 4.1 | Context documented and reviewed | AIMS Section 3 §4.1 | | | |
| 4.2 | Interested parties documented | AIMS Section 3 §4.2 | | | |
| 4.3 | Scope defined; in-scope systems listed | AIMS Section 3 §4.3 | | | |
| 4.4 | AIMS established and integrated with ISMS | AIMS Section 3 §4.4 | | | |
| 5.1 | Leadership commitment evidenced | CEO approval records; resource allocation | | | |
| 5.2 | AI Policy approved and communicated | AI Policy in Section 11; distribution record | | | |
| 5.3 | Roles, responsibilities, authorities assigned | RACI in §5.3; appointment records | | | |
| 6.1.2 | Risk assessment conducted; documented | Section 4 risk register; dates; assessor | | | |
| 6.1.3 | Risk treatment documented; accepted risks signed | Section 4; Risk Acceptance Records | | | |
| 6.1.4 | AISIAs conducted; signed; dated | Section 6 AISIAs | | | |
| 6.2 | Objectives measurable; measurement data available | §6.2 table; Evidence log (Section 14) | | | |
| 6.3 | Changes planned and controlled | CR-2026-001; change procedure | | | |
| 7.1 | Resources documented | Section 7 §1 | | | |
| 7.2 | Competence criteria defined; training records exist | Section 13 training records | | | |
| 7.3 | Awareness delivered; records exist | Section 13 training records | | | |
| 7.4 | Communication plan documented | §7.4 table | | | |
| 7.5 | Document control; records retention | §7.5 tables; Google Drive | | | |
| 8.1 | Operational controls implemented; evidence | Section 8; consent logs; event logs | | | |
| 8.2 | Risk assessment re-run on change | Section 4; dates | | | |
| 8.3 | Controls applied and verified | Section 5 SoA; evidence | | | |
| 8.4 | AISIA/DPIA updated on change | Section 6; Section 9; dates | | | |
| 9.1 | Monitoring conducted; objectives measured | Section 14 evidence log; monitoring log | | | |
| 9.2 | Internal audit conducted; findings documented | Audit records in Google Drive | | | |
| 9.3 | Management review conducted; outputs recorded | Section 13 management review record | | | |
| 10.1 | Nonconformities logged; corrective actions closed | Section 13 NC log | | | |
| 10.2 | Improvement plan maintained; actions tracked | Appendix A | | | |
| A.2.2 | AI Policy exists; approved; current | Section 11; CEO approval (Review & Approval Log) | | | |
| A.3.2 | Roles assigned | §5.3 | | | |
| A.4.3 | Data register complete; provenance documented | Section 7 §2 | | | |
| A.4.6 | Training records for all roles | Section 13 | | | |
| A.5.3 | AISIAs signed and dated | Section 6 | | | |
| A.6.2 | Validation records; monitoring logs; change records | Section 13 MVR; MML; CR | | | |
| A.7.4 | Data quality checks documented | Model cards Section 10; quality records | | | |
| A.8.2 | User documentation; consent form | Section 13 user documentation | | | |
| A.8.4 | AI incident procedure; incidents logged | Section 12 PROC-IR-001; Section 13 E-11 | | | |
| A.10.3 | Supplier DPAs on file; risk assessments done | Section 7 §3; Google Drive | | | |

**Audit conclusion:** [Conforming / Minor nonconformities / Major nonconformities — detail]
**Auditor (name):** __________________ Date: __________
**AIMS Owner review:** ___________________________ Date: ___

---

## Management Review Record

**Template ID:** MRR | **Retention:** 3 years

| Field | Value |
|---|---|
| Review ID | MRR-[001] |
| Date | [Date] |
| Chair | Inge Proost (AIMS Owner / CEO) |
| Attendees | [Names] |
| AIMS version reviewed | [Version] |

**Input review:**

| Input | Summary | Status |
|---|---|---|
| Previous review actions | [List actions; complete/incomplete] | [Status] |
| External/internal context changes | [Changes since last review] | [Impact] |
| AI objectives status | [Each objective; met/not met; data] | [Status] |
| AI incidents and nonconformities | [Count; open/closed] | [Status] |
| Internal audit results | [Findings; actions] | [Status] |
| SoA control status | [Any partially implemented; changes] | [Status] |
| Risk register status | [New/changed risks] | [Status] |
| Supplier performance | [Issues; DPA renewals] | [Status] |
| Regulatory developments | [EU AI Act updates; GDPR changes] | [Impact] |
| Continual improvement plan | [Progress on Appendix A items] | [Status] |
| Resource adequacy | [Are resources sufficient] | [Decision] |

**Outputs / Decisions:**

| Decision | Owner | Deadline |
|---|---|---|
| AIMS suitability/adequacy/effectiveness: [conclusion] | — | — |
| [Improvement action 1] | [Owner] | [Date] |
| [Resource decision] | AIMS Owner | [Date] |
| [Policy/objective update] | [Owner] | [Date] |

**Chair (name):** Inge Proost (CEO) Date: __________

---

## User Information Sheet Template (iVessy — A.8.2)

**To be provided to patients/clients before iVessy sessions:**

---

**Information about your AI-assisted care session**

*[Healthcare organization name]* uses an AI assistant called iVessy to help record your care information.

**What does the AI do?**
The AI listens to what you say and converts your words into a structured record for your care team. It does not make any decisions about your care — your care professional does that.

**What happens to my voice?**
Your voice is processed in real time and is **not saved or stored**. Only the structured information you confirm is kept.

**Emotion analysis (if enabled):**
If emotion analysis is enabled, the AI may analyze the tone of your voice and show your care professional a general indication (such as "calm" or "concerned"). This is approximate and for context only — it does not affect your care.

**Your rights:**
- You can review and correct all information before it is saved
- You can stop the session at any time
- You can withdraw your consent at any time
- You have the right to access, correct, or delete your data under GDPR

**Who can I contact?**
For questions about your data: [Healthcare organization privacy contact / DPO]
For questions about the AI: [Rate.nl support email]

**Your consent:**
By participating in this session, you confirm that you have read this information and consent to the AI-assisted recording.

☐ I agree / □ I do not agree (session proceeds without AI-assisted recording)

*Confirmation recorded:* __________________ Date: __________

---

## AI Ethics Review Record

**Record ID:** ETH-[NNN] | **Owner:** AI Technical Lead | **When:** lifecycle Phase 5 and on significant change.

Given the healthcare context and vulnerable users, each AI system undergoes a documented ethics review before deployment. ISO 42001 does not mandate an ethics board; this lightweight review meets the expectation and can draw on knowledge partners (Avans — Responsible AI; Erasmus MC — clinical).

| Ethics checkpoint | Question | Assessment | Action |
|---|---|---|---|
| Beneficence | Clear benefit to patients/care? | | |
| Non-maleficence | Could it cause harm (wrong data, distress, exclusion)? Mitigated? | | |
| Autonomy & dignity | Can the user understand, consent, review, edit, decline? | | |
| Fairness | Are vulnerable/minority groups fairly served? Bias monitored? | | |
| Transparency | AI use (and emotion analysis) clearly disclosed? | | |
| Human oversight | Human always in control of any decision? | | |
| Proportionality | Data use proportionate to benefit? | | |
| External input | Knowledge-partner/ethics input sought where warranted? | | |

| Field | Value |
|---|---|
| System | [iVessy / Vess360 / Vera] |
| Reviewed by | Firas Kassoumeh (AI Technical Lead) |
| External input | [Avans / Erasmus MC / none] |
| Date | [Date] |
| Outcome | ☐ Proceed ☐ Proceed with conditions ☐ Do not proceed |
| Conditions / notes | |

**Approval:** Recorded in the AIMS Review & Approval Log.

---

## AI System Decommission Record

**Record ID:** DEC-[NNN] | **Owner:** AI Technical Lead | **Lifecycle Phase 10 (Retirement).**

| Field | Value |
|---|---|
| System / model | [Name + version] |
| Reason | [Replacement / obsolescence / risk / end of use] |
| Decommission date | [Date] |
| Data handling | [Training/inference data deleted or archived per retention schedule] |
| Model artefact handling | [Weights archived/deleted; keys revoked] |
| Dependent systems notified | [Yes/No — which] |
| Model card archived | [Link] |
| Supplier services terminated | [OpenAI/Azure/Google — contracts/keys closed as applicable] |
| Evidence log updated | [Yes — E-ref] |
| Residual risk after decommission | [Assessment] |
| Approved by | Recorded in the AIMS Review & Approval Log |

**Data-deletion confirmation:** ☐ Deleted per schedule ☐ Archived (justification) — verified by [name], [date].

---

## Supplier AI Risk Assessment Template

**Template ID:** SAR | **Use per AI supplier**

| Field | Value |
|---|---|
| Assessment ID | SAR-[NNN] |
| Supplier | [Name] |
| Service | [What AI/data service] |
| Data processed | [Type and classification] |
| Assessed by | Firas Kassoumeh |
| Date | [Date] |
| Next review | [Annual] |

| Assessment area | Finding | Risk | Control / Action |
|---|---|---|---|
| DPA / SCC in place | [Yes/No/Pending] | [H/M/L] | [Action] |
| EU data residency | [Confirmed/Partial/No] | [H/M/L] | [Action] |
| No model training on our data | [Confirmed in contract] | [H/M/L] | [Contract clause ref] |
| Security certification (ISO 27001 / SOC 2) | [Certificate details] | [H/M/L] | [Link] |
| Incident notification clause in DPA | [Yes/No] | [H/M/L] | [Action] |
| Sub-processor disclosure | [Disclosed/Not disclosed] | [H/M/L] | [Action] |
| Transfer risk (CLOUD Act etc.) | [Assessment] | [H/M/L] | [TIA ref] |
| Audit rights | [Yes/No] | [H/M/L] | [Contract clause] |
| Overall supplier risk | [H/M/L] | | |

**Approval to use supplier:** ☐ Approved ☐ Approved with conditions ☐ Not approved
**Approved by:** ___________________________ Date: ___

### SAR-001 — OpenAI (iVessy LLM, transitional) — preliminary
| Assessment area | Preliminary finding (public info — confirm) | Risk | Action |
|---|---|---|---|
| DPA / SCC | OpenAI provides a DPA incorporating EU SCCs — **obtain signed copy** | H | Sign & file DPA |
| EU data residency | US processing; EU data-residency / Zero-Data-Retention options on some tiers — confirm | H | Confirm option; minimise data; migrate to EU/self-hosted |
| No training on our data | API/Business terms: data not used to train models by default — confirm | M | Verify clause |
| Security certification | SOC 2 Type 2 reported; CSA STAR — **obtain current report** | L | File link |
| Incident notification | Confirm breach-notification clause in DPA | M | Verify |
| Sub-processor disclosure | Confirm sub-processor list | M | Obtain list |
| Transfer risk (CLOUD Act) | US provider — see TIA (DPIA §7) | M | SCTs; migration |
| Overall | Medium (transitional) — accepted RA-AI-001 | M | |

### SAR-002 — Microsoft Azure (Vess360 STT) — preliminary
| Assessment area | Preliminary finding (public info — confirm) | Risk | Action |
|---|---|---|---|
| DPA / SCC | Microsoft Products & Services DPA incl. EU SCCs — **obtain/confirm signed** | M | File DPA |
| EU data residency | EU regions + EU Data Boundary — confirm configuration | L | Confirm region config |
| No training on our data | Azure AI: customer data not used to train foundation models — confirm | L | Verify |
| Security certification | ISO/IEC 27001, 27017, 27018; SOC 1/2/3 — **obtain current attestations** | L | File links |
| Incident notification | Confirm DPA breach-notification terms | L | Verify |
| Sub-processor disclosure | Microsoft sub-processor list published — confirm | L | File link |
| Transfer risk | EU region, US-HQ — see TIA (DPIA §7) | M | SCCs |
| Overall | Medium — accepted RA-AI-006 | M | |

### SAR-003 — Google Cloud (Vess360 translate/run/training) — preliminary
| Assessment area | Preliminary finding (public info — confirm) | Risk | Action |
|---|---|---|---|
| DPA / SCC | Google Cloud DPA incl. EU SCCs — **obtain/confirm signed** | M | File DPA |
| EU data residency | EU regions + data-residency controls — confirm | L | Confirm config |
| No training on our data | Google Cloud: customer data not used to train models — confirm | L | Verify |
| Security certification | ISO/IEC 27001, 27017, 27018; SOC 1/2/3 — **obtain current reports** | L | File links |
| Incident notification | Confirm DPA breach terms | L | Verify |
| Sub-processor disclosure | Google sub-processor list published — confirm | L | File link |
| Transfer risk | EU region, US-HQ — see TIA (DPIA §7) | M | SCCs |
| Overall | Medium — accepted RA-AI-006 | M | |

**Completion status:** SAR-001/002/003 drafted above from public due diligence; **signed DPAs + current attestations to be obtained and filed** (NC-AI-005), then finalise risk ratings and record CEO approval. Due Q3 2026.

---

---

# 14. Integrated Evidence Log

**Purpose:** Central register of all evidence proving the AIMS operates as documented. This is the primary file an auditor requests.
**Owner:** Firas Kassoumeh (AI Technical Lead) — collection | Inge Proost (AIMS Owner) — review
**Status legend:** ✅ Collected | 🔄 In progress | ⬜ Planned | ❌ Overdue
**Updated:** 30 June 2026

## Evidence Index

| Ref | AIMS item | ISO 42001 clause | Evidence required | Location | Target date | Status |
|---|---|---|---|---|---|---|
| E-1 | Objective: iVessy intake-time reduction | 9.1, 6.2 | Time-motion / EPD timestamp comparison (≥ 20% reduction vs. baseline) | Google Drive / EPD export | WP2 2026 | ⬜ |
| E-2 | Objective: iVessy field quality | 9.1, A.6.2 | Validation set results (field accuracy ≥ 90%; clarification rate) | GitHub / Google Drive | Before pilot go-live | ⬜ |
| E-3 | Objective: Vess360 emotion reliability | 9.1, A.6.2 | Model evaluation report (overall accuracy; per-emotion F1; confidence distribution) | GitHub / Google Drive | Q3 2026 | 🔄 |
| E-4 | Objective: Fairness | 9.1, A.5.4 | Subgroup performance analysis (iVessy: language/accent/assistance; Vess360: corpus-level) | Google Drive | Q3 2026 | ⬜ |
| E-5 | Objective: Model monitoring | 9.1, A.6.2 | Semi-annual drift-check log (MML in Section 13) | This document Section 13 | 6 months post-launch | ⬜ |
| E-6 | DPIA signed (standalone) | A.5.3, GDPR | Signed standalone DPIA document (DPIA-iVessy-Vess360-v2.0-[date].pdf) | Google Drive | Q3 2026 | 🔄 |
| E-7 | Model cards (versioned, approved) | A.6.2, A.6.1 | Model cards MC-001, MC-002, MC-003 — approved, dated, version-controlled | This document Section 10 + GitHub | 30 Jun 2026 | 🔄 (recorded in Review & Approval Log) |
| E-8 | Validation-before-deployment records | A.6.2 | MVR-001 (iVessy LLM) and MVR-002 (Vess360) — signed | Google Drive + Section 13 | Before pilot go-live | ⬜ |
| E-9 | Consent and transparency logs | A.8.2, A.9.2 | Sample consent log exports; consent infrastructure test results | App logs / Google Drive | Before pilot go-live | ⬜ |
| E-10 | Supplier DPAs / SCCs | A.10.3 | Signed DPAs with OpenAI, Azure, Google — on file | Google Drive | Q3 2026 | 🔄 |
| E-11 | AI incident records | A.8.4, 10.1 | AI incident log (Section 13 NC log) — operational with at least one test/drill entry | This document Section 13 | Q3 2026 | 🔄 (template in place; operational pending) |
| E-12 | Internal audit + management review | 9.2, 9.3 | Audit report (IAC-AIMS-001 completed); Management Review Record (MRR-001 completed) | Google Drive | Q3 2026 | ⬜ |
| E-13 | Training and awareness records | 7.2, 7.3 | Training register (Section 13 TR-AIMS) — all roles; first AI-specific training session completed | Google Drive | Q3 2026 | ⬜ |
| E-14 | Risk Acceptance Records | 6.1.3 | All 7 CEO-approved Risk Acceptance Records (Section 4 §5) | This document Section 4 | 30 Jun 2026 | 🔄 (recorded in Review & Approval Log) |
| E-15 | AI Policy communication | 5.2, 7.3 | Evidence AI Policy was communicated to all staff (email/meeting record) | Google Drive | Q3 2026 | ⬜ |
| E-16 | AISIA approvals | A.5.3 | Approved AISIA-001 and AISIA-002 (Section 6) | This document Section 6 | Q3 2026 | 🔄 (recorded in Review & Approval Log) |
| E-17 | CEO AIMS approval | 5.1 | CEO approval recorded in the AIMS Review & Approval Log | This document | 30 Jun 2026 | 🔄 (recorded in Review & Approval Log) |
| E-18 | Supplier AI risk assessments | A.10.3 | SAR-001, SAR-002, SAR-003 completed (Section 13 templates) | Google Drive | Q3 2026 | ⬜ |
| E-19 | User information sheet / consent form | A.8.2 | Approved user-facing information sheet (Section 13 template) | This document + Google Drive | Before pilot go-live | ⬜ |
| E-20 | Data quality records (DS-004) | A.7.4 | Inter-rater agreement results (Krippendorff's α); quality check report | Google Drive / GitHub | Q3 2026 | ⬜ |

## Evidence Collection Progress

| Status | Count | % |
|---|---|---|
| ✅ Collected | 0 | 0% |
| 🔄 In progress / partially done | 7 | 35% |
| ⬜ Planned | 13 | 65% |
| **Total** | **20** | |

**Target before external audit:** ≥ 17 of 20 items ✅ Collected (85%)

---

---

# 15. EU AI Act Compliance Mapping

**Basis:** Regulation (EU) 2024/1689 (EU AI Act) — phased application 2024–2027
**Last reviewed:** 30 June 2026 | **Owner:** Firas Kassoumeh

## Article 13 & Article 50 Transparency Checklist

Concrete transparency obligations mapped to implementation; reviewed before each deployment.

**Art. 13 — information to users (iVessy)**
| Requirement | Provided? | Where |
|---|---|---|
| That the user interacts with an AI system | ✅ | Pre-session disclosure (Section 8 §2.1) |
| Identity / purpose of the system | ✅ | Pre-session disclosure |
| Data processed (speech, content, emotion) | ✅ | Disclosure + consent |
| Human oversight (professional reviews output) | ✅ | Disclosure; process design |
| Right to review / edit / withdraw | ✅ | Disclosure; UX |
| Contact for questions | ✅ | Disclosure (care professional / privacy contact) |
| Known limitations / accuracy caveat | 🔄 | Add accuracy caveat to the user information sheet |

**Art. 50 — emotion-recognition disclosure (Vess360)**
| Requirement | Provided? | Where |
|---|---|---|
| Explicit disclosure that emotion recognition is used | ✅ | Pre-session disclosure |
| Consent before emotion analysis | ✅ | Logged consent |
| Emotion is supportive-only, not decisional | ✅ | Disclosure + policy |
| No workplace / education use (Art. 5) | ✅ | Contractual restriction; SoA |
| Data-subject rights honoured | ✅ | GDPR rights in disclosure |

**Emotion-recognition disclosure wording (Vess360):** *"During this session, an AI tool may analyse the tone of your voice to give your care professional an indication of your emotional state. This is for supportive context only and does not make any decision about your care. You can decline this at any time."*

## Public AI Transparency Notice & Responsible Disclosure

**Public notice (to publish on Rate.nl):** *"Rate develops AI-assisted tools (iVessy, Vess360) that help care professionals capture care information through natural conversation and provide supportive emotional context. These tools support — and never replace — professional judgment; no automated decisions are made about care. Voice is processed in the EU and audio is not stored by iVessy. We operate an AI Management System aligned with ISO/IEC 42001 and comply with the GDPR and the EU AI Act."*

**Responsible disclosure channel:** Anyone can report a concern or adverse impact of our AI systems via the Rate.nl contact form / privacy contact, routed to the AI Technical Lead and logged in the AI incident log (E-11), acknowledged within a defined timeframe.

## 1. Risk Classification Summary

| System | Provisional classification | Basis | Date of classification | Review trigger |
|---|---|---|---|---|
| iVessy | **Limited-risk** + transparency obligations (Art. 13) | No autonomous decision-making; not in Annex III; human-in-the-loop; administrative purpose only | 30 Jun 2026 | Before Mixtral migration; before scale-up beyond pilot |
| Vess360 | **Limited-risk** + emotion recognition transparency obligations (Art. 50) | Emotion recognition in medical context with consent and professional oversight; not prohibited (not workplace/education); not high-risk autonomous decision | 30 Jun 2026 | Before any new deployment context |
| Vera | **TBD** — to be classified at operational launch per AISIA-003 | — | At launch | — |

**Classification rationale — iVessy (not high-risk):**
- Not listed in Annex III (biometric identification, critical infrastructure, education, employment, access to essential services, law enforcement, migration, justice, democracy)
- Does not make autonomous decisions affecting individuals' access to services or their rights
- Human-in-the-loop is a hard architectural constraint, not a policy choice
- Output is administrative data collection, not clinical assessment

**Prohibited-use confirmation (Art. 5):**
The following prohibited AI practices are confirmed as not present in any in-scope system:
- ☑ No real-time remote biometric identification in publicly accessible spaces
- ☑ No emotion recognition in workplace or education settings
- ☑ No social scoring systems
- ☑ No AI exploiting vulnerabilities of individuals for manipulation
- ☑ No subliminal or deceptive techniques
- ☑ No predictive policing based on profiling

## 2. Article-by-Article Compliance Mapping

### Article 9 — Risk Management System (for high-risk AI)
*Applicability: Not directly applicable (iVessy/Vess360 are Limited-risk). However, we implement equivalent controls voluntarily as good practice.*

| Requirement | AIMS control | Reference | Status |
|---|---|---|---|
| Risk management system | AI risk assessment procedure | Section 12 PROC-RA-001; Section 4 | ✅ |
| Residual risk minimization | Risk treatment and residual risk tracking | Section 4 | ✅ |
| Testing for accuracy, robustness, cybersecurity | Model validation; security testing (ISMS) | Section 13 MVR; ISMS | 🔄 |

### Article 10 — Data Governance (for high-risk AI)
*Applicability: Voluntary good practice*

| Requirement | AIMS control | Reference | Status |
|---|---|---|---|
| Training data quality | Multi-rater labelling; quality checks | Section 10 MC-003; Section 13 E-20 | 🔄 |
| Data provenance | Data register with full provenance | Section 7 §2 | ✅ |
| Data minimization | No audio storage; structured output only | Section 8 §2.2; Section 9 | ✅ |
| Bias monitoring | Fairness analysis | Section 8 §3.3; E-4 | ⬜ |

### Article 13 — Transparency and Provision of Information to Deployers
*Applicability: Applies to Limited-risk systems as transparency obligations*

| Requirement | AIMS control | Reference | Status |
|---|---|---|---|
| Identify system as AI to users | Pre-session disclosure | Section 8 §2.1; E-9 | 🔄 (pending consent log implementation) |
| Inform of capabilities and limitations | User information sheet | Section 13 user information sheet; model cards | 🔄 |
| Inform of intended purpose | Scope (§4.3); model cards; user sheet | Section 6 AISIA; Section 10 | ✅ |
| Inform of human oversight | Professional confirmation loop; user review | Section 8 §2.2 | ✅ |
| Inform of accuracy and limitations | Model cards; user sheet | Section 10; Section 13 | 🔄 |
| Provide deployer with technical documentation | AIMS; model cards; AISIA; DPIA | This document | ✅ |

**Action:** Complete the user information sheet (Section 13 template) and implement in iVessy UI before pilot go-live (E-19).

### Article 14 — Human Oversight
*Applicability: Good practice; partially required for Limited-risk*

| Requirement | AIMS control | Reference | Status |
|---|---|---|---|
| Human oversight measures in design | Hard requirement for human confirmation before data commit | Section 8 §2.2; AISIA-001 | ✅ |
| Ability to interpret AI output | Professional training; "uncertain" label on Vess360 | Section 8 §3.1; model card | ✅ |
| Ability to override or stop | User can stop session; professional can reject output | Section 8 §2.1 | ✅ |
| Ability to interrupt | Session can be abandoned at any time | Section 8 §2.1; user sheet | ✅ |

### Article 50 — Transparency Obligations for Certain AI Systems
*Applicability: **DIRECTLY APPLICABLE** to Vess360 (emotion recognition)*

| Requirement | AIMS control | Reference | Status |
|---|---|---|---|
| Inform persons they are subject to emotion recognition | Pre-session disclosure; explicit consent | Section 8 §3.2; AI Policy §5.2 Principle 3 | 🔄 (consent log pending) |
| Obtain explicit consent for emotion recognition | Logged explicit consent before each session | Section 8 §3.2; CTL in Section 13 | 🔄 (implementation pending) |
| Right to refuse emotion analysis | Option to decline emotion analysis; session continues without it | Section 8 §3.2 | ✅ (by design) |
| No use in prohibited contexts (workplace, education) | Contractual and design prohibition | AI Policy §5.2; ASMP-001; AISIA-002 | ✅ |

**Consent disclosure wording for Art. 50:**
> *"This session uses voice-emotion analysis. The AI will analyze the tone of your voice and may show your care professional an indication of your emotional state (e.g., calm, concerned). This is approximate — accuracy is limited — and is for context only. Your care professional uses their professional judgment. You can decline this analysis and the session will continue normally. By saying 'yes' or clicking Agree, you consent to voice-emotion analysis."*

This wording must be presented **before** emotion analysis begins, in the user's language. Consent is logged per session (E-9).

### Article 53 — General-Purpose AI Model (GPAI) Obligations
*Applicability: OpenAI and Mistral/Mixtral may be GPAI models; obligations are on the GPAI provider, not on us as the deployer. We use GPAI models; we are not their provider.*

| Consideration | AIMS position |
|---|---|
| GPAI provider obligations | OpenAI/Mistral are responsible for their GPAI model compliance. We receive the benefit of their compliance. |
| Our deployer obligations | Ensure intended use complies with our scope; review GPAI provider's GPAI terms; document in supplier register |
| Self-hosted Mixtral | When self-hosted, we take on additional responsibility as the deployer — AIMS controls apply |

### Regulation Timeline / Phased Application

| Date | Provision | Applicability to us |
|---|---|---|
| 2 Feb 2025 | Prohibited AI practices (Art. 5) in force | ✅ Confirmed no prohibited practices |
| 2 Aug 2025 | GPAI model obligations (Art. 53–55) in force | OpenAI/Mistral compliance; our supplier DPA review |
| 2 Aug 2026 | Transparency obligations (Art. 50) fully in force | ✅ Consent/disclosure controls required before this date |
| 2 Aug 2026 | Governance and market surveillance (Art. 56–94) | Monitor regulatory guidance |
| 2 Aug 2027 | High-risk AI obligations (Annex III) fully in force | Classification review at this point |

**Key deadline:** Vess360 Art. 50 consent and disclosure controls must be **fully operational by 2 August 2026**. Current status: 🔄 In progress — consent log implementation required (E-9).

## 3. EU AI Act Compliance Action Plan

| Action | Responsible | Deadline | Priority |
|---|---|---|---|
| Implement consent logging for Art. 50 (E-9) | AI Technical Lead | Before 2 Aug 2026 | CRITICAL |
| Complete user information sheet (E-19) and implement in iVessy UI | AI Technical Lead | Before pilot go-live | HIGH |
| Complete Art. 13 transparency checklist for iVessy | AI Technical Lead | Q3 2026 | HIGH |
| Review OpenAI and Mixtral GPAI compliance documentation | AI Technical Lead | Q3 2026 | MEDIUM |
| Conduct formal EU AI Act classification decision (documented) for all systems | AI Technical Lead | Q3 2026 | MEDIUM |
| Monitor EU AI Act secondary legislation and guidance | AI Technical Lead | Ongoing | MEDIUM |
| Review classification at iVessy Mixtral deployment | AI Technical Lead | At deployment | MEDIUM |
| Review classification at Vera launch | AI Technical Lead | At Vera launch | MEDIUM |

---

---

# Appendix A — Continual Improvement Plan

**Last updated:** 30 June 2026 | **Owner:** AI Technical Lead | **Review:** At each management review

| # | Action | Owner | Target date | Priority | Status | Progress notes |
|---|---|---|---|---|---|---|
| 1 | Deliver first AI-specific training session for all roles; document records in Section 13 (TR-AIMS); define competence criteria | AI Technical Lead | Q3 2026 | CRITICAL | 🔄 Open | Training content being prepared |
| 2 | Conduct first AIMS internal audit (IAC-AIMS-001); document findings; raise corrective actions | AI Technical Lead | Q3 2026 | CRITICAL | 🔄 Open | Checklist in Section 13 |
| 3 | Conduct first AIMS management review (MRR-001); document outputs; AIMS Owner to sign | AIMS Owner | Q3 2026 | CRITICAL | 🔄 Open | Template in Section 13 |
| 4 | Finalize and sign DPIA as standalone document; file in Google Drive | AI Technical Lead + CEO | Q3 2026 | CRITICAL | 🔄 Open | Draft in Section 9 |
| 5 | Confirm and file supplier DPAs (OpenAI, Azure, Google); complete supplier risk assessments (SAR-001, 002, 003) | AI Technical Lead | Q3 2026 | CRITICAL | 🔄 Open | Templates in Section 13 |
| 6 | Implement consent logging infrastructure; test; document sample evidence (E-9) | AI Technical Lead | Before pilot go-live / before 2 Aug 2026 | CRITICAL | 🔄 Open | Required for Art. 50 |
| 7 | Complete model validation records (MVR-001, MVR-002) before any live patient data processing | AI Technical Lead | Before pilot go-live | CRITICAL | 🔄 Open | Templates in Section 13 |
| 8 | Record CEO approval for all AISIA (Section 6) and Risk Acceptance Records (Section 4 §5) in the AIMS Review & Approval Log | AIMS Owner | Q3 2026 | HIGH | 🔄 Open | Documents ready in this AIMS |
| 9 | Complete first Vess360 model evaluation (E-3); populate per-emotion F1 in model card | AI Technical Lead | Q3 2026 | HIGH | 🔄 Open | |
| 10 | Complete data quality checks for DS-004 (E-20); document inter-rater agreement | AI Technical Lead | Q3 2026 | HIGH | 🔄 Open | |
| 11 | Conduct Vess360 fairness analysis — corpus-level subgroup analysis (E-4) | AI Technical Lead | Q3 2026 | HIGH | 🔄 Open | |
| 12 | Complete AI Use Policy communication to all staff (E-15) | AI Technical Lead | Q3 2026 | HIGH | 🔄 Open | Policy in Section 11 |
| 13 | Publish AI transparency notice and responsible disclosure channel (E-18, A.8.3) | AI Technical Lead | Q3 2026 | MEDIUM | 🔄 Drafted (Section 15) — publish on Rate.nl | |
| 14 | Create data preprocessing procedure for Vess360 training (A.7.6) | AI Technical Lead | Q3 2026 | MEDIUM | ✅ Done (PROC-DP-001, Section 12) | |
| 15 | Complete iVessy pilot study registration and E-1/E-2 measurement plan (WP2) | AI Technical Lead | Q3–Q4 2026 | MEDIUM | ⬜ Planned | |
| 16 | Execute iVessy migration from OpenAI → EU → self-hosted Mixtral (CR-2026-001) | AI Technical Lead | Per roadmap | MEDIUM | 🔄 In progress | Change request in Section 13 |
| 17 | Improve Vess360 emotion accuracy above ~0.48 Dutch baseline | AI Technical Lead | Ongoing — semi-annual review | MEDIUM | 🔄 Ongoing | |
| 18 | Conduct iVessy fairness subgroup analysis on WP2 pilot data | AI Technical Lead | Post-WP2 pilot | MEDIUM | ⬜ Planned | |
| 19 | Conduct first semi-annual model drift check (E-5) | AI Technical Lead | 6 months post-deployment | MEDIUM | ⬜ Planned | |
| 20 | Review Vess360 confidence threshold (0.70) after first pilot results available | AI Technical Lead | Post-WP2 pilot | MEDIUM | ⬜ Planned | |
| 21 | Onboard Vera into the AIMS at operational launch (AISIA-003; model card; DPIA update; risk register) | AI Technical Lead | At Vera launch | MEDIUM | ⬜ Planned | Template in AISIA-003 |
| 22 | Document succession plan for AI Technical Lead key-person risk (Org-1) | AI Technical Lead + AIMS Owner | Q4 2026 | MEDIUM | ⬜ Planned | |
| 23 | Add Vess B.V. to the certified ISO 27001 / AIMS boundary | AIMS Owner | At AIMS certification | LOW | ⬜ Planned | |
| 24 | Complete NEN 7510:2022 certification process (external audit) | AIMS Owner | 2026 | LOW | ⬜ Planned | |
| 25 | Submit AIMS for ISO 42001:2023 certification (DNV or equivalent) | AIMS Owner | 2027 | LOW | ⬜ Planned | |

---

# Appendix B — Cross-Reference: AIMS ↔ ISMS

| AIMS element | ISMS equivalent | Integration approach |
|---|---|---|
| AI risk assessment (§6.1.2) | ISMS risk assessment (readme.md §6) | Same methodology extended; shared risk scales; separate AI risk register |
| AI SoA (Section 5) | ISMS SoA (readme.md §3) | Separate documents; both reviewed at management review |
| AI incident management (Section 12 PROC-IR-001) | ISMS Incident Response (readme.md §9; Logs.md §2) | AI incidents logged in ISMS incident log with AI category tag; AI-specific procedure extends ISMS process |
| AI supplier management (Section 11 ASMP-001; Section 7 §3) | ISMS supplier management (readme.md) | Shared supplier register where overlapping; AI-specific requirements added |
| AI training (Section 13 TR-AIMS; Section 11 ATCP-001) | ISMS training (Logs.md §1) | Combined annual awareness session with AI-specific module; separate AI training register |
| AI management review (Section 12 PROC-MR-001; Section 13 MRR) | ISMS management review (Logs.md §13) | Separate AIMS management review; outputs reported to ISMS review |
| AI internal audit (Section 12 PROC-AUDIT-001; Section 13 IAC) | ISMS internal audit (readme.md) | AI audit added to ISMS audit programme; same auditor; separate checklist |
| AI change management (Section 12 PROC-CM-001; Section 13 CR) | ISMS change control (Logs.md §6) | AI change requests use ISMS change log with AI-specific fields; AI Technical Lead leads AI changes |
| AI document control (§7.5) | ISMS document control | AIMS stored in same repository (rate-nl/ISO); same retention schedule |
| AI asset register (Section 7 §1) | ISMS asset inventory (Logs.md §5) | AI models and compute resources listed in ISMS asset inventory AND AI resource register; AI Technical Lead owns AI assets |
| AI data protection (Section 9 DPIA) | ISMS privacy/data protection (readme.md §4) | DPIA is AIMS-specific; references ISMS privacy policy; shared AP breach notification process |

---

# Appendix C — Document History

| Version | Date | Author | Change summary | Approved by |
|---|---|---|---|---|
| 0.1 | 2026 | Firas Kassoumeh | Initial AIMS skeleton | — |
| 1.0 | 18 Jun 2026 | Firas Kassoumeh | First complete AIMS: Clauses 4–10, SoA, risk register, AISIAs, registers, lifecycle, DPIA, model cards, continual-improvement plan | Inge Proost |
| 2.0 | 30 Jun 2026 | Firas Kassoumeh | Gap-analysis remediation: added standalone procedures (Section 12); complete record templates (Section 13); integrated evidence log (Section 14); EU AI Act compliance mapping (Section 15); AI policies (Section 11); risk acceptance records (Section 4 §5); nonconformity log with open NCs from gap analysis; updated SoA with remediation status; AISIA approvals recorded; model card approvals recorded; management review procedure; internal audit checklist; user information sheet template; supplier risk assessment template; AI competence criteria and training register; consent log template; monitoring log template; change request CR-2026-001; updated continual improvement plan (25 items); cross-reference appendix | Inge Proost |
| 3.0 | 6 Jul 2026 | Firas Kassoumeh | Format & governance revision: removed all inline signature blocks (single CEO sign-off via the AIMS Review & Approval Log + Manager Approvals folder); added the AIMS Governance Records section (approval log, audit calendar, evidence links); reformatted to ISMS-style numbered sections (1–15 + Appendices) with a linked Table of Contents and an Introduction (purpose, scope, definitions). No change to policy, risk, AISIA, DPIA or control content. | Inge Proost (approval pending) |

---

*End of AIMS Complete Implementation — v3.0 — 6 July 2026*
*DineRate B.V. / Rate.nl — CONFIDENTIAL*
