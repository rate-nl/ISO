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
| CrowdSec Monitoring Log   | Detect threats (port scans, brute-force, etc.) | 3 year         | Team Lead Developer    | Annually  | 30 minutes  |
| Alternative Access Method Test | Validate ability to access production servers using Hetzner console and manual firewall IP update | 1 year | Team Lead Developer | Annually or after network change | 15 minutes |



---

## 1. Training Completion Log

**Purpose:** Confirm completion of combined **Security Awareness Training** and **ISMS Management Awareness Session** for 2025. Given Rate's small team size, both sessions were merged into a single training and delivered in one meeting.

**Retention:** 3 years
**Owner:** Managing Director

| Date       | Employee Name    | Training Module                | Status      | Notes                     | Link                                                                                                                                                                                                                                     |
| ---------- | ---------------- | ------------------------------ | ----------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2025-05-20 | Inge Proost      | Security + ISMS Awareness 2025 | ✅ Completed | See MoM & materials below | [Minutes](https://docs.google.com/document/d/1icjVU979pQZrNTgcScfVoTWJKHIZbYxIfz-RaKfFWHQ/edit?tab=t.0#heading=h.gsg0462khpl), [Materials](https://docs.google.com/document/d/1aTxQP5pj_n1xqduZj4EwyiqsfY3rcI7aY18_ee-SKQA/edit?tab=t.0) |
| 2025-05-20 | Firas Kassoumeh  | Security + ISMS Awareness 2025 | ✅ Completed | See MoM & materials below | [Minutes](https://docs.google.com/document/d/1icjVU979pQZrNTgcScfVoTWJKHIZbYxIfz-RaKfFWHQ/edit?tab=t.0#heading=h.gsg0462khpl), [Materials](https://docs.google.com/document/d/1aTxQP5pj_n1xqduZj4EwyiqsfY3rcI7aY18_ee-SKQA/edit?tab=t.0) |
| 2025-05-20 | Bassel Alkhateeb | Security + ISMS Awareness 2025 | ✅ Completed | See MoM & materials below | [Minutes](https://docs.google.com/document/d/1icjVU979pQZrNTgcScfVoTWJKHIZbYxIfz-RaKfFWHQ/edit?tab=t.0#heading=h.gsg0462khpl), [Materials](https://docs.google.com/document/d/1aTxQP5pj_n1xqduZj4EwyiqsfY3rcI7aY18_ee-SKQA/edit?tab=t.0) |


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
| 2025-02-20  | 6              | Suhail Sakhizadh left, access no longer needed | Access revoked   | [Review Document](https://docs.google.com/document/d/1GfA3R8gUsjzp-ethsc6uStHqIxs00M3Bz6rT269_Mrs/edit?usp=drive_link) |
| 2025-04-30  | 5              | Ricardo Keus left, access no longer needed     | Access revoked   | [Review Document](https://docs.google.com/document/d/167eYbklP_rwdDb2xfGFF3Rff8ztmD8x-S4gsfpR1-Ig/edit?usp=drive_link) |
| 2025-06-30  | 4              | Younes Shina left, access no longer needed     | Access revoked   | [Review Document](https://docs.google.com/document/d/15MG6e8FEyScGgtp2Z4UrARt_XLwgUnFWjwGUF-iaa-w/edit?usp=drive_link) |
| 2025-07-10  | 3              | Annual review, all current access valid        | No action needed | [Review Document](https://docs.google.com/document/d/1wKoK-Bx0WtrgXlnWCtZZbh0e6dKL4ockuB7z3MI3nfY/edit?usp=drive_link) |
| 2025-07-10  | 3              | Bassel Alkhateeb left, access no longer needed        | Access revoked | [Review Document](https://docs.google.com/document/d/1YJJGUH13eCq4EjNuuxK3dhFxqGSmlvyn1-hlck4ciiA/edit?tab=t.0) |


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
| 2025-06-11  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB     | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-07-10  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB     | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |
| 2025-08-12  | prod_db_test | Firas Kassoumeh | Success | Manual restore to test DB     | [Screenshot](https://drive.google.com/drive/folders/1GmgUvBjcJPJz7uHGvbFHhH6pUHFmn3Lu) |




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
**Change Management Log** https://docs.google.com/spreadsheets/d/1aTAYJK-ycFjJh9wI8hkGKIsSFxHTPhW5TxiL7bMx1hA/edit?usp=sharing


---

## 7. Endpoint Patch/Update Log  
**Purpose:** Prove system vulnerabilities are managed  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Patch ID     | Date       | System      | Description                                                                                  | Status   | Link                                                                                                   |
|--------------|------------|-------------|----------------------------------------------------------------------------------------------|----------|--------------------------------------------------------------------------------------------------------|
| SEC-2025-003 | 2025-07-02 | Dev Server  | Automatic updates applied: KB5001716, KB5060533, KB5058379, KB5057056, KB5055683, KB5055518  | ✅ Done | [Update Screenshot](https://drive.google.com/file/d/1NLQs2yoWaTEsjjweUqAM-2IyP5zgTLfF/view?usp=drive_link) |

> **Note:** Automatic updates are enabled on this server. Patch history is verified annually via Windows Update History screenshots . Screenshot evidence is stored in Google Drive.


---

## 8. Risk Assessment Report  
**Purpose:** Documented risk identification and analysis  
**Retention:** 3 years  
**Owner:** Managing Director  
**Old Risk assessments were managed within relevant trello cards**

| Assessment ID | Date       | Assessor           | Summary                                                       | Status   | Link                                               |
|---------------|------------|--------------------|---------------------------------------------------------------|----------|----------------------------------------------------|
| RA-2025-001   | 2025-06-17 | Firas Kassoumeh     | Risk assessment for migrating production servers to Hetzner. Risks included data loss, downtime, compatibility, and security. Mitigations documented. | ✅ Closed | [Trello: Hetzner Migration Risk](https://trello.com/c/PdvfZXPs) |

---

## 9. Restore Drill Checklist  
**Purpose:** Validate that backup recovery is documented and tested  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Drill ID   | Date       | Participants      | Outcome    | Notes               | Link                         |
|:-----------|:-----------|:------------------|:-----------|:--------------------|:-----------------------------|
| DRILL-001  | 10-01-2025 | Team lead , Developers    | Successful | Met 4-hour RTO goal | [Hetzner migration](https://trello.com/c/PdvfZXPs)  |
| DRILL-002  | 29-07-2025 | CEO, Team lead    | Successful | Met 4-hour RTO goal | [Business Continuity & Disaster Recovery Drill Report](https://docs.google.com/document/d/10gqrAy8atvssXkNBAlIAWsQb5nvZivrszV974V0S1u4/edit?tab=t.0)  |


---

## 10. Device Offboarding Checklist  
**Purpose:** Confirm access revoked and assets returned  
**Retention:** 3 years  
**Owner:** Managing Director
**Access grants and revokes are maintained within EXACT software and managed by the managing director**

## 11. CrowdSec Monitoring Log

**Purpose:** Detect and block intrusion attempts, port scans, and other server-level threats using CrowdSec.

**Retention:** 1 year  
**Owner:** Team Lead Developer

| Log ID   | Date       | System        | Detected Threats                | Action Taken           | Link                                     |
|----------|------------|----------------|----------------------------------|------------------------|------------------------------------------|
| CSEC-001 | 2025-07-14 | Production     | 0 brute-force attempts blocked | IPs banned automatically | [CrowdSec Report](https://drive.google.com/file/d/1ezrkXcxCGAwg8tC8z4s_orQlk4hRmS0i/view?usp=sharing) |


## 12. Alternative Access Method Test Log

**Purpose:** Confirm ability to access production servers when primary network (e.g., office internet) is unavailable. Ensures resilience through console access and external firewall control.  
**Retention:** 1 year  
**Owner:** Team Lead Developer  

| Test ID      | Date       | Method Used                                      | Result     | Notes                                                                                                 | Evidence Link                                                                                     |
|--------------|------------|--------------------------------------------------|------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ALT-2025-001 | 2025-08-25 | Hetzner console access + manual IP whitelist for RDP | ✅ Success | Simulated office internet outage. Used mobile hotspot. Accessed Hetzner console, added IP to firewall, verified RDP access. | [Screenshot](https://drive.google.com/file/d/13Bzt_BORRn0bEKqXy1DE6XisBaL_T9-w/view?usp=drive_link) , [Screenshot](https://drive.google.com/file/d/1hyfHDD3tsLjLTyFirXoN6oA5RJIup1o_/view?usp=drive_link)| 

