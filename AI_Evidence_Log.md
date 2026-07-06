# AI Evidence Log

**Purpose:** central register of evidence proving the AIMS operates as documented in `AIMS.md`. This is the file an auditor asks for. It mirrors the ISMS `Logs.md` approach.
**Owner:** Firas Kassoumeh (AI Technical Lead) — collection · Inge Proost (AIMS Owner) — review
**Related:** `AIMS.md`, `readme.md` (ISMS), `Logs.md` (ISMS evidence)
**Status legend:** ⬜ Planned · 🔄 In progress · ✅ Collected
**How to use:** when something is done/measured, fill the row — date, result, and a link to the raw data (Google Drive / GitHub / EPD export). Keep raw files; this log points to them.

> Note: iVessy is in the **development phase**, so most performance evidence is **Planned** until the WP2 pilot (2026). Targets are pre-filled; results are added when measured. The only measured baseline so far is Vess360 accuracy ≈ 0.48.

---

## 1. Evidence index (master map)

| Ref | AIMS item | Evidence needed | Location | Status |
|---|---|---|---|---|
| E-1 | Objective: iVessy intake-time reduction | Time-motion / EPD timestamp comparison | Google Drive / EPD export | ⬜ |
| E-2 | Objective: iVessy field quality | Validation-set results (accuracy, clarification, contradiction) | GitHub / Drive | ⬜ |
| E-3 | Objective: Vess360 emotion reliability | Model evaluation report (F1/accuracy, confidence) | GitHub / Drive | 🔄 |
| E-4 | Objective: Fairness | Subgroup performance review | Drive | ⬜ |
| E-5 | Objective: Model monitoring | Semi-annual drift-check log (this file, §5) | This file | ⬜ |
| E-6 | A.5 / Section 9 | Standalone DPIA drafted (v1.0, 8 Jul 2026); CEO signature pending | Drive | 🔄 |
| E-7 | A.6 / Section 10 | Model cards (versioned) | GitHub | 🔄 |
| E-8 | A.6.2 | Validation records — Go/No-Go decision rule defined (AIMS Section 13); runs pending (hard blocker) | GitHub / Drive | ⬜ |
| E-9 | A.8/A.9 | Consent & transparency logs | App logs / Drive | ⬜ |
| E-10 | A.10.3 | Supplier DPAs/SCCs — SAR-001/002/003 drafted (public due diligence); signed DPAs pending | Drive | 🔄 |
| E-11 | A.8.4 / 10.2 | AI incident records | This file, §8 / ISMS | ⬜ |
| E-12 | Clause 9.2 / 9.3 | Internal audit + management review | Drive | ⬜ |
| E-13 | Clause 7.2/7.3 | Training & awareness records | Drive | ⬜ |

---

## 2. iVessy — pilot performance (E-1, E-2) — objective §6.2

| Metric | Target | Result | Date | Pilot / org | Evidence link | Status |
|---|---|---|---|---|---|---|
| Intake-time reduction | ≥ 20% | — | — | — | — | ⬜ |
| Field-extraction accuracy | ≥ 90% | — | — | — | — | ⬜ |
| Missing-fields rate | trend ↓ | — | — | — | — | ⬜ |
| Contradiction rate | low | — | — | — | — | ⬜ |
| "Needs-clarification" rate | trend ↓ | — | — | — | — | ⬜ |
| Data-quality vs. baseline | no significant drop | — | — | — | — | ⬜ |

*Method:* WP2 pilot, ≥3 care organisations, ~100 clients each; primary outcome time-per-intake (EPD logs); registered prospectively.

---

## 3. Vess360 — model evaluation (E-3) — risk Ve-1/Ve-2

| Metric | Baseline | Target | Latest result | Date | Model version | Evidence link | Status |
|---|---|---|---|---|---|---|---|
| Overall accuracy (Dutch) | ≈ 0.48 | improve over baseline | — | — | — | — | 🔄 |
| Confidence display threshold | 0.70 (rule) | maintained | — | — | — | — | ✅ (rule set in AIMS.md) |
| Per-emotion F1 — happy | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — sad | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — angry | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — fear | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — disgust | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — surprise | — | — | — | — | — | — | ⬜ |
| Per-emotion F1 — neutral | — | — | — | — | — | — | ⬜ |

---

## 4. Fairness / bias checks (E-4) — risk iV-4 / Ve-2

| System | Attribute monitored | Method | Result / gap | Date | Evidence link | Status |
|---|---|---|---|---|---|---|
| iVessy | Language | Subgroup performance | — | — | — | ⬜ |
| iVessy | Accent / dialect | Subgroup performance | — | — | — | ⬜ |
| iVessy | Level of assistance | Subgroup performance | — | — | — | ⬜ |
| Vess360 | Dataset diversity (no demographics stored) | Corpus-level review + aggregate accuracy | — | — | — | ⬜ |

