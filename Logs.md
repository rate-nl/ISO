# ISMS Evidence & Logs

_A single file to capture and track all required ISMS evidence in one place._

---

## Summary Table

| Evidence Title               | Purpose                                                | Retention Period | Responsible Owner     | Frequency                              | Estimated Time           |
|-----------------------------|--------------------------------------------------------|------------------|------------------------|-----------------------------------------|--------------------------|
| Training Completion Log      | Confirm annual employee awareness training             | 3 years          | Managing Director      | Annually                                | 1 hour                   |
| Incident Response Log        | Track security events and responses                    | 3 years          | Managing Director      | After each incident + Annual review     | 30 minutes per incident  |
| Access Control Review Record | Review of user permissions and updates                 | 3 years          | Team Lead Developer    | Annually                                | 1 hour                   |
| DB Restore Test Log          | Confirm successful backup recovery tests               | 1 year           | Team Lead Developer    | Monthly + Annually                      | 1 hour                   |
| Asset Inventory              | Track hardware, software and ownership                 | 3 years          | Managing Director      | Annually                                | 2 hours                  |
| Change Control Log           | Track changes in production systems with approvals     | 3 years          | Team Lead Developer    | Per change                              | 10 minutes per entry     |
| Endpoint Patch/Update Log    | Prove system vulnerabilities are managed               | 1 year           | Team Lead Developer    | Monthly                                 | 30 minutes               |
| Risk Assessment Report       | Documented risk identification and analysis            | 3 years          | Managing Director      | After major change                      | 2 hours                  |
| Restore Drill Checklist      | Validate that backup recovery is documented and tested | 1 year           | Team Lead Developer    | Annually                                | 1 hour                   |
| Device Offboarding Checklist | Confirm access revoked and assets returned             | 3 years          | Managing Director      | Per offboarding                         | 15 minutes per employee  |


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

| Review Date | Users Reviewed | Findings                                      | Action Taken     | Link                                                                 |
|:------------|----------------|-----------------------------------------------|------------------|----------------------------------------------------------------------|
| 2025-01-15  | 6              | All access valid and aligned with roles       | No action needed | [Review Document](https://docs.google.com/document/d/1Q85vPlBdjrNonck1D5RbVWWLV86JbY6f0dcBgCFLygE/edit?tab=t.0) |


---

## 4. DB Restore Test Log  
**Purpose:** Confirm successful backup recovery tests  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Test Date   | Database     | Tested By       | Result  | Notes                              | Link                                                                 |
|-------------|--------------|-----------------|---------|------------------------------------|----------------------------------------------------------------------|
| 2025-01-07  | prod_db      | Firas Kassoumeh | Success | Verified during production migration | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-02-15  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB          | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-03-28  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB     | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-04-12  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB  | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-05-13  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB     | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |




---

## 5. Asset Inventory  
**Purpose:** Track hardware, software and ownership  
**Retention:** 3 years  
**Owner:** Managing Director  
**Hardware and Software assets** [Link](https://docs.google.com/spreadsheets/d/1pTpcCb0NRaoKwHqVUfqojYlkyGQRnSVEPFTyKMASNBg/edit?usp=sharing)

---

## 6. Change Control Log  
**Purpose:** Track changes in production systems with approvals  
**Retention:** 3 years  
**Owner:** Team Lead Developer
**Old Log** https://docs.google.com/spreadsheets/d/1aTAYJK-ycFjJh9wI8hkGKIsSFxHTPhW5TxiL7bMx1hA/edit?usp=sharing

| Change ID  | Date       | Description              | Requested By | Approval | Status   | Link                         |
|:-----------|:-----------|:-------------------------|:-------------|:---------|:---------|:-----------------------------|


---

## 7. Endpoint Patch/Update Log  
**Purpose:** Prove system vulnerabilities are managed  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Patch ID   | Date       | System        | Description     | Status  | Link                         |
|:-----------|:-----------|:--------------|:----------------|:--------|:-----------------------------|


---

## 8. Risk Assessment Report  
**Purpose:** Documented risk identification and analysis  
**Retention:** 3 years  
**Owner:** Managing Director  
**Old Risk assessments were managed within relevant trello cards**

| Assessment ID | Date       | Assessor      | Summary               | Status   | Link                         |
|:--------------|:-----------|:--------------|:----------------------|:---------|:-----------------------------|

---

## 9. Restore Drill Checklist  
**Purpose:** Validate that backup recovery is documented and tested  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Drill ID   | Date       | Participants      | Outcome    | Notes               | Link                         |
|:-----------|:-----------|:------------------|:-----------|:--------------------|:-----------------------------|
| DRILL-001  | 10-01-2025 | Developers    | Successful | Met 4-hour RTO goal | [Hetzner migration](https://trello.com/c/PdvfZXPs)  |

---

## 10. Device Offboarding Checklist  
**Purpose:** Confirm access revoked and assets returned  
**Retention:** 3 years  
**Owner:** Managing Director
**Access grants and revokes are maintained within EXACT software and managed by the managing director**


