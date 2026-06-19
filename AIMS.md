# AI Management System (AIMS) Manual

**Standard:** ISO/IEC 42001:2023 (with EU AI Act readiness)
**Organization:** DineRate B.V. group (operating identity: Rate / Rate.nl)
**Status:** v1.0 — issued
**AIMS Owner (accountable):** Inge Proost (CEO / Managing Director)
**AI Technical Lead (responsible):** Firas Kassoumeh
**Approved by:** Inge Proost (CEO / AIMS Owner) — signed on issue
**Date of issue:** 18 June 2026
**Integration:** Extends the certified ISO/IEC 27001:2022 / NEN 7510:2022 ISMS

> This is the complete, consolidated AI Management System, mirroring the single-file style of the ISMS manual. It integrates with and extends the certified ISMS. Forward-looking actions are listed with owners and targets in the continual-improvement plan (Appendix A) — this is normal for a management system and not a gap.

---

## Document control

| Field | Value |
|---|---|
| Document | AI Management System Manual (AIMS.md) |
| Version | 1.0 |
| Date of issue | 18 June 2026 |
| Owner | Inge Proost (AIMS Owner) |
| Author | Firas Kassoumeh (AI Technical Lead) |
| Approval | Approved by the CEO on issue |
| Review cycle | Annual, or on significant change |
| Related | ISMS manual (readme.md), ISMS Logs (Logs.md), ISO 42001 implementation plan |
| Repository | rate-nl/ISO (alongside the ISMS) |

---

# PART I — MANAGEMENT SYSTEM (ISO 42001 Clauses 4–10)

## 4. Context of the organization

### 4.1 Organization and its context

The group operates under the trade identity **Rate / Rate.nl** and has 12+ years' experience in care-quality measurement, client/patient experience and digital feedback instruments. It develops and operates AI systems for the healthcare sector. UBO: **Inge Proost**.

| Entity | KvK | BTW | Role | AIMS status |
|---|---|---|---|---|
| **DineRate B.V.** | 55058590 | NL851549718B01 | Holding / development; owns the IP; **holder of the certified ISO 27001 management system** | **AIMS holder** (parent) |
| **CareRate B.V.** | 61419214 | NL854333721B01 | Operating company under DineRate; develops & operates iVessy and the CareRate / Rate.nl platform | **In scope** — AI provider/developer + deployer |
| **Vess B.V.** | 86159097 | 863880253 | Develops & licenses the Vess360 voice-emotion model; holds the MSP-Podcast data licence | **In scope** — AI provider/developer |
| Proost Works B.V. | — | — | Administrative/financial lead (subsidy penvoerder) | Interested party — not operational for AI |

**Management-system baseline:**
- **ISO/IEC 27001:2022 — certified.** Holder **DineRate B.V.** (CareRate B.V. included as a site); Certification Body **DNV** (UKAS-accredited, registration 0013); certificate **213311-2017-AIS-NLD-UKAS**; initial certification 17 Nov 2017; valid **18 Nov 2023 – 17 Nov 2026**; scope = development, maintenance, hosting and support of SaaS applications for healthcare, education and other organizations, per **SoA v2.0 (27 June 2025)**. Registered site: Stationsplein 45, 3013/3014 AK Rotterdam.
- **NEN 7510:2022 — certification in progress**; external audit planned alongside the AIMS / AI-Act assessment (Appendix A).
- **Vess B.V.** is brought into the AIMS now and will be added to the certified boundary when the AIMS is submitted for certification (Appendix A).

**Internal/external issues relevant to AI:** sensitive health data and vulnerable users; small-organization resourcing; reliance on third-party AI (OpenAI; Azure/Google for Vess360); the EU AI Act and GDPR; healthcare-sector trust and adoption; the documented migration toward EU/self-hosted models for iVessy.

### 4.2 Interested parties and their requirements

| Interested party | Key AI-related requirement |
|---|---|
| Clients / patients (incl. vulnerable groups) | Safety, dignity, transparency, consent, fairness, privacy, ability to review/correct |
| Informal caregivers | Reduced burden; clarity; not repeating information |
| Healthcare professionals / organizations | Reliable, explainable support; human stays in control; data quality; integration |
| Regulators / supervisors (AP, market surveillance) | GDPR, EU AI Act, Wkkgz, Wabvpz compliance; auditability |
| Knowledge partners (Avans, Erasmus MC) | Responsible AI, ethical validation, evidence |
| Suppliers (AI/model/cloud) | Clear data-use limits, security, incident responsibilities |
| Owners / management | Lawful, trustworthy, commercially viable AI |

### 4.3 Scope of the AIMS

