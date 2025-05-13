# ISMS Evidence & Logs

_A single file to capture and track all required ISMS evidence in one place._

---

## Summary Table

| Evidence Title               | Purpose                                                | Retention Period   | Responsible Owner   | Last Updated |
|:-----------------------------|:-------------------------------------------------------|:-------------------|:--------------------|:-------------|
| Training Completion Log      | Confirm annual employee awareness training             | 3 years            | Managing Director   | YYYY-MM-DD   |
| Incident Response Log        | Track security events and responses                    | 3 years            | Managing Director   | YYYY-MM-DD   |
| Access Control Review Record | Review of user permissions and updates                 | 3 years            | Team Lead Developer | YYYY-MM-DD   |
| DB Restore Test Log          | Confirm successful backup recovery tests               | 1 year             | Team Lead Developer | YYYY-MM-DD   |
| Backup Job Reports           | Proof of scheduled backup executions                   | 1 year             | Team Lead Developer | YYYY-MM-DD   |
| Asset Inventory              | Track hardware, software and ownership                 | 3 years            | Managing Director   | YYYY-MM-DD   |
| Change Control Log           | Track changes in production systems with approvals     | 3 years            | Team Lead Developer | YYYY-MM-DD   |
| Endpoint Patch/Update Log    | Prove system vulnerabilities are managed               | 1 year             | Team Lead Developer | YYYY-MM-DD   |
| Risk Assessment Report       | Documented risk identification and analysis            | 3 years            | Managing Director   | YYYY-MM-DD   |
| Restore Drill Checklist      | Validate that backup recovery is documented and tested | 1 year             | Team Lead Developer | YYYY-MM-DD   |
| Device Offboarding Checklist | Confirm access revoked and assets returned             | 3 years            | Managing Director   | YYYY-MM-DD   |

---

## 1. Training Completion Log  
**Purpose:** Confirm annual employee awareness training  
**Retention:** 3 years  
**Owner:** Managing Director  

| Date       | Employee Name     | Training Module        | Status   | Notes               | Link                                             |
|------------|------------------|------------------------|----------|---------------------|--------------------------------------------------|
| 2025-05-19 | Inge Proost       | Security Awareness 2025| Pending  | Confirm by email    | `Pending`      |
| 2025-05-19 | Firas Kassoumeh   | Security Awareness 2025| Pending  | Confirm by email    | `Pending`     |
| 2025-05-19 | Bassel Alkhateeb  | Security Awareness 2025| Pending  | Confirm by email    | `Pending`    |


---

## 2. Incident Response Log  
**Purpose:** Track security events and responses  
**Retention:** 3 years  
**Owner:** Managing Director  

| Incident ID  | Date       | Description                              | Severity | Response Summary                            | Status | Link                                                                                  |
|--------------|------------|------------------------------------------|----------|----------------------------------------------|--------|---------------------------------------------------------------------------------------|
| IR-2025-001  | 2025-01-27 | Customer data overwritten due to session conflict | Medium   | Data restored; safeguards planned             | Closed | [Incident Report](https://docs.google.com/document/d/1qPG9Pe-GH_z7szprc42ms2sIN_t3KYaUsw6GKezd5zk/edit?tab=t.0#heading=h.epb41kpmjny7) |
| IR-2023-001  | 2023-03-03 | Web crawler activity causing abnormal traffic      | Normal   | Investigation done; continued monitoring      | Closed | [Incident Report](https://docs.google.com/document/d/15sr1S8co-Eznn-npCsZYK-JQo8gfgqouN0Stac-YJPY/edit?tab=t.0)                      |

---

## 3. Access Control Review Record  
**Purpose:** Review of user permissions and updates  
**Retention:** 3 years  
**Owner:** Team Lead Developer  

| Review Date | System | Users Reviewed | Findings                | Action Taken    | Link                         |
|:------------|:-------|:---------------|:------------------------|:----------------|:-----------------------------|
| YYYY-MM-DD  | GitHub | 12             | 2 inactive accounts     | Removed access  | `/evidence/access/review1.md` |

---

## 4. DB Restore Test Log  
**Purpose:** Confirm successful backup recovery tests  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Test Date  | Database   | Tested By | Result   | Notes                    | Link                         |
|:-----------|:-----------|:----------|:---------|:-------------------------|:-----------------------------|
| YYYY-MM-DD | prod_db    | John Doe  | Success  | Restoration in 5 minutes | `/evidence/dbrestore/test1.md` |

---

## 5. Backup Job Reports  
**Purpose:** Proof of scheduled backup executions  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Report Date | Job Name       | Status    | Duration | Notes      | Link                         |
|:------------|:---------------|:----------|:---------|:-----------|:-----------------------------|
| YYYY-MM-DD  | DailyBackup001 | Completed | 15m      | No errors  | `/evidence/backups/rep1.md`  |

---

## 6. Asset Inventory  
**Purpose:** Track hardware, software and ownership  
**Retention:** 3 years  
**Owner:** Managing Director  

| Asset ID   | Type   | Description          | Owner             | Location | Link                         |
|:-----------|:-------|:---------------------|:------------------|:---------|:-----------------------------|
| ASSET-001  | Laptop | MD’s MacBook Pro     | Managing Director | Office   | `/evidence/assets/asset1.md` |

---

## 7. Change Control Log  
**Purpose:** Track changes in production systems with approvals  
**Retention:** 3 years  
**Owner:** Team Lead Developer
**Old Log** https://docs.google.com/spreadsheets/d/1aTAYJK-ycFjJh9wI8hkGKIsSFxHTPhW5TxiL7bMx1hA/edit?usp=sharing

| Change ID  | Date       | Description              | Requested By | Approval | Status   | Link                         |
|:-----------|:-----------|:-------------------------|:-------------|:---------|:---------|:-----------------------------|


---

## 8. Endpoint Patch/Update Log  
**Purpose:** Prove system vulnerabilities are managed  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Patch ID   | Date       | System        | Description     | Status  | Link                         |
|:-----------|:-----------|:--------------|:----------------|:--------|:-----------------------------|


---

## 9. Risk Assessment Report  
**Purpose:** Documented risk identification and analysis  
**Retention:** 3 years  
**Owner:** Managing Director  
**Old Risk assessments were managed within relevant trello cards**

| Assessment ID | Date       | Assessor      | Summary               | Status   | Link                         |
|:--------------|:-----------|:--------------|:----------------------|:---------|:-----------------------------|
| RA-2025-Q1    | YYYY-MM-DD | Managing Dir. | Identified 5 high risks | Complete | [Hetzner migration](`https://trello.com/c/PdvfZXPs`)    |

---

## 10. Restore Drill Checklist  
**Purpose:** Validate that backup recovery is documented and tested  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Drill ID   | Date       | Participants      | Outcome    | Notes               | Link                         |
|:-----------|:-----------|:------------------|:-----------|:--------------------|:-----------------------------|
| DRILL-001  | 10-01-2025 | Developers    | Successful | Met 4-hour RTO goal | [Hetzner migration](https://trello.com/c/PdvfZXPs)  |

---

## 11. Device Offboarding Checklist  
**Purpose:** Confirm access revoked and assets returned  
**Retention:** 3 years  
**Owner:** Managing Director  

| Offboard ID | Date       | Employee Name | Assets Returned        | Access Revoked | Notes     | Link                         |
|:------------|:-----------|:--------------|:-----------------------|:---------------|:----------|:-----------------------------|
| OFF-2025-01 | YYYY-MM-DD | John Smith    | Laptop, Badge, Phone   | Yes            | Completed | `/evidence/offboard/off1.md` |

