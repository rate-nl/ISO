# **Statement of Applicability (SoA)**

## **1. Introduction**

### **1.1 Purpose**
The **Statement of Applicability (SoA)** defines the security controls selected and applied within **Rate’s Information Security Management System (ISMS)**. It ensures alignment with **ISO/IEC 27001:2022** and provides justification for the inclusion or exclusion of Annex A controls.

This document:
- Identifies applicable **Annex A** controls from ISO/IEC 27001:2022.
- Provides justification for inclusion or exclusion.
- Maps selected controls to **Rate’s Risk Assessment and Risk Treatment Plan (RTP)**.
- Assigns responsibility for control implementation and maintenance.

### **1.2 Scope**
This SoA applies to **all information security policies, processes, systems, and assets** within Rate’s ISMS scope, including:
- **Cloud Infrastructure:** Servers, databases, backups on Hetzner.
- **Internal Networks & Systems:** NAS, VPN, access control mechanisms.
- **Cloud Applications & Services:** Google Workspace, GitHub, LastPass, Exact Online.
- **Personnel:** Employees, contractors, and third-party service providers.

The SoA ensures that selected controls effectively mitigate risks identified in the **Risk Assessment and Risk Treatment Plan (RTP)**.

---

## **2. Applicable ISO 27001:2022 Controls**

The following controls are **selected** as they address specific security risks identified in the **Risk Assessment and Risk Treatment Plan (RTP)**.

| **Annex A Control** | **Control Description** | **Justification** | **Related Policy/Process** | **Responsible Role** |
|--------------------|----------------------|-----------------|--------------------|------------------|
| **A.5 Information Security Policies** | Establishes security policies aligned with ISO 27001. | Required for ISMS governance and compliance. | Information Security Policy | CEO |
| **A.6 Organization of Information Security** | Defines security roles and responsibilities. | Ensures accountability and security governance. | ISMS Roles & Responsibilities | CEO, Managing Director |
| **A.7 Human Resource Security** | Covers security awareness and employee lifecycle controls. | Reduces insider threats and enforces security training. | Security Awareness Training | Managing Director |
| **A.8 Asset Management** | Identifies, classifies, and protects information assets. | Prevents data loss and unauthorized access. | Asset Management Policy | Managing Director, Team Lead Developer |
| **A.9 Access Control** | Implements Role-Based Access Control (RBAC), authentication, and authorization. | Protects against unauthorized access. | Access Control Policy | Tech Lead Developer |
| **A.10 Cryptography** | Ensures encryption of sensitive data (e.g., passwords, backups). | Protects confidentiality and integrity of stored and transmitted data. | Secure Encryption Standards | Team Lead Developer |
| **A.11 Physical and Environmental Security** | Protects physical access to critical assets (office, NAS, servers). | Prevents unauthorized access to hardware. | Physical Security Measures | Managing Director |
| **A.12 Operations Security** | Ensures secure system administration, logging, and patch management. | Prevents system vulnerabilities and unauthorized system changes. | Backup & Patch Management Policy | Team Lead Developer |
| **A.13 Communications Security** | Secures internal and external communications (VPN, encrypted email). | Protects data in transit against interception. | Secure Communication Standards | Tech Lead Developer |
| **A.14 System Acquisition, Development, and Maintenance** | Applies security best practices in software development. | Prevents vulnerabilities in software. | Secure Development Practices | Team Lead Developer |
| **A.15 Supplier Relationships** | Ensures security in third-party and vendor agreements. | Mitigates supply chain risks. | Supplier Security Policy | Managing Director |
| **A.16 Information Security Incident Management** | Defines incident response, reporting, and resolution procedures. | Ensures a structured response to security incidents. | Incident Management and Response Plan | Managing Director |
| **A.17 Business Continuity Management** | Ensures business continuity planning and disaster recovery. | Maintains availability of critical services. | Business Continuity & Disaster Recovery Plan | CEO, Managing Director |
| **A.18 Compliance** | Ensures legal, regulatory, and contractual compliance. | Aligns ISMS with GDPR, ISO 27001, and other regulations. | Compliance Monitoring & Legal Requirements | CEO |

---

## **3. Justification for Control Exclusions**
Some **ISO 27001 Annex A controls** are **excluded** because they are **not applicable** to Rate’s ISMS scope. These exclusions are justified as follows:

| **Excluded Control** | **Justification** |
|---------------------|------------------|
| **A.14.2.9 - Outsourced Development** | Rate does **not** outsource development; all software development is done in-house. |
| **A.10.1.1 - Key Management** | Rate does **not** operate a large-scale PKI or issue digital certificates. |
| **A.11.2.6 - Secure Disposal of Media** | Rate operates entirely cloud-based, meaning no physical media is used for sensitive data storage. |

The **exclusions** are documented to ensure **compliance with ISO 27001:2022**.

---

## **4. Control Review and Updates**
The **Statement of Applicability (SoA)** is reviewed and updated:
- **Annually** or **whenever significant changes occur** in **technology, business processes, or risk landscape**.
- **During internal audits** as part of Rate’s **Continuous Improvement Process**.
- **When new risks are identified** that require control modifications.
- **Upon regulatory changes** affecting information security compliance (**e.g., GDPR updates**).

### **Approval and Versioning**
- **Reviewed by:** Managing Director  
- **Approved by:** CEO  
- **Last Review Date:** [Insert Date]  
- **Next Scheduled Review:** [Insert Date]  

---

This **minimal SoA** ensures **ISO 27001:2022 compliance** while remaining **concise and relevant** to your ISMS and RTP.