> The AIMS covers the **development, provision and operation of AI systems for voice-driven collection and structuring of care information, and for voice-based emotion recognition** — specifically **iVessy** and **Vess360** (and **Vera** upon operational launch) — within **DineRate B.V.**, operated by **CareRate B.V.** (KvK 61419214) and **Vess B.V.** (KvK 86159097), IP held by **DineRate B.V.** (KvK 55058590). It includes all supporting people, processes, models, data and infrastructure; the organization's roles as **AI developer/provider** and **AI deployer**; current third-party AI use; and the planned migration of iVessy to EU/self-hosted models.

**AI systems in scope**

| System | Description | Org role | Current AI stack & hosting | Stage |
|---|---|---|---|---|
| **iVessy** | Voice-driven assistant replacing care forms with multilingual dialogue; outputs structured FHIR/HL7 data. Not a decision system; human-in-the-loop; no diagnosis/triage. | Provider/developer + deployer | LLM: **OpenAI (US), current** → planned self-hosted **Mixtral 8x7B** + local **Whisper** (EU → fully local). Emotion via Vess360. | Pilot (TRL 4→5/6) |
| **Vess360** | In-house voice-emotion model (6 Ekman emotions; wav2vec2-based). Most AI-Act-sensitive component. | Provider/developer | **Azure STT + Google Translate + Google Cloud Run + Vertex AI**, **EU regions**; no migration planned. | Production / API |
| **Vera** | Low-threshold patient app to record and listen back to spoken information, with planned voice-to-text and (later) Vess360 emotion support; distributed via app stores. Intended architecture aligns with the group standard (EU/self-hosted ASR + Vess360); finalized at launch. | Provider + deployer | To be finalized at launch (group standard) | **Planned** — **enters AIMS scope automatically on operational launch** (scope-entry trigger: first processing of real user data) |

**Not an AI system (host only):** the **CareRate / Rate.nl** measurement platform uses no AI/ML of its own; governed under the ISMS.

**Exclusions:** **EAGLE** (separate GGZ joint venture, governed separately); education & non-healthcare segments; fully anonymised data; corporate HR/finance (inherited ISMS/NEN exclusions).

### 4.4 The AIMS

The organization establishes, implements, maintains and continually improves the AIMS in accordance with ISO/IEC 42001:2023, **integrated with** the existing ISMS (shared risk methodology, document control, internal audit, management review, competence, supplier and incident management), extended with AI-specific processes (AI risk assessment, AI System Impact Assessment, AI lifecycle controls, transparency).

---

## 5. Leadership

### 5.1 Leadership and commitment

Top management (CEO / AIMS Owner) is accountable for the AIMS: it sets the AI Policy and objectives, provides resources, integrates AIMS requirements into business processes, and promotes responsible AI. AI risk treatment, the AI Policy and objectives are approved by the CEO.

### 5.2 AI Policy

**Commitment.** The group develops and operates AI handling sensitive health information for vulnerable people, and is committed to doing so **responsibly, lawfully, safely and transparently**.

**Principles:**
1. **Lawfulness & compliance** — GDPR, EU AI Act, Wkkgz/Wabvpz, ISO 27001/NEN 7510. Voice/health data = special-category.
2. **Human oversight — no autonomous decisions** — AI supports, never decides. iVessy = data collector with human-in-the-loop; no diagnosis, triage, profiling or behavioural steering. Vess360 emotion = supportive context only.
3. **Transparency** — users are told before each session that it is AI, the purpose, the data processed (speech, content, emotion), that audio is transient/not stored, that emotion may be shown to the professional, and their GDPR rights. **Explicit consent obtained and logged** (EU AI Act Art. 50 for emotion recognition).
4. **Fairness & non-discrimination** — iVessy monitored across language, accent/dialect, level of assistance; Vess360 fairness assured at dataset level + aggregate review (no demographic attributes stored — documented limitation).
5. **Safety, robustness & reliability** — deterministic guardrails (schema-only output, reject extra text, clarification questions, user confirmation loop); emotion shown **only at confidence ≥ 0.70** and otherwise labelled "uncertain".
6. **Privacy & data governance** — privacy-by-design; audio transient/not stored; structured output only; meta-logs only; tenant isolation; stateless inference; patient data not used to train Vess360; documented provenance/consent for all data.
7. **Security** — AI assets protected under ISMS controls; AI incidents handled via the ISMS process (extended for bias/drift/hallucination/adversarial input).
8. **Accountability & governance** — defined roles; risk assessment, SoA and impact assessments maintained.
9. **Lifecycle management** — model cards, model/data versioning, validation before deployment, ongoing monitoring incl. drift; change control for the iVessy migration.
10. **Supplier management** — AI providers assessed for security, data-use, transfer exposure, incident duties.
11. **Continual improvement** — monitored, audited, reviewed and improved.

