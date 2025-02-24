# **Statement of Applicability (SoA)**  

## **1. Introduction**  

### **1.1 Purpose of the SoA**  
The **Statement of Applicability (SoA)** defines the security controls selected and applied within **Rate’s Information Security Management System (ISMS)**. It ensures alignment with **ISO/IEC 27001:2022** requirements and justifies the inclusion or exclusion of Annex A controls based on **Rate’s risk assessment and business needs**.  

This document:  
- **Identifies** applicable **Annex A** controls from ISO/IEC 27001:2022.  
- **Provides justification** for the inclusion or exclusion of each control.  
- **Maps** selected controls to **Rate’s policies and procedures**.  
- **Assigns** responsibility for each control’s implementation and maintenance.  

The SoA is a **living document** reviewed and updated **annually** or when significant changes occur in **risk landscape, technology, or business processes**.  

---

### **1.2 Scope of Applicability**  
The SoA applies to **all information security policies, processes, systems, and assets** within Rate’s ISMS scope, including:  
- **Cloud Infrastructure:** Servers, databases, and backup solutions on Hetzner.  
- **Internal Networks & Systems:** NAS, Development Server, VPN, and access control mechanisms.  
- **Cloud Applications & Services:** Google Workspace, GitHub, LastPass, Exact Online, and project management tools.  
- **Physical Security:** Office premises, secured access, and asset management procedures.  
- **Personnel:** All employees, contractors, and third-party service providers.  

The SoA ensures that selected controls **effectively mitigate risks** identified in the **Risk Assessment and Risk Treatment Plan (RARTP)**.  

---

### **1.3 Reference to ISO/IEC 27001:2022**  
This SoA follows **ISO/IEC 27001:2022** standards and aligns with its **Annex A** controls. It is linked directly to **Rate’s Risk Assessment and Risk Treatment Plan (RARTP)**, ensuring a **risk-driven approach** to control implementation.  

---

## **2. Risk-Based Control Selection**  

### **2.1 Overview of Risk Assessment and Treatment Approach**  
Rate adopts a **risk-driven approach** to selecting and implementing security controls. The **Risk Assessment and Risk Treatment Plan (RARTP)** outlines risks to **information assets, infrastructure, personnel, and cloud environments**.  

The following principles guide the **control selection process**:  
- **Risk-Based Decision Making:** Controls are selected based on their ability to **mitigate identified risks**.  
- **ISO 27001 Annex A Alignment:** Controls map directly to **Annex A** where applicable.  
- **Business Impact Consideration:** High-impact risks receive **priority treatment** in control implementation.  
- **Regulatory & Compliance Alignment:** Controls support compliance with **ISO 27001, GDPR, and internal policies**.  
- **Cost vs. Security Balance:** Controls are selected to provide **effective security without unnecessary overhead**.  

---

### **2.2 Criteria for Selecting and Justifying Controls**  
The following criteria determine whether an **Annex A control is applicable**:  
- **Is the risk applicable to Rate’s ISMS scope?**  
- **Does the control address an identified risk in the RARTP?**  
- **Is the control required by legal, regulatory, or contractual obligations (e.g., GDPR)?**  
- **Does the control enhance existing security measures without excessive cost or complexity?**  

For **excluded controls**, a **justification** is provided based on **low risk, alternative controls, or business irrelevance**.  

---

### **2.3 Mapping to Risk Assessment and Risk Treatment Plan**  
Each selected control is **mapped to risks identified in the RARTP**. The table below provides an example of this **mapping methodology**:  

| **Annex A Control** | **Related Risk (RARTP)** | **Risk Owner** | **Control Implementation** |
|--------------------|----------------------|-------------|---------------------|
| A.9 Access Control | Unauthorized database access | Tech Lead Developer | Role-Based Access Control (RBAC), MFA for cloud services |
| A.12 Backup Policy | Data loss from server crash | Team Lead Developer | Daily NAS & cloud backups, monthly integrity testing |
| A.16 Incident Management | Malware attack on company devices | Managing Director | Security incident response plan, endpoint protection |
| A.17 Business Continuity | Production server failure | Team Lead Developer | Disaster Recovery Plan (DRP), failover provisioning |

This **mapping approach** ensures controls are **directly linked** to identified risks, aligning **ISMS policies** with security objectives.  

---