---

## 5. Model monitoring & drift (E-5) — semi-annual — objective §6.2

| Date | System / model version | Metric checked | Result | Drift vs. previous | Retrain triggered? | Owner | Status |
|---|---|---|---|---|---|---|---|
| — | — | — | — | — | — | AI Technical Lead | ⬜ |
| — | — | — | — | — | — | AI Technical Lead | ⬜ |

*Cadence:* twice per year + after any major change. Retrain trigger = defined accuracy drop.

---

## 6. DPIA records (E-6) — Section 9

| System | DPIA status | Version / date | Reviewed by | Controller (deployment) | Evidence link | Status |
|---|---|---|---|---|---|---|
| iVessy | Standalone DPIA drafted (DPIA_iVessy_Vess360 v1.0) | v1.0 / 8 Jul 2026 | Inge Proost (signature pending) | Healthcare org (processor: CareRate B.V.) | DPIA_iVessy_Vess360.docx | 🔄 signature pending |
| Vess360 | Standalone DPIA drafted (same document) | v1.0 / 8 Jul 2026 | Inge Proost (signature pending) | Vess B.V. (own corpus) | DPIA_iVessy_Vess360.docx | 🔄 signature pending |

*Action:* finalise & sign before processing real patient data; review on iVessy migration.

---

## 7. Model cards & deployment validation (E-7, E-8) — Section 8/10

| Model | Card location | Current version | Validation done | Validation date | Approved by | Status |
|---|---|---|---|---|---|---|
| iVessy LLM (OpenAI → Mixtral) | AIMS.md §10 (MC-001) / GitHub | — | — | — | — | 🔄 |
| ASR Whisper | AIMS.md §10 (MC-002) / GitHub | — | — | — | — | 🔄 |
| Vess360 emotion | AIMS.md §10 (MC-003) / GitHub | — | — | — | — | 🔄 |

*Deployment decision rule (Go / Conditional Go / No-Go) defined in AIMS Section 13. MVR-001/002 runs pending — hard blocker for live patient data.*

---

## 8. Consent & transparency logs (E-9) — A.8/A.9

| Pilot / org | Consent flow shown | Consent logged | Emotion disclosure shown | Sample export link | Date | Status |
|---|---|---|---|---|---|---|
| — | — | — | — | — | — | ⬜ |

---

## 9. Supplier DPAs / transfer safeguards (E-10) — A.10.3

| Supplier | Service | DPA signed | SCCs / transfer safeguard | Review date | Evidence link | Status |
|---|---|---|---|---|---|---|
| OpenAI | iVessy LLM (current, US) | Pending | SCTs (obtain) | — | SAR-001 drafted | 🔄 SAR drafted; DPA pending |
| Microsoft Azure | Vess360 STT (EU region) | Pending | SCCs (confirm) | — | SAR-002 drafted | 🔄 SAR drafted; DPA pending |
| Google Cloud | Vess360 translate/run/training (EU region) | Pending | SCCs (confirm) | — | SAR-003 drafted | 🔄 SAR drafted; DPA pending |

---

## 10. AI incident log (E-11) — A.8.4 / 10.2

| ID | Date | Type (bias / drift / hallucination / adversarial / privacy) | Description | Action taken | Reported to (if applicable) | Status |
|---|---|---|---|---|---|---|
| AI-INC-0001 | — | — | — | — | — | ⬜ |

*Process:* logged & handled via the ISMS incident + corrective-action process; GDPR breach → AP within 72h where required.

---

## 11. Internal audit & management review (E-12) — Clause 9.2/9.3

| Activity | Date | Outcome / findings | Actions | Owner | Status |
|---|---|---|---|---|---|
| AIMS internal audit | — | — | — | AI Technical Lead | ⬜ |
| AIMS management review | — | — | — | AIMS Owner | ⬜ |

---

## 12. Training & awareness (E-13) — Clause 7.2/7.3

| Person / group | Topic (responsible AI, bias, AI Act, incident reporting) | Date completed | Evidence link | Status |
|---|---|---|---|---|
| — | — | — | — | ⬜ |

---

## Document history
| Version | Date | Change | Author |
|---|---|---|---|
| 1.0 | 18 Jun 2026 | Initial evidence-log template created with index, targets and baselines pre-filled | Firas Kassoumeh |
| 1.1 | 8 Jul 2026 | Synced with AIMS v3.0 gap-remediation (B1–B11): standalone DPIA drafted (E-6); Go/No-Go rule (E-8); SAR-001/002/003 drafted (E-10); Part→Section references updated | Firas Kassoumeh |