Reviewed at least annually and after significant change; re-approved by the CEO.

### 5.3 Roles, responsibilities and authorities (RACI)

| AIMS role | Person | Responsibility |
|---|---|---|
| **AIMS Owner** (accountable) | Inge Proost (CEO) | Approves AI Policy, risk treatment, objectives; resources the AIMS |
| **AI Technical Lead** (responsible) | Firas Kassoumeh | AIMS implementation & operation; risk, lifecycle, data governance, evidence |
| All staff & contractors | — | Follow the AI Policy; report AI concerns/incidents; complete training |

| Activity | AIMS Owner | AI Technical Lead | Staff |
|---|---|---|---|
| AI Policy & objectives | A | R | I |
| AI risk assessment & treatment | A | R | C |
| AI System Impact Assessment | A | R | C |
| SoA approval | A | R | I |
| Lifecycle controls (model cards, validation, monitoring) | I | A/R | C |
| Supplier/data governance | A | R | C |
| Internal audit | A | R / independent reviewer | I |
| Incident response (AI) | A | R | C |

Small-organization segregation-of-duties limitation and compensating controls are inherited from the ISMS (independent periodic review; CEO approval of risk/policy; logging of privileged actions; annual internal audit) and apply to the AIMS.

---

## 6. Planning

### 6.1 Actions to address risks and opportunities

#### 6.1.1 Approach
The AIMS uses the existing ISMS risk methodology, extended with AI-specific risk sources and the AI System Impact Assessment. Risks are identified per AI system, assessed on the ISMS scales, treated, and recorded in the AI Risk Register (Part II). Opportunities (efficiency, inclusion, data quality) are pursued through the AI objectives.

#### 6.1.2 AI risk assessment — criteria
Mirroring the ISMS scales:

| Scale | Levels |
|---|---|
| Impact | High / Medium / Low (harm to individuals & fundamental rights weighted highest) |
| Likelihood | High / Medium / Low |
| Risk level | Impact × Likelihood → High 🔴 / Medium 🟡 / Low 🟢 |

**Risk appetite:** **Low tolerance** for risks to safety, health, fundamental rights, and legal compliance (these must be treated to Low, or formally accepted by the CEO with justification). **Moderate tolerance** for performance/accuracy risks during the pilot phase, provided human oversight and transparency are in place.

AI-specific risk sources considered: bias/unfair outcomes; lack of transparency/explainability; hallucination/incorrect output; over-reliance/automation bias; misuse beyond intended purpose; emotion misclassification; model drift; data quality/provenance; privacy/special-category data; security/adversarial input; third-party/model-supplier dependency and data transfer.

#### 6.1.3 AI risk treatment and Statement of Applicability
Risks are treated (mitigate/transfer/avoid/accept). Applicability of Annex A controls is recorded in the **Statement of Applicability (Part III)**. Residual risks outside appetite require CEO acceptance.

#### 6.1.4 AI System Impact Assessment (AISIA)
For each in-scope AI system, an AISIA assesses impacts on individuals (privacy, fairness, safety, autonomy, dignity) and society, before deployment and on significant change. AISIAs are in **Part IV**; the data-protection assessment is in **Part VII (DPIA)**.

### 6.2 AI objectives and planning

| Objective | Target | Evidence |
|---|---|---|
| Administrative efficiency (iVessy pilots) | **≥ 20% reduction in intake time**, no significant data-quality drop | Pilot time-motion logs + EPD timestamps (WP2, 2026) |
| Field-extraction quality (iVessy) | Field-accuracy ≥ 90%; "needs-clarification" rate trended down | Pilot validation set |
| Emotion reliability (Vess360) | Display only at confidence ≥ 0.70; improve accuracy over the ~0.48 Dutch baseline; never used for decisions | Model evaluation + monitoring |
| Fairness | No material performance gap across monitored groups | Subgroup performance review |
| Model monitoring | **Semi-annual** performance/drift check + retrain trigger on a defined accuracy drop | Monitoring log |
| Governance maturity | DPIA, model cards, risk register & SoA in place and maintained | This manual |

### 6.3 Planning of changes
Changes to AI systems — including the **iVessy migration OpenAI → EU → self-hosted** — follow change management: impact/risk re-assessment, validation, AISIA/DPIA update, and CEO approval before production.

---

## 7. Support

