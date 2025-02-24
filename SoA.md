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
# **3. Summary of Applicable Annex A Controls**

## **3.1 Overview**  
This section outlines the **Annex A security controls** that are **applicable to Rate’s ISMS**. Each selected control is mapped to **relevant risks**, **policies**, and **responsible roles**.  

### **Control Selection Criteria:**  
- The control **addresses an identified risk** in the **Risk Assessment and Risk Treatment Plan (RARTP)**.  
- The control **supports compliance** with **ISO 27001:2022**, **GDPR**, or **business requirements**.  
- The control **aligns with Rate’s security objectives**, ensuring **confidentiality, integrity, and availability** of assets.  

---

## **3.2 List of Applicable Controls**  

| **Annex A Control** | **Control Description** | **Justification** | **Related Policy/Process** | **Responsible Role** |
|--------------------|----------------------|-----------------|--------------------|------------------|
| **A.5 Information Security Policies** | Establishes and maintains security policies aligned with ISO 27001. | Required for ISMS governance and compliance. | Information Security Policy | CEO |
| **A.6 Organization of Information Security** | Defines security responsibilities and internal governance. | Ensures clear accountability and roles. | ISMS Roles & Responsibilities | CEO, Managing Director |
| **A.7 Human Resource Security** | Ensures security awareness and controls for employee lifecycle (onboarding, termination). | Reduces insider threats and enhances security culture. | Security Awareness Training | Managing Director |
| **A.8 Asset Management** | Identifies, classifies, and protects information assets. | Ensures asset security and compliance. | Asset Management & Data Protection Policy | Managing Director, Team Lead Developer |
| **A.9 Access Control** | Implements Role-Based Access Control (RBAC), authentication, and authorization. | Protects against unauthorized access and privilege abuse. | Access Control Policy | Tech Lead Developer |
| **A.10 Cryptography** | Ensures secure encryption of sensitive data (e.g., passwords, backups). | Protects confidentiality and integrity of stored and transmitted data. | Secure Encryption Standards | Team Lead Developer |
| **A.11 Physical and Environmental Security** | Protects physical access to critical assets (office, NAS, Dev Server). | Prevents unauthorized physical access to company assets. | Physical Security Measures | Managing Director |
| **A.12 Operations Security** | Ensures secure system administration, monitoring, and patch management. | Prevents system vulnerabilities and ensures operational security. | Backup & Patch Management Policy | Team Lead Developer |
| **A.13 Communications Security** | Secures internal and external communications (VPN, encrypted email). | Protects data in transit against interception and tampering. | Secure Communication Standards | Tech Lead Developer |
| **A.14 System Acquisition, Development, and Maintenance** | Applies security best practices in software development. | Prevents vulnerabilities in developed software. | Secure Development Practices | Team Lead Developer |
| **A.15 Supplier Relationships** | Ensures security in third-party and vendor agreements. | Protects Rate from supply chain risks. | Supplier Security Policy | Managing Director |
| **A.16 Information Security Incident Management** | Defines security incident reporting, response, and resolution procedures. | Ensures a structured response to security breaches. | Incident Management and Response Plan | Managing Director |
| **A.17 Business Continuity Management** | Ensures business continuity planning and disaster recovery. | Maintains availability of critical services. | Business Continuity and Disaster Recovery Plan | CEO, Managing Director |
| **A.18 Compliance** | Ensures legal, regulatory, and contractual compliance with data protection laws. | Aligns ISMS with GDPR, ISO 27001, and industry regulations. | Compliance Monitoring & Legal Requirements | CEO |

---

## **3.3 Justification for Control Inclusion and Exclusion**  

### **3.3.1 Included Controls**  
The following controls are **included** as they **directly mitigate identified risks** in Rate’s **Risk Assessment and Risk Treatment Plan (RARTP)**:  
- **Access Control (A.9)** → Prevents unauthorized access.  
- **Backup & Disaster Recovery (A.17)** → Ensures business continuity.  
- **Incident Management (A.16)** → Provides structured response to security incidents.  
- **Operations Security (A.12)** → Protects against software vulnerabilities and unauthorized system changes.  

### **3.3.2 Excluded Controls**  
Some **ISO 27001 Annex A controls** are **excluded** because they are **not applicable** to Rate’s ISMS scope:  

| **Excluded Control** | **Reason for Exclusion** |
|---------------------|------------------------|
| **A.14.2.9 - Outsourced Development** | Rate does **not** outsource development activities. |
| **A.10.1.1 - Key Management** | Rate does **not** manage large-scale cryptographic keys (e.g., PKI). |
| **A.11.2.6 - Secure Disposal of Media** | All Rate data is **cloud-based** with no sensitive data stored on physical media. |

The **exclusions** are documented with **justifications** to ensure **compliance with ISO 27001:2022**.

---

