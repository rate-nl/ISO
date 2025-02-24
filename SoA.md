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

# **4. Justification for Control Inclusion and Exclusion**

## **4.1 Control Inclusion Criteria**
The selection of controls from **ISO/IEC 27001:2022 Annex A** is based on a **risk-based approach**, ensuring that Rate implements security measures that **effectively mitigate risks** identified in the **Risk Assessment and Risk Treatment Plan (RARTP)**.

A control is **included** if it meets one or more of the following criteria:
- **Addresses an identified risk** in Rate’s **Risk Assessment and Risk Treatment Plan (RARTP)**.
- **Required for compliance** with **ISO 27001:2022**, **GDPR**, or **contractual obligations**.
- **Enhances Rate’s overall security posture**, even if not explicitly required by regulations.
- **Supports business continuity** by preventing or mitigating potential security incidents.
- **Aligns with Rate’s information security objectives**, ensuring confidentiality, integrity, and availability.

---

## **4.2 Summary of Included Controls**
The following **Annex A controls** are **included** because they **address specific security risks** and align with **Rate’s security objectives**:

| **Annex A Control** | **Reason for Inclusion** | **Related Risk (RARTP)** | **Responsible Role** |
|--------------------|----------------------|-----------------|------------------|
| **A.5 Information Security Policies** | Establishes and maintains ISMS policies. | Lack of defined security policies | CEO |
| **A.6 Organization of Information Security** | Defines security responsibilities and governance. | Undefined roles and responsibilities | CEO, Managing Director |
| **A.7 Human Resource Security** | Ensures security awareness and controls for employees. | Insider threats and unauthorized access | Managing Director |
| **A.8 Asset Management** | Identifies, classifies, and protects assets. | Unauthorized access, loss, or misuse of assets | Managing Director, Team Lead Developer |
| **A.9 Access Control** | Implements Role-Based Access Control (RBAC), authentication, and authorization. | Unauthorized database or system access | Tech Lead Developer |
| **A.10 Cryptography** | Ensures encryption of sensitive data (e.g., passwords, backups). | Data breach or exposure of sensitive information | Team Lead Developer |
| **A.11 Physical and Environmental Security** | Protects office access, NAS, and development servers. | Unauthorized physical access to sensitive data | Managing Director |
| **A.12 Operations Security** | Ensures secure system administration, patch management, and logging. | System vulnerabilities and outdated software | Team Lead Developer |
| **A.13 Communications Security** | Secures network communications (VPN, encrypted email). | Data interception and MITM attacks | Tech Lead Developer |
| **A.14 System Acquisition, Development, and Maintenance** | Ensures secure software development practices. | Application security vulnerabilities | Team Lead Developer |
| **A.15 Supplier Relationships** | Ensures security in vendor and third-party agreements. | Third-party risks and data leaks | Managing Director |
| **A.16 Information Security Incident Management** | Defines procedures for handling security incidents. | Lack of structured response to security breaches | Managing Director |
| **A.17 Business Continuity Management** | Ensures business continuity and disaster recovery planning. | System failures or cloud provider outages | CEO, Managing Director |
| **A.18 Compliance** | Ensures compliance with legal and regulatory requirements. | GDPR and ISO 27001 non-compliance risks | CEO |

These controls are **implemented through Rate’s ISMS policies**, including:
- **Information Security Policy**
- **Access Control Policy**
- **Incident Management and Response Plan**
- **Business Continuity and Disaster Recovery Plan**
- **Asset Management and Data Protection Policy**

---

## **4.3 Justification for Control Exclusions**
Certain **Annex A controls** are **excluded** from Rate’s ISMS scope due to **business irrelevance, alternative mitigations, or lack of risk applicability**. Exclusions are **documented and justified** to comply with **ISO 27001 certification requirements**.

| **Excluded Control** | **Justification** | **Alternative Mitigation (If Applicable)** |
|---------------------|------------------|----------------------------|
| **A.14.2.9 - Outsourced Development** | Rate does **not** outsource development activities. | Internal development team follows **Secure Development Practices**. |
| **A.10.1.1 - Key Management** | Rate does **not** manage large-scale cryptographic keys (e.g., PKI). | Passwords and encryption keys are **secured in LastPass** with MFA. |
| **A.11.2.6 - Secure Disposal of Media** | Rate does **not** store sensitive data on physical media. | All data is **cloud-based**, and decommissioned hardware is securely wiped. |

Rate **continuously reviews** security risks and **may re-evaluate exclusions** if new threats emerge or **business needs change**.

---

## **4.4 Continuous Review and Update of Control Applicability**
To maintain **ISMS effectiveness**, Rate ensures that the **Statement of Applicability (SoA) is reviewed and updated**:
- **Annually** or **whenever significant changes occur** in **technology, business processes, or regulations**.
- **During internal audits** as part of Rate’s **Continuous Improvement Process**.
- **When new risks are identified** that require control modifications.

**Approval and Versioning:**
- **Reviewed by:** Managing Director  
- **Approved by:** CEO  
- **Last Review Date:** [Insert Date]  
- **Next Scheduled Review:** [Insert Date]  

---

# **5. Control Mapping and Implementation Responsibility**

## **5.1 Overview**
This section provides a **detailed mapping of applicable Annex A controls** to Rate’s **policies, processes, and responsible roles**. Each control is aligned with **implementation mechanisms**, ensuring that security measures are properly assigned and managed.