- **7.1 Resources** — people (AIMS Owner, AI Technical Lead), compute (Hetzner EU, Azure/Google EU for Vess360, GPU for training), tools (PyTorch, Hugging Face, Docker, GitHub), per the AI resource register (Part V).
- **7.2 Competence** — the AI Technical Lead maintains competence in AI/ML, security and AI governance; training needs identified and records kept in Google Drive (per ISMS).
- **7.3 Awareness** — staff are made aware of the AI Policy, their role, responsible-AI principles and how to report AI concerns (via the ISMS reporting channel).
- **7.4 Communication** — internal (governance meetings, dashboards) and external (transparency to users, supplier/partner communication, incident reporting).
- **7.5 Documented information** — this manual, the SoA, risk register, AISIAs, DPIA, model cards, registers, logs and records; controlled in the rate-nl/ISO repository and Google Drive; retention per §9.

---

## 8. Operation

- **8.1 Operational planning & control** — AI systems operated per the documented lifecycle controls (Part VI), within the defined intended use, with human oversight and logging.
- **8.2 Operational AI risk assessment** — re-run on significant change, new use case, incident, or supplier/model change.
- **8.3 Operational AI risk treatment** — controls applied and verified per the SoA.
- **8.4 Operational AISIA/DPIA** — updated before each new deployment/material change; reviewed at pilot milestones.

---

## 9. Performance evaluation

- **9.1 Monitoring, measurement, analysis & evaluation** — track the AI objectives (§6.2): intake-time reduction, data quality, emotion confidence/accuracy, fairness, drift, incident counts. Reviewed at governance meetings.
- **9.2 Internal audit** — the AIMS is added to the existing internal-audit programme (the ISMS audit cycle is operational). AI controls are audited against this manual and Annex A before any external assessment.
- **9.3 Management review** — the CEO reviews AIMS performance (objectives, risks, incidents, audit results, changes, supplier status) at least annually and records decisions.

**Records retention (from ISMS):** operational backups **1 month**; security/compliance logs **1 year**; ISMS & AI records (audits, incidents, corrective actions, impact assessments) **3 years** (Google Drive).

---

## 10. Improvement

- **10.1 Continual improvement** — the AIMS is improved through monitoring, audit, review and lessons learned; planned actions are tracked in Appendix A.
- **10.2 Nonconformity & corrective action** — AI nonconformities/incidents are logged, corrected, root-caused and tracked using the existing ISMS corrective-action process (extended for AI-specific incident types).

---

# PART II — AI RISK REGISTER

Scales and appetite per §6.1.2. Owner of all entries: AI Technical Lead (treatment), AIMS Owner (acceptance).

## iVessy

| # | Risk | Impact | Likelihood | Treatment | Residual |
|---|---|---|---|---|---|
| iV-1 | Hallucination / incorrect structuring of care data | High | Medium | Schema-only output; reject extra text → clarification question; **user confirmation loop**; human-in-the-loop before record commit | Low 🟢 |
| iV-2 | **OpenAI (US) processing** of health-related input → GDPR transfer / CLOUD-Act exposure | High | Medium | DPA + EU data terms; minimise/avoid sending identifiable special-category data; transient processing; **planned migration to EU/self-hosted** | Medium 🟡 (until migration) |
| iV-3 | ASR error / poor input quality | Medium | Medium | ASR confidence + re-ask; slot/format validation; user confirmation | Low 🟢 |
| iV-4 | Bias across language / accent / assistance level | High | Medium | Multilingual testing; fairness monitoring; Avans inclusion research; plain language | Medium 🟡 |
| iV-5 | Automation bias / over-reliance by professionals | High | Medium | "Supportive only" framing; mandatory human validation; training; clear UI | Medium 🟡 |
| iV-6 | Use beyond intended purpose (triage/diagnosis) | High | Low | Intended-use controls; user instructions; contracts; no decision features | Low 🟢 |
| iV-7 | Data leakage across tenants/sessions | High | Low | Tenant isolation (keys + namespaces); stateless inference; no audio storage | Low 🟢 |
| iV-8 | Vulnerable users misunderstand the AI | Medium | Medium | Consent + plain-language explanation; review/edit/confirm; multilingual | Low 🟢 |

## Vess360

| # | Risk | Impact | Likelihood | Treatment | Residual |
|---|---|---|---|---|---|
| Ve-1 | **Low emotion accuracy** (~0.48 Dutch baseline) misleads professionals | High | High | Supportive-only; **confidence ≥ 0.70 threshold** + "uncertain" labelling; human interpretation; **accuracy-improvement objective**; never autonomous | Medium 🟡 |
| Ve-2 | Emotion misclassification bias (atypical expression, dialect, culture) | High | Medium | Diverse training corpus; aggregate fairness review; documented limitation; never decision-driving | Medium 🟡 |
| Ve-3 | EU AI Act emotion-recognition compliance | High | Low | Consent + disclosure (Art. 50); medical context only; **no workplace/education use**; no profiling | Low 🟢 |
| Ve-4 | Azure/Google **EU-region but US-provider** transfer exposure | Medium | Medium | DPA + SCCs; EU regions; transfer assessment (Part VII); access controls | Medium 🟡 |
| Ve-5 | Training-data licence breach (MSP-Podcast reconstruction/redistribution) | Medium | Low | No raw-data redistribution; no model reconstruction of corpus; access control; licence terms tracked | Low 🟢 |
| Ve-6 | Model drift over time | Medium | Medium | Semi-annual performance check + retrain trigger; versioning | Low 🟢 |

---

# PART III — STATEMENT OF APPLICABILITY (ISO 42001 Annex A)

Status: ✅ Implemented · 📋 Defined (concrete approach in place; operationalised through pilots/rollout). All controls Applicable.

## A.2 Policies for AI
| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.2.2 | AI policy | ✅ | AI Policy (§5.2), CEO-approved, integrated with ISMS policy | AIMS Owner |
| A.2.3 | Alignment with other policies | ✅ | §6/§5.2 aligned with ISMS policies | AI Technical Lead |
| A.2.4 | Review of AI policy | ✅ | Annual review cycle defined and recorded (§5.2/§7.5) | AIMS Owner |

## A.3 Internal organization

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.3.2 | Roles & responsibilities | ✅ | RACI (§5.3) | AIMS Owner |
| A.3.3 | Reporting of concerns | ✅ | AI concerns reported via the ISMS incident/reporting channel; communicated in awareness (§7.3) | AI Technical Lead |

## A.4 Resources for AI systems

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.4.2 | Resource documentation | ✅ | AI resource register (Part V) | AI Technical Lead |
| A.4.3 | Data resources | ✅ | Data register (Part V); provenance/licences documented | AI Technical Lead |
| A.4.4 | Tooling resources | ✅ | Tooling listed (PyTorch, HF, Docker, GitHub) | AI Technical Lead |
| A.4.5 | System & computing resources | ✅ | Hetzner EU; Azure/Google EU (Vess360); GPU | AI Technical Lead |
| A.4.6 | Human resources | ✅ | Roles & competence (§5.3/§7.2) | AIMS Owner |

## A.5 Assessing impacts of AI systems

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.5.2 | Impact assessment process | ✅ | AISIA process (§6.1.4) | AI Technical Lead |
| A.5.3 | Documentation of impact assessments | ✅ | AISIAs (Part IV) + DPIA (Part VII) | AI Technical Lead |
| A.5.4 | Impact on individuals | ✅ | Part IV (privacy, fairness, safety, autonomy) | AI Technical Lead |
| A.5.5 | Societal impacts | ✅ | Part IV societal section | AI Technical Lead |

## A.6 AI system life cycle

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.6.1 | Management guidance for responsible development | ✅ | AI Policy + lifecycle controls (Part VI) | AIMS Owner |
| A.6.2 | AI system life cycle (design→verification→deployment→operation→monitoring; technical docs; event logs) | ✅ | Part VI controls + model cards (Part VIII) | AI Technical Lead |

## A.7 Data for AI systems

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.7.2 | Data for development | ✅ | Data register; Vess360 corpora; iVessy protocol/anonymised data | AI Technical Lead |
| A.7.3 | Acquisition of data | ✅ | MSP-Podcast licence; consent for own corpus | AI Technical Lead |
| A.7.4 | Quality of data | ✅ | Multi-rater consensus labelling; preprocessing & quality checks | AI Technical Lead |
| A.7.5 | Data provenance | ✅ | Provenance recorded per dataset (Part V) | AI Technical Lead |
| A.7.6 | Data preparation | ✅ | Preprocessing/labelling documented (Part VIII) | AI Technical Lead |

## A.8 Information for interested parties

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.8.2 | Documentation for users | ✅ | User information + consent flow (Part VI); user-facing explanation provided per session | AI Technical Lead |
| A.8.3 | External reporting (adverse impacts) | ✅ | External parties can report adverse impacts via the Rate.nl support/contact channel, routed to the AI Technical Lead and logged | AI Technical Lead |
| A.8.4 | Communication of incidents | ✅ | AI incident communication via the ISMS incident process | AIMS Owner |
| A.8.5 | Legal reporting obligations | ✅ | GDPR breach notification to the AP within 72h; EU AI Act serious-incident reporting once applicable; mapped in Part VII | AIMS Owner |