---

## **5.2 Control Implementation Responsibility Matrix**

| **Annex A Control** | **Implementation Responsibility** | **Related Policy/Procedure** | **Supporting Systems** |
|--------------------|-------------------------------|---------------------------|----------------------|
| **A.5 Information Security Policies** | CEO | Information Security Policy | ISMS Documentation |
| **A.6 Organization of Information Security** | CEO, Managing Director | ISMS Roles & Responsibilities | ISMS Documentation |
| **A.7 Human Resource Security** | Managing Director | Security Awareness Training | Employee Training Records |
| **A.8 Asset Management** | Managing Director, Team Lead Developer | Asset Management & Data Protection Policy | Asset Inventory, Google Drive |
| **A.9 Access Control** | Tech Lead Developer | Access Control Policy | VPN, Google Workspace, LastPass |
| **A.10 Cryptography** | Tech Lead Developer | Secure Encryption Standards | Google Workspace, GitHub |
| **A.11 Physical and Environmental Security** | Managing Director | Physical Security Measures | NAS, Locked Development Server |
| **A.12 Operations Security** | Team Lead Developer | Backup & Patch Management Policy | Hetzner Cloud, NAS |
| **A.13 Communications Security** | Tech Lead Developer | Secure Communication Standards | VPN, Google Workspace |
| **A.14 System Acquisition, Development, and Maintenance** | Team Lead Developer | Secure Development Practices | GitHub, Code Repositories |
| **A.15 Supplier Relationships** | Managing Director | Supplier Security Policy | Vendor Contracts |
| **A.16 Information Security Incident Management** | Managing Director | Incident Management and Response Plan | Incident Logs, Google Drive |
| **A.17 Business Continuity Management** | CEO, Managing Director | Business Continuity and Disaster Recovery Plan | NAS, Google Drive, Hetzner Cloud |
| **A.18 Compliance** | CEO | Compliance Monitoring & Legal Requirements | ISMS Documentation |

- **Primary Owners:** Each control has a **primary responsible party** ensuring that it is implemented and maintained.
- **Supporting Policies:** Controls are mapped to **existing policies** to demonstrate compliance.
- **Supporting Systems:** Tools and technologies used to **enforce and monitor** the controls.

---

# **6. Continuous Monitoring and Review**

## **6.1 Overview**
To ensure **ongoing compliance** with **ISO 27001:2022**, Rate follows a structured **monitoring and review** process for all applicable controls. The **Statement of Applicability (SoA)** is **reviewed, updated, and audited** on a **regular basis**.

---

## **6.2 Review Frequency and Criteria**
The **Statement of Applicability (SoA)** is **formally reviewed:**
- **Annually** as part of Rate’s **ISMS internal audit process**.
- **After any major change** in **technology, business processes, or risk landscape**.
- **Following security incidents** that require **policy updates or control adjustments**.
- **Upon regulatory changes** affecting information security compliance (**e.g., GDPR updates**).

---

## **6.3 Monitoring of Controls**
Each applicable **Annex A control** is **continuously monitored** through:
- **Access Logs & Security Audits:** VPN, Google Workspace, NAS, and Hetzner Cloud.
- **Backup Integrity Checks:** Monthly and annual full validation.
- **Incident Response Reviews:** Post-incident analysis and remediation.
- **Physical Security Audits:** NAS and development server lock compliance.
- **Employee Awareness Training Records:** Verification of participation.

**Audit Documentation:**  
All **audit findings, corrective actions, and resolutions** are **recorded** in:
- **Google Drive (Audit Logs, Policy Updates)**
- **Incident Management Logs**
- **Security Training Reports**
- **Backup Testing Reports**

---

## **6.4 Non-Conformities and Corrective Actions**
If **non-conformities** are identified during an **internal audit** or **external ISO certification assessment**, Rate will:
1. **Document the issue** in the **Corrective Actions Log**.
2. **Assign responsibility** for remediation (CEO or Managing Director).
3. **Implement corrective actions** within a defined timeframe.
4. **Reassess compliance** after remediation is completed.

---

# **7. Approval and Versioning**

## **7.1 Approval and Ownership**
The **Statement of Applicability (SoA)** is formally **approved** and maintained by **Rate’s top management**.

- **Document Owner:** CEO
- **Review Authority:** Managing Director
- **Implementation Oversight:** Team Lead Developer

---

## **7.2 Version Control and Recordkeeping**
The **SoA document is version-controlled**, ensuring that all updates are **properly documented**.

| **Version** | **Date** | **Change Description** | **Approved By** |
|------------|---------|----------------------|---------------|
| **1.0** | [Initial Date] | Initial draft | CEO |
| **1.1** | [Update Date] | Updated Annex A mapping | CEO |
| **1.2** | [Update Date] | Added continuous monitoring section | CEO |

- **Retention Policy:** SoA versions are **retained for 3 years** for audit purposes.
- **Storage Location:** Google Drive (ISO Documentation Folder).
- **Access Control:** Restricted to **CEO, Managing Director, and Team Lead Developer**.

---

## **7.3 Next Scheduled Review**
- **Next Review Date:** [Insert Date]
- **Reviewer:** Managing Director
- **Purpose:** Annual review and updates based on new risks, incidents, and compliance changes.

---