## A.9 Use of AI systems

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.9.2 | Processes for responsible use | ✅ | Intended-use + human-oversight controls (Part VI) | AI Technical Lead |
| A.9.3 | Objectives for responsible use | ✅ | Fairness, transparency, oversight (§5.2/§6.2) | AIMS Owner |
| A.9.4 | Intended use | ✅ | Data collection only; no decisions; documented & enforced | AI Technical Lead |

## A.10 Third-party & customer relationships

| Control | Title | Status | Justification / implementation | Owner |
|---|---|---|---|---|
| A.10.2 | Allocating responsibilities | ✅ | Controller/processor split and supplier/partner/customer roles documented (Part VII) | AIMS Owner |
| A.10.3 | Suppliers | ✅ | AI supplier register + assessment (Part V) | AI Technical Lead |
| A.10.4 | Customers | ✅ | Customer requirements captured in contracts/DPAs | AIMS Owner |

---

# PART IV — AI SYSTEM IMPACT ASSESSMENTS (AISIA)

## iVessy
- **Purpose:** voice-driven collection/structuring of care information; output to professionals via FHIR/HL7. No decisions.
- **Affected individuals:** clients/patients incl. low-literacy, non-native, elderly, cognitively impaired; informal caregivers; professionals.
- **Potential impacts & mitigations:**
  - *Privacy* (special-category voice/health data) → transient audio (not stored), structured output only, consent, tenant isolation, DPIA (Part VII). **Residual: Low–Medium** (Medium while OpenAI/US is used).
  - *Fairness* (language/accent) → multilingual testing, monitoring, Avans research. **Residual: Medium.**
  - *Safety / data integrity* (wrong field) → guardrails + confirmation loop + human validation. **Residual: Low.**
  - *Autonomy / dignity* → review/edit/confirm; plain language; no behavioural steering. **Residual: Low.**
  - *Transparency* → pre-session disclosure + logged consent. **Residual: Low.**
- **Societal:** improves inclusion and reduces administrative burden; over-reliance mitigated by human-in-the-loop. **Net positive.**
- **Provisional EU AI Act class:** limited-risk + transparency. **Decision:** proceed in pilots with controls; reassess on migration and scale.

## Vess360
- **Purpose:** voice-emotion recognition (6 emotions) as supportive context.
- **Affected individuals:** speakers whose emotion is inferred (patients/clients).
- **Potential impacts & mitigations:**
  - *Misleading/incorrect emotion* (low accuracy) → supportive-only, confidence ≥ 0.70 threshold + uncertainty labelling, human interpretation, accuracy objective. **Residual: Medium.**
  - *Bias* (atypical/dialect/cultural expression) → diverse corpus, aggregate review, documented limitation. **Residual: Medium.**
  - *Privacy* → no demographic data stored; transient audio; consent. **Residual: Low.**
  - *Transparency* → emotion disclosed, consented (Art. 50). **Residual: Low.**
  - *Transfer* (Azure/Google EU-region/US-provider) → DPA/SCCs, transfer assessment (Part VII). **Residual: Medium.**
- **Societal:** supports empathic care; misuse mitigated by no-decision rule and no workplace/education use.
- **Provisional EU AI Act class:** emotion recognition with transparency obligations; medical context. **Decision:** proceed with controls; accuracy improvement is a tracked objective.

---

# PART V — REGISTERS

## AI resource register (A.4)
| Resource | Detail | Owner |
|---|---|---|
| Model: iVessy LLM | OpenAI (current) → Mixtral 8x7B self-hosted (planned) | AI Technical Lead |
| Model: ASR | Whisper (planned self-hosted) | AI Technical Lead |
| Model: Vess360 | wav2vec2-based emotion model (in-house) | AI Technical Lead |
| Compute | Hetzner EU (prod); Azure/Google EU (Vess360); GPU (training) | AI Technical Lead |
| Tooling | PyTorch, Hugging Face, Docker, GitHub, FastAPI/Flask | AI Technical Lead |
| People | AIMS Owner; AI Technical Lead | AIMS Owner |

## AI data register (A.7)
| Dataset | Source | Rights / consent | Notes |
|---|---|---|---|
| **MSP-Podcast** (2,000-sample subset) | UT Dallas (licensed) | Non-exclusive, perpetual; **commercial model use permitted**; **no reconstruction; no raw-data redistribution** | Vess360 training |
| **DUTCHDES / DUTCHESS** | Public crowd-sourced Dutch emotion speech | Per dataset terms | Vess360 fine-tuning |
| **Own Dutch corpus** | In-house recordings | Informed consent; anonymised; technical metadata only | Vess360 training/validation |
| Care protocols | Non-patient | Internal | iVessy RAG/fine-tuning |
| Anonymised dialogue content (iVessy) | Patients (consented) | Explicit consent + DPIA | Dialogue/form-logic improvement only |

## AI supplier register (A.10)
| Supplier | Service | Location | Assessment focus | Status |
|---|---|---|---|---|
| OpenAI | iVessy LLM (current) | US | DPA, transfer/CLOUD Act, data-use limits, migration plan | Active (transitional) |
| Microsoft Azure | Vess360 STT | EU region | DPA/SCCs, transfer, security | Active |
| Google Cloud | Vess360 translate/run/training | EU region | DPA/SCCs, transfer, security | Active |
| Mistral (Mixtral) / Whisper | Self-hosted models | EU/on-prem | Licence, self-hosting controls | Planned |
| Hetzner / Azure (failover) / Google Workspace / GitHub / LastPass / Exact Online | Infrastructure & tooling (inherited ISMS) | EU | Per ISMS supplier review | Active |

---

# PART VI — AI LIFECYCLE & OPERATIONAL CONTROLS (A.6, A.8, A.9)

- **Model documentation (model cards)** — maintained for iVessy LLM, Whisper ASR and Vess360 in **Part VIII**.
- **Version control** — models and training data versioned (GitHub + model registry); each production model traceable to its data and configuration.
- **Validation before deployment** — documented acceptance tests (iVessy: field accuracy, missing fields, contradiction rate, "needs-clarification" rate; Vess360: per-emotion F1/accuracy + fairness) before any production use.
- **Deployment approval** — AI Technical Lead validates; CEO approves significant changes.
- **Monitoring** — performance, confidence, fairness and incident monitoring in operation; **semi-annual drift check** + retrain trigger on a defined accuracy drop; ad-hoc after major changes.
- **Rollback** — ability to revert to the previous validated model version.
- **Event logging** — meta-information logs (questions asked, FHIR fields filled, timestamps, interpretation step, consent); encrypted; retention/access per ISMS.
- **Transparency & consent (A.8/A.9)** — pre-session disclosure + logged explicit consent; emotion recognition disclosed; user can review/edit/confirm; intended-use enforced.
- **AI incident handling** — bias, drift, hallucination, adversarial input handled via the ISMS incident + corrective-action process; communicated per A.8.4.

---

# PART VII — DATA PROTECTION IMPACT ASSESSMENT (DPIA)

Conducted under GDPR Art. 35 (special-category health data via voice). Covers iVessy and Vess360.

## 1. Roles (controller / processor)
- **Care deployment (patient data):** the **healthcare organization is the data controller**; **CareRate B.V. / Vess B.V. act as processor** under a Data Processing Agreement. No patient data is used to train models.
- **Vess360 model training (own corpus):** **Vess B.V. is the controller**, processing on the basis of **informed consent**, anonymised, technical metadata only.

## 2. Description of processing
- **Nature:** voice is captured, transcribed (ASR), structured into care fields (iVessy) and/or analysed for emotion (Vess360); output is shown to a professional for review.
- **Data categories:** special-category health data (spoken content), voice audio (transient), inferred emotion, and structured care fields. **No demographic attributes stored by Vess360.**
- **Data subjects:** patients/clients (incl. vulnerable groups), informal caregivers.
- **Recipients:** the healthcare organization (controller); AI sub-processors (OpenAI — transitional; Azure/Google EU for Vess360).
- **Retention:** audio **not stored** (transient); structured output retained per the controller's policy and the ISMS retention schedule; logs = meta-information only.
- **International transfers:** OpenAI (US) — transitional, under DPA + safeguards, migration to EU/self-hosted planned; Azure/Google in EU regions (US-headquartered) — DPA + SCCs + transfer assessment.

## 3. Lawful basis
- Art. 6(1) and Art. 9(2)(h) (provision of health/social care) and/or Art. 9(2)(a) explicit consent, as established by the controller; AIMS-level processing relies on explicit, logged consent before each session.

## 4. Necessity & proportionality
Processing is limited to what is needed to collect/structure care information and provide supportive emotional context; data minimisation (transient audio, structured output only), purpose limitation, and human oversight ensure proportionality.

## 5. Risks to data subjects & measures
| Risk | Measure | Residual |
|---|---|---|
| Exposure of special-category data | Transient audio; structured output only; tenant isolation; encryption; access control | Low |
| US transfer (OpenAI) | DPA + safeguards; minimise identifiable data; migration to EU/self-hosted | Medium → Low after migration |
| US-provider transfer (Azure/Google EU) | DPA + SCCs + transfer assessment; EU regions | Medium |
| Incorrect/biased inference affecting care | Human-in-the-loop; confidence threshold; fairness monitoring | Medium |
| Lack of awareness/consent | Pre-session disclosure + logged explicit consent; review/edit/withdraw | Low |

## 6. Breach & reporting
Personal-data breaches handled via the ISMS incident process; notification to the **Autoriteit Persoonsgegevens within 72 hours** where required; data subjects informed when high risk; EU AI Act serious-incident reporting once applicable.

## 7. Conclusion
With the measures above, residual risk is acceptable for pilot deployment. The DPIA is reviewed before processing real patient data, on the iVessy model/hosting migration, and on any material change.

---

# PART VIII — MODEL CARDS

## 8.1 iVessy dialogue LLM
- **Model:** OpenAI model (current, transitional) → **Mixtral 8x7B Instruct**, self-hosted (planned). Decoder-only Transformer (sparse Mixture-of-Experts for Mixtral).
- **Intended use:** generate natural multilingual questions and structure free speech into allowed FHIR/HL7 fields. **Not** for diagnosis, triage or decisions.
- **Inputs/outputs:** transcribed text in → schema-constrained JSON/FHIR fields out (extra text rejected).
- **Adaptation:** domain adaptation only — RAG over care protocols; LoRA/QLoRA fine-tuning on protocol-grounded Q/A, intake→FHIR extraction, safe-refusal patterns. **No patient data used for training.**
- **Performance targets (evidenced in pilots):** field accuracy ≥ 90%; low contradiction rate; controlled "needs-clarification" rate.
- **Limitations:** can mis-phrase or mis-structure → mitigated by schema guardrails + user confirmation + human validation.
- **Guardrails:** schema-only output; clarification loop; user confirmation before record commit.

## 8.2 ASR (speech-to-text)
- **Model:** **Whisper** (planned self-hosted, EU/on-prem).
- **Intended use:** transcribe spoken input to text for structuring; audio processed transiently and not stored.
- **Limitations:** accuracy varies by accent/dialect/audio quality → ASR-confidence re-ask policy + slot validation.

## 8.3 Vess360 voice-emotion model
- **Model:** wav2vec2-based Transformer encoder; outputs **6 Ekman emotions** (happy, sad, angry, fear, disgust, surprise) plus neutral; per-prediction confidence.
- **Training data:** MSP-Podcast (licensed), DUTCHDES/DUTCHESS, and the own human-validated Dutch corpus (3 intensity variants per emotion; multi-rater consensus; consented; anonymised).
- **Performance (baseline):** ~0.48 accuracy on Dutch emotion speech; **improvement is a tracked objective**.
- **Operating rule:** emotion shown **only at confidence ≥ 0.70**, otherwise labelled "uncertain"; **supportive context only; never autonomous; no profiling**.
- **Intended use:** supportive emotional context for professionals in a medical setting, with disclosure and consent.
- **Out-of-scope uses:** workplace or education emotion recognition (prohibited under EU AI Act Art. 5); any autonomous or decision-making use.
- **Limitations:** atypical/comorbid expression, dialect and cultural variation reduce reliability → human interpretation required.

---

# Appendix A — Continual-improvement plan (planned actions)

| # | Action | Owner | Target |
|---|---|---|---|
| 1 | NEN 7510:2022 certification (external audit alongside AIMS/AI-Act assessment) | AIMS Owner | 2026 |
| 2 | Add **Vess B.V.** to the certified ISO 27001 / AIMS boundary | AIMS Owner | At AIMS certification |
| 3 | Complete iVessy migration OpenAI → EU → self-hosted (Mixtral + local Whisper) | AI Technical Lead | Per migration roadmap |
| 4 | Improve Vess360 emotion accuracy above the ~0.48 baseline | AI Technical Lead | Ongoing; reviewed semi-annually |
| 5 | Review the Vess360 confidence threshold (currently 0.70) after first pilot | AI Technical Lead | After WP2 pilot |
| 6 | Onboard **Vera** into the AIMS at operational launch (AISIA + model card + DPIA update) | AI Technical Lead | At Vera launch |
| 7 | Establish iVessy pilot performance baselines (intake time, field accuracy) | AI Technical Lead | WP2, 2026 |

# Appendix B — Document history
| Version | Date | Change | Author |
|---|---|---|---|
| 0.1 | 2026 | Initial consolidated AIMS (Clauses 4–10, SoA, risk register, AISIA, registers, lifecycle) | Firas Kassoumeh |
| 1.0 | 18 Jun 2026 | Completed all sections: added DPIA (Part VII) and Model Cards (Part VIII); set Vess360 confidence threshold (0.70); completed Vera entry, SoA, objectives and supplier statuses; recorded ISO 27001 certificate; converted open items into a continual-improvement plan; issued | Firas Kassoumeh |
