# Information Security Management System (ISMS) Manual  

## 1. Introduction

## 2. Core ISMS Documents
   - [Information Security Policy](#Information-Security-Policy)
   - [Risk Assessment and Risk Treatment Plan](##risk-assessment-and-risk-treatment-plan)
   - [Access Control Policy](#Access-Control-Policy)
   - [Incident Management and Response Plan](#Incident-Management-and-Response-Plan)
   - [Business Continuity and Disaster Recovery Plan](#Business-Continuity-and-Disaster-Recovery-Plan)
   - [Asset Management Policy](#Asset-Management-Policy)
   - [Secure Development & Change Management](#secure-development--change-management)


## 3. Statement of Applicability

## 4. Compliance & Security Governance
   - [Legal & Regulatory Compliance](#legal--regulatory-compliance)
   - [Privacy & Data Protection Policy](#privacy--data-protection-policy)
   - [Supplier Security & Contractual Obligations](#supplier-security--contractual-obligations)
   - [Internal Audit Program](#internal-audit-program)
   - [Corrective Actions & Non-Compliance Log](#corrective-actions--non-compliance-log)
   - [Management Review](#Management-Review)
   - [ISMS Performance Metrics](#ISMS-Performance-Metrics)
   - [Evidence & Logs](#Evidence-&-Logs)


---


## 1. Introduction

### Purpose and Objectives of the ISMS

Rate is committed to safeguarding the confidentiality, integrity, and availability of all physical and electronic information assets. Our Information Security Management System (ISMS) is designed to manage information security risks effectively, ensuring business continuity and minimizing potential threats.

## Scope of the ISMS

The ISMS encompasses all processes, systems, and personnel involved in the development, maintenance, and delivery of our survey platform services. This includes:

- **Physical Location:** Our office at Stationsplein 45 Unit D3.125, 3013 AK Rotterdam, Netherlands.
- **Assets:** Servers, databases, backups, company laptops, and network infrastructure.
- **Information:** Customer survey data and employee personal information.
- **Activities:** Data collection, processing, storage, and analysis related to customer surveys.


### Definitions and Abbreviations

- **ISMS**: Information Security Management System
- **Information Assets**: Data, systems, and processes vital to Rate's operations
- **Confidentiality**: Ensuring information is accessible only to authorized individuals
- **Integrity**: Maintaining the accuracy and completeness of information
- **Availability**: Ensuring information and resources are accessible when needed


---


# 2. Core ISMS Documents

# Information Security Policy

## 1. Purpose

The purpose of this Information Security Policy is to establish a framework for managing and protecting Rate's information assets, ensuring their confidentiality, integrity, and availability. This policy aligns with the requirements of ISO/IEC 27001:2022 and demonstrates our commitment to information security.

## 2. Scope

This policy applies to all employees, contractors, consultants, temporary staff, and any other personnel at Rate who have access to information assets. It encompasses all information systems, networks, applications, and data owned or managed by Rate.

## 3. Information Security Objectives

Rate is committed to the following measurable information security objectives:

- Maintain 100% completion rate for annual information security awareness training for all employees.
- Ensure all backups are tested monthly with a minimum 90% success rate.
- Limit unauthorized access incidents to zero per year.
- Review access permissions for all systems at least once per year.
- Complete annual internal ISMS audit and resolve 100% of non-conformities within 30 days.


## 4. Roles and Responsibilities

In accordance with ISO/IEC 27001:2022 Clause 5.3 and Annex A.5.2, the following roles and responsibilities are defined:

### 4.1. Chief Executive Officer (CEO)

- **Accountability**: Holds overall accountability for the ISMS.
- **Responsibilities**:
  - Ensure strategic alignment of the ISMS with business objectives.
  - Provide necessary resources for ISMS implementation and maintenance.
  - Promote a culture of information security within the organization.
  - Oversee compliance with regulatory and security standards.
  - Approve risk assessments and the Risk Treatment Plan (RTP).
  - Oversee **incident management and resolution** for critical security incidents.
  - Ensure periodic **reviews of security incidents and ISMS effectiveness**.
- **Competency Requirements**:
  - Understanding of information security governance and ISO 27001 principles.
  - Familiarity with legal, regulatory, and contractual obligations related to information security.
  - Experience in organizational risk management and executive decision-making.


### 4.2. Managing Director

- **Accountability**: Oversees the implementation and operation of the ISMS.
- **Responsibilities**:
  - Develop and maintain information security policies and procedures.
  - Conduct organization-wide risk assessments and manage risk treatment plans.
  - Ensure compliance with information security policies and applicable laws.
  - Report ISMS performance to top management.
  - Support operational security measures and access control strategies.
  - Review risk assessments before CEO approval.
  - Lead **incident response planning** and coordinate with affected teams.
  - Conduct **annual security reviews** and adjust strategies as needed.
  - Assign and review asset owners and ensure asset records are up to date and accurate.
- **Competency Requirements**:
  - Knowledge of ISO 27001 control implementation and audit preparation.
  - Skills in risk assessment, compliance monitoring, and incident management.
  - Completion of formal training on ISMS frameworks and regulatory compliance.

### 4.3. Team Lead Developer

- **Accountability**: Ensures secure software development practices and cybersecurity risk mitigation.
- **Responsibilities**:
  - Lead the development team in implementing secure coding practices and ensuring software security.
  - Enforce security policies within the software development lifecycle.
  - Conduct periodic code reviews and security assessments to identify vulnerabilities.
  - Manage and monitor security compliance related to development infrastructure.
  - Ensure **SSL certificate renewal** is managed through **automatic renewal or alerts**.
  - Investigate and provide technical remediation for **security incidents** affecting development environments.
  - Maintain security and availability of hardware and data assets under their ownership.
- **Competency Requirements**:
  - Experience with secure coding practices and vulnerability management.
  - Proficiency in access control principles and DevSecOps.
  - Completion of secure development lifecycle (SDLC) and information security training.


### 4.4. Developers

- **Accountability**: Implement secure coding practices and access controls.
- **Responsibilities**:
  - Follow secure coding standards and guidelines.
  - Enforce access control and authentication processes within the development environment.
  - Support security compliance by maintaining documentation and adhering to best practices.
  - Identify and report potential software vulnerabilities to the Team Lead Developer.
  - Assist in responding to security incidents by providing technical expertise and remediation support.
  - Implement and enforce **access control measures** in compliance with **Annex A.9**.
- **Competency Requirements**:
  - Knowledge of secure coding standards and access control.
  - Participation in annual security awareness training.
  - Ability to identify and report vulnerabilities.


### 4.5. All Employees

- **Accountability**: Adhere to information security policies and procedures.
- **Responsibilities**:
  - Protect information assets within their control.
  - Report security incidents or weaknesses promptly.
  - Participate in information security training and awareness programs.
- **Competency Requirements**:
  - Completion of onboarding and annual information security awareness training.
  - Understanding of how to report incidents and follow policies.


## 5. Information Security Principles

Rate adopts the following principles to guide its information security efforts:

- **Confidentiality**: Ensuring that information is accessible only to those authorized to have access.
- **Integrity**: Safeguarding the accuracy and completeness of information and processing methods.
- **Availability**: Ensuring that authorized users have access to information and associated assets when required.

## 6. Risk Management

Rate implements a structured risk management process based on ISO 27005, consisting of the following steps:

### 6.1 Risk Identification
- Identify threats and vulnerabilities that could affect information assets, services, and business processes.
- Document assets and associated risks in the risk register.

### 6.2 Risk Assessment
- **Likelihood and Impact Assessment:** Assess the likelihood and potential impact of each identified risk using a defined risk matrix.
- Assign a risk level (Low / Medium / High) for prioritization.

### 6.3 Risk Evaluation
- Compare risk levels against Rate’s **risk acceptance criteria**.
- Risks that exceed acceptable thresholds are escalated for treatment.

### 6.4 Risk Treatment
- Select one or more of the following options:
  - **Mitigate:** Apply security controls to reduce risk.
  - **Avoid:** Discontinue the activity causing the risk.
  - **Transfer:** Outsource the risk (e.g., through insurance or contracts).
  - **Accept:** Justify and document acceptance of the residual risk.
- Define and document mitigation actions in the **Risk Treatment Plan**.

### 6.5 Risk Monitoring and Review
- Risks are reviewed **annually** or after major changes/incidents.
- Effectiveness of controls is verified through internal audits and incident analysis.

### 6.6 Roles and Responsibilities
- **Managing Director:** Owns the risk management process.
- **CEO:** Approves risk assessments and treatment decisions.
- **Team Lead Developer:** Supports technical risk analysis and control implementation.

### 6.7 Documentation
- All risk activities are documented in:
  - **Risk Assessment Report**
  - **Risk Treatment Plan**
  - **Statement of Applicability (SoA)**


## 7. Access Control

In accordance with **Annex A.9 - Access Control**, Rate enforces the following security measures:

- **Role-based access control (RBAC)** is implemented for all systems.
- **Firewall rules and VPN access restrictions** are enforced to protect critical infrastructure.
- **Alternative access methods** to production servers are maintained to ensure availability in case of VPN failures.
- **Access Reviews**: All user access rights, including administrative access, are formally reviewed **annually** by the **Team Lead Developer** in coordination with the **Managing Director**.
- **Log Reviews**: System and access logs are reviewed **annually** for anomalies, with findings documented and reported during the management review.
- **Log Retention**: Access and system logs are retained for **one year**, aligning with compliance requirements and internal policies.

## 8. Compliance

Rate is committed to complying with all applicable legal, regulatory, and contractual requirements related to information security. This includes, but is not limited to, data protection laws and industry standards.

## 9. Incident Reporting and Response

In accordance with ISO/IEC 27001:2022 Clause 16.1.1, Rate has established a formal Incident Response Plan (IRP) that includes:

- **Incident Identification**: All employees are responsible for reporting suspected information security incidents immediately to the **Managing Director**.
- **Incident Escalation**: Significant incidents will be escalated to the **CEO** if necessary.
- **Incident Resolution**: The **Team Lead Developer** and relevant personnel will coordinate the response to and resolution of the incident.

## 10. Policy Review and Approval

In compliance with ISO/IEC 27001:2022 Clause 5.1.2, this Information Security Policy shall be:

- **Reviewed**: The **Managing Director** is responsible for reviewing this policy **at least annually** or when significant changes occur.
- **Approved**: The policy must be **approved by the Chief Executive Officer (CEO)** to ensure its relevance and effectiveness.


---
# Risk Assessment and Risk Treatment Plan

This document outlines the identified risks, their likelihood and impact, and the appropriate risk treatment actions in accordance with **ISO 27001:2022**.

---

## **1. Risk Categorization**

### **1.1 Data Security Risks**

| **Risk**                                | **Likelihood** | **Impact** | **Risk Owner**       | **Treatment Option** | **Mitigation Actions**                                                                                                                                         | **Annex A Reference** | **Risk Acceptance Criteria**                                             |
|-----------------------------------------|----------------|------------|----------------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------|---------------------------------------------------------------------------|
| **Unauthorized access to customer database** | Medium         | High       | Developers           | Mitigate             | Enforce strict **access controls** using a **firewall** and strong authentication mechanisms. Refer to the **Access Control Policy – Sections 3 & 4**.        | A.9 Access Control     | Acceptable if **strong passwords are enforced and the firewall is active**. |
| **Data loss from a server crash**       | Medium         | High       | Developers           | Mitigate             | Ensure **automatic backups** to NAS and **perform regular backup tests**. Refer to the **Business Continuity and Disaster Recovery Plan – Section 5.1**.      | A.12 Backup Policy     | Acceptable if **offsite backups are tested annually**.                    |
| **Insider threats (employee mishandling data)** | Low            | High       | Managing Director    | Mitigate             | Implement **role-based access control (RBAC)** and log all sensitive actions. Refer to the **Access Control Policy – Section 3** and **Incident Plan – Section 6**. | A.7 Human Resource Security | Acceptable if **RBAC is enforced & reviewed annually**.                   |

---

### **1.2 Infrastructure Risks**

| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions**                                                                                                                                               | **Annex A Reference**    | **Risk Acceptance Criteria**                                                            |
|----------|----------------|------------|----------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|------------------------------------------------------------------------------------------|
| **Server crash causing service disruption** | Medium         | High       | Developers         | Mitigate             | Implement **regular database and code backups**. Monitor server health and set **automated alerts**. Refer to the **BCDR Plan – Section 5.1 & 6.1**.                 | A.17 Business Continuity | Acceptable if **regular backups are performed and automatic alerts are configured**.     |
| **Losing physical or internet access to head office (VPN, backups, development server)** | Medium         | High       | Developers         | Mitigate             | Ensure **production server firewall rules** can be modified securely **without VPN access**. Maintain **alternative access** methods. Refer to the **Access Control Policy – Section 7** and **BCDR Plan – Section 6.3**. | A.13 Network Security     | Acceptable if **alternative means of accessing production servers exist**.               |
| **NAS Storage corruption or damage** | Medium         | High       | Team Lead Developer | Mitigate             | Conduct a **yearly backup integrity check**. Refer to the **BCDR Plan – Section 5.1 & 8** for test and retention validation procedures.                               | A.12 Backup Policy        | Acceptable if **yearly backups pass integrity checks**.                                 |

---

### **1.3 Human Resource Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Critical employee suddenly leaving** | Medium | Medium | Managing Director | Mitigate | Document **all key processes** in the internal knowledge base, ensure **secure password storage** in LastPass, and implement **role-based access restrictions** as defined in the [Access Control Policy](#access-control-policy). | A.7 Human Resource Security | Acceptable if **a knowledge base is maintained and access controls are enforced**. |
| **Developer’s laptop lost, stolen, or damaged** | Medium | Medium | Team Lead Developer | Mitigate | Enforce **cloud-based storage with encryption** (per [Asset Management Policy](#asset-management-policy)) and use **secure password managers** as defined in the [Access Control Policy](#access-control-policy). | A.8 Asset Management | Acceptable if **all critical data is securely stored in the cloud**. |
| **Sudden departure of CEO or Managing Director** | Low | High | CEO / Managing Director | Mitigate | Store all critical credentials in a shared LastPass vault. Define succession roles and document recovery steps in the BCDRP. | A.7 Human Resource Security | Acceptable if full access continuity is documented and roles are reassigned within 1 day. |


---

### **1.4 Cybersecurity Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Virus or ransomware attack on company devices** | Medium | Medium | Team Lead Developer | Mitigate | Install **enterprise-grade antivirus software**, enable **automatic updates**, and conduct **regular security training** as outlined in the [Access Control Policy](#access-control-policy). | A.12 Malware Protection | Acceptable if **endpoint protection is always enabled and updated**. |
| **Losing access to LastPass (password manager)** | Low | High | CEO | Mitigate | Maintain a **bi-yearly backup of critical passwords** in an **encrypted and secure location**, documented in the [Access Control Policy](#access-control-policy). | A.9 Access Control | Acceptable if **backup plan is tested annually**. |
| **SSL certificate expiry for platform or website** | High | Medium | Team Lead Developer | Mitigate | Enable **automatic SSL renewal** or set up **early expiration alerts** as described in the [Access Control Policy](#access-control-policy). | A.14 System Security | Acceptable if **automatic renewal is active or renewal reminders are in place**. |

---

## **2. Risk Review and Approval**

This document will be reviewed **annually** and **after any significant changes** to infrastructure, services, or security risks.


---

# Access Control Policy

## 1. Purpose

This Access Control Policy defines guidelines for managing access to Rate's information systems, cloud applications, and on-premises infrastructure. It ensures proper role-based access and aligns with ISO/IEC 27001:2022 Annex A.5.15 requirements.

## 2. Scope

This policy applies to all personnel accessing Rate's information assets, including:

- **On-Premises Systems and Networks:**
  - `dashboard.rate.nl` (Global Admin and Client-specific)
  - `dashdev.rate.nl` (Test & Development)
  - NAS (Backup System) - Secured with locked storage
  - Development Server - Secured with locked storage
  - WiFi Networks: "Rate.nl employee," "Rate.nl guest," and "KH\_OFFICES"
- **Cloud Applications and Providers:** Google Drive, Google Workspace, GitHub, Stack Overflow, Exact Online, WordPress, and Hetzner Cloud
- **Remote Access Systems:** Remote Desktop Server, Local VPN (Hetzner), and employee-managed laptops

## 3. Access Control Principles

- **Least Privilege:** Limit access to the minimum necessary for tasks.
- **Need-to-Know:** Restrict sensitive data access.
- **Role-Based Access Control (RBAC):** Assign permissions based on job roles.
- **Separation of Duties:** Divide security-sensitive responsibilities.

## 4. User Access Management

### **4.1. Registration and De-registration**

- **Registration:** Requests are submitted to the team lead via email. CEO approval is required for high-privilege access. Requests are stored in email records, which serve as documentation.
- **De-registration:** The CEO instructs the team lead via email to revoke access upon role change or departure.
- **Documentation:** Access approvals and removals are retained in email records. and must be updated in **Access Overview** ([view file](https://docs.google.com/document/d/1zzRYV8-JB9kXEzqw2DPTuI3aIKU_ifDiUABFxwWd43I/edit?tab=t.0)).


### **4.2. Provisioning and Review**

- Developers are responsible for ensuring secure implementation of access control measures within the systems they develop.
- Records are maintained for audit purposes.
- **User Access Review Frequency:** Access permissions are reviewed \*\*annually \*\*to ensure only authorized users retain access to systems.

### **4.3. Onboarding and Offboarding Process**&#x20;

#### **Pre-Employment Screening**

In alignment with ISO/IEC 27001:2022 Annex A.7.1.1, all candidates offered employment at Rate undergo pre-employment screening appropriate to the role. This includes:

- Verification of identity and qualifications.
- Reference checks (where legally permissible).
- Confirmation of past employment history.

Pre-employment screening is coordinated by the Managing Director and documented in the HR records.


#### **Onboarding**

1. **User Registration:** HR submits an onboarding request to the Managing Director.
2. **Access Provisioning:** IT provisions necessary accounts (VPN, email, internal platforms) with **role-based access**.Access granted is recorded in the **Access Overview** ([view file](https://docs.google.com/document/d/1zzRYV8-JB9kXEzqw2DPTuI3aIKU_ifDiUABFxwWd43I/edit?tab=t.0))
3. **Security Training:** New employees must complete security awareness training within the first week.
4. **NDA Agreement:** Employees sign a **Confidentiality Agreement (NDA)** before accessing sensitive data.
5. **Asset Assignment:** Laptops, security tokens, and other assets are logged in the asset inventory.

#### **Offboarding**

1. **Account Deactivation:** The **CEO or Managing Director** instructs the **team lead** to revoke all access.
2. **Asset Return:** Employees return laptops, access cards, and security tokens to the **Managing Director**.
3. **Exit Security Review:** The Managing Director ensures final security clearance and access revocation is signed off in the **Access Overview** ([view file](https://docs.google.com/document/d/1zzRYV8-JB9kXEzqw2DPTuI3aIKU_ifDiUABFxwWd43I/edit?tab=t.0)).


#### Security Awareness Training

## 1. Purpose

To ensure all employees understand their **security responsibilities** and comply with Rate’s ISMS, as required by **ISO 27001:2022 Clause A.7.2.2**.

## 2. Training Requirements

| **Training**                | **Target Audience** | **Frequency**              | **Delivery Method**                |
| --------------------------- | ------------------- | -------------------------- | ---------------------------------- |
| Security Awareness Training | All employees       | Upon onboarding + annually | Online session / internal training |

## 3. Compliance Tracking

- Training completion records are **logged and retained** in **Google Drive**.
- Employees who fail to complete mandatory training will be **notified and required to comply**.
- Non-compliance may result in **access restrictions** or further corrective measures.
- **The Managing Director is responsible for overseeing the training program, ensuring compliance, and tracking completion rates.**

## 5. Authentication and Password Management

In compliance with ISO/IEC 27001:2022 Annex A.9.4.3, Rate enforces a strong password policy for all systems and applications:

- **Minimum Length:** Passwords must be at least **12 characters** long.
- **Complexity Requirements:** Passwords must include **at least three of the following**:
  - Uppercase letters (A–Z)
  - Lowercase letters (a–z)
  - Numbers (0–9)
  - Special characters (e.g., !@#$%^&*)
- **Password History:** Users must not reuse the last **5 passwords**.
- **Password Expiry:** Passwords must be changed **every 180 days** unless longer periods are justified by additional security measures.
- **Account Lockout:** Accounts are locked after **5 failed login attempts**, with automatic unlock after 15 minutes.
- **Secure Storage:** Passwords must never be stored in plaintext. All credentials are securely stored using **LastPass** with end-to-end encryption.
- All critical credentials (production servers, cloud accounts, HR systems) are securely stored in LastPass, with shared access for both the CEO and Managing Director.In the event one of them leaves, the other ensures smooth access continuity and triggers access reviews and necessary reassignments.
- **Multi-Factor Authentication (MFA):** MFA is **recommended** for access to production systems, VPN, and administrative tools to enhance security.

All employees are made aware of these requirements during onboarding and through annual security awareness training.


## 6. Monitoring and Logging

- **Logs:** Collected from all on-premises and cloud systems.
- **Retention:** Logs are retained for **1 year**&#x20;

## 7. Alternative Secure Access Methods

In the event of **VPN failure**, an **alternative secure access method** must be available to ensure continued access to critical systems. This may include:

- Direct secure SSH access with IP whitelisting.
- Temporary access via emergency backup accounts (only activated under CEO approval).
- Additional secure remote access solutions evaluated based on security needs.

## 8. Physical Access Control

- Building entry requires key card access.
- Office access is secured by key.
- NAS and Development Server are stored under lock.
- Production servers are cloud-hosted on Hetzner.

## 9. Responsibilities

- **team lead:** Manages access, and oversees configurations.
- **CEO:** Approves sensitive access requests and enforces compliance.
- **Developers:** Ensure secure implementation of access control measures in systems they develop.
- **All Employees:** Maintain laptop security and promptly report incidents.

## 10. Policy Review

The policy undergoes **annual review** or immediate revision after major changes.

## 11. Compliance

Non-compliance may result in disciplinary actions or legal consequences.

*Note: Employees will be notified of all policy updates.*



---


# Incident Management and Response Plan

## 1. Purpose
This Incident Management and Response Process outlines the procedures for identifying, reporting, assessing, responding to, and recovering from security incidents at Rate. The objective is to minimize the impact of incidents, protect information assets, and ensure business continuity.

## 2. Scope
This plan applies to all employees, contractors, and third-party service providers with access to Rate's systems, applications, and networks.

## 3. Incident Definition
A security incident is any event that compromises the confidentiality, integrity, or availability of Rate's information systems. Examples include:
- Unauthorized access to `dashboard.rate.nl`, `dashdev.rate.nl`, or cloud services
- Data breaches or loss of customer survey data
- Malware or ransomware attacks
- Network outages affecting `Rate.nl` WiFi or VPN services
- Physical security breaches (e.g., NAS or Development Server access)

## 4. Reporting Mechanism
### **4.1. Internal Reporting**
- Employees must report incidents immediately via email to the team lead.
- High-severity incidents should be escalated to the CEO and Managing Director.
- Incident details should include date, time, affected systems, and a brief description.
* Use the following form to record incidents:

| **Template Name**             | **Purpose**                                                | **Link**                                                          |
| ----------------------------- | ---------------------------------------------------------- | ----------------------------------------------------------------- |
| Security Incident Report Form | To document and manage security incidents (A.5.24, A.5.25) | [View Template](https://docs.google.com/document/d/1qNgrz0pVWFuE2jzb2sc4SQB8KdniGmpaVv-866N25tg/edit?tab=t.0#heading=h.epb41kpmjny7) |


### **4.2. External Reporting**
- If customer data is affected, the CEO will communicate with impacted parties.
- Regulatory bodies (e.g., GDPR authorities) will be notified if required by law.

## 5. Incident Response Phases
### **5.1. Identification**
- Incidents are detected through system monitoring, employee reports, and automated alerts.
- The team lead reviews logs from cloud providers (Google Workspace, Hetzner) and on-premises systems.

### **5.2. Containment**
- Immediate actions include disabling compromised accounts and revoking VPN access.
- Affected devices should be isolated from corporate networks.

### **5.3. Eradication**
- The root cause of the incident is identified and mitigated.
- Systems are patched, malware is removed, and security gaps are addressed.

### **5.4. Recovery**
- Systems are restored from backups, and normal operations resume.
- Data integrity is verified on Google Drive, Exact Online, and production servers.
- **Annual backup testing is required** to ensure reliability, in alignment with the Risk Treatment Plan (RTP).

### **5.6. Post-Incident Learning (Annex A.5.27)**

Following any significant security incident, a **Post-Incident Review (PIR)** must be conducted by the Managing Director and team lead to:

- Identify the root cause of the incident.
- Assess the effectiveness of existing controls and the response process.
- Document lessons learned and areas for improvement.
- Recommend updates to policies, procedures, or technical safeguards if applicable.
- Record all findings in the **Incident Log** and assign any actions in the **Corrective Actions Log**.

PIR outcomes are reviewed during **Management Review Meetings** and are used to improve the ISMS continuously.


## 6. Documentation and Reporting
- All incidents must be logged, including:
  - Incident ID
  - Date and time of detection
  - Description and impact
  - Actions taken
  - Resolution date
- Incident logs are maintained in Google Drive.

## 7. Roles and Responsibilities
### **7.1. Employees**
- Report security incidents immediately.
- Cooperate with investigations and follow security protocols.

### **7.2. team lead**
- Leads **technical containment and resolution** of incidents.
- Reviews and maintains incident logs.
- Coordinates security improvements post-incident.

### **7.3. Managing Director**
- **Leads overall incident response efforts**, ensuring proper execution of containment, eradication, and recovery steps.
- Assists in response when the team lead is unavailable.
- Supports log analysis and recovery processes.

### **7.4. CEO**
- Approves major response actions and external reporting.
- Oversees communication with stakeholders and regulatory bodies.

## 8. Communication Plan
- **Internal:** team lead provides updates via email to the CEO and relevant teams.
- **External:** The CEO handles customer notifications and regulatory compliance communication.

## 9. Plan Review and Testing
- The plan is reviewed after major incidents.

## 10. Compliance and Reporting
- Incident logs are retained in Google Drive.
- The plan adheres to **ISO/IEC 27001:2022** and **GDPR** requirements.

*Note: Employees will be notified of policy updates.*


---

# Business Continuity and Disaster Recovery Plan (BCDRP)

**Aligned with ISO/IEC 27001:2022 and Integrated with Risk Assessment and Treatment Plan**

## **1. Purpose**

This plan outlines procedures for maintaining business operations and recovering from disruptions at **Rate**, ensuring continuity of services and rapid recovery from disasters. It incorporates controls from the Risk Assessment and Treatment Plan (RTP).

## **2. Scope**

Covers all systems, employees, cloud services, and processes supporting **Rate's platform and operations**.

## **3. Key Contacts**

- **Disaster Recovery Team:**
  - **CEO (Head)** – Primary decision-maker
  - **Managing Director** – Operations and communications
  - **Team Lead Developer** – Technical recovery lead
- **Contact Email:** [info@rate.nl](mailto\:info@rate.nl)

## **4. Critical Systems and Dependencies**

| **System/Service**                       | **Provider**                   | **Backup Location**                                              | **RTO**   | **RPO**    | **Owner**           |
| ---------------------------------------- | ------------------------------ | ---------------------------------------------------------------- | --------- | ---------- | ------------------- |
| **Production Hosting**                   | Hetzner (Primary)              | NAS                                                              | 4 hours   | 30 minutes | Team Lead Developer |
| **Secondary Hosting (Provider Failure)** | Azure                          | Cloud                                                            | 4 hours   | 30 minutes | Team Lead Developer |
| **Source Code Repository**               | GitHub                         | Cloud with integrity checks                                      | 1 hour    | Real-time  | Team Lead Developer |
| **Backups**                              | NAS (Local)                    | Monthly restoration tests & **annual full integrity validation** | N/A       | 30 minutes | Team Lead Developer |
| **VPN & Remote Access**                  | Local VPN on Dev Server        | N/A                                                              | Immediate | None       | Managing Director   |
| **Communication Tools**                  | Google Workspace (email, docs) | Google Cloud                                                     | Immediate | None       | Managing Director   |
| **HR and Compliance System**             | Exact Online                   | Cloud                                                            | 2 hours   | 1 hour     | Managing Director   |
| **Password Manager**                     | LastPass                       | NAS                                                 | 1 hour    | 30 minutes | CEO                 |
**Third-Party Responsibilities:**

- **Hetzner** is responsible for the availability and physical security of the production infrastructure hosted on their cloud platform. This includes power supply, physical access control, and network connectivity within the data center.
- Rate is responsible for server configuration, data backups, monitoring, and triggering recovery procedures.
- In the event of a Hetzner outage, Rate will initiate failover to Azure and handle full restoration.


## **5. Backup and Recovery Procedures**

### **5.1 Database Backups (Critical)**

- **Full Daily Backup:** 03:00 (retained 1 month) – Stored on NAS and cloud
- **Incremental Backups:** Every 4 hours (retained 1 month)
- **Transaction Log Backups:** Every 30 minutes (retained 1 month)
- **Testing:** Monthly restoration from backups & **annual full validation check**
- **Backup Retention Policy:** *(Updated)* Backups retained for **one month for standard data, one year for critical logs**.

### **5.2 Production Application Folder Backups**

- **Full Daily Backup:** 03:00 (retained 1 month) – Stored on NAS and cloud
- **Testing:** Monthly restoration and integrity checks & **annual full validation check**

### **5.3 Source Code Backups**

- **Managed In:** GitHub

### **5.4 Backup Retention Policy:**

- **Location:** Local NAS
- **Retention Period:** 3 Years.

## **6. Disaster Scenarios, RTO, and RPO**

| **Scenario**                                         | **Action Plan**                                                                              | **Lead**            | **RTO (Recovery Time Objective)** | **RPO (Recovery Point Objective)** |
| ---------------------------------------------------- | -------------------------------------------------------------------------------------------- | ------------------- | --------------------------------- | ---------------------------------- |
| **6.1 Production Server Failure (Hetzner)**          | Provision a new Hetzner server, restore from repository backups                              | Team Lead Developer | 4 hours                           | 30 minutes                         |
| **6.2 Cloud Provider Failure (Hetzner Unavailable)** | Deploy server on Azure, restore backups, notify customers                                    | Team Lead Developer | 4 hours                           | 30 minutes                         |
| **6.3 Office Internet Outage**                       | Use alternative access means like whitelisting new ips in the firewall.                      | Managing Director   | Immediate                         | None                               |
| **6.4 Data Leak or Malware Attack**                  | Isolate systems, notify Managing Director, conduct forensic analysis                         | Managing Director   | 2 hours                           | 30 minutes                         |
| **6.5 Calamities (Fire, Flood, Physical Theft)**     | Follow Groothandelsgebouw escape plan, secure backups offsite                                | CEO                 | As feasible                       | 30 minutes                         |
| **6.6 Loss of LastPass (Password Manager)**          | Restore from encrypted NAS backup, reset passwords for critical systems                    | CEO                 | 1 hour                            | 30 minutes                         |
| **6.7 SSL Certificate Expiry for Website/Platform**  | **Enable SSL auto-renewals are enabled** or set calendar reminders for manual renewal checks | Team Lead Developer | 1 hour                            | None                               |
| **6.8 Sudden Departure of CEO or Managing Director** | Access Rate's credentials via LastPass. Redistribute operational and ISMS responsibilities to designated successors. Document transition actions and notify key stakeholders. | Managing Director / CEO | 1 day | None |


## **7. Roles and Responsibilities**

| **Role**                                 | **Responsibilities During Disaster**                                          |
| ---------------------------------------- | ----------------------------------------------------------------------------- |
| **CEO (Head of Disaster Recovery Team)** | Authorizes major decisions, communicates with customers and stakeholders      |
| **Managing Director**                    | Oversees recovery operations, manages communications, maintains incident logs |
| **Team Lead Developer**                  | Executes technical recovery steps, restores servers, maintains backup records |
| **All Employees**                        | Follow the BCDRP procedures and report security incidents immediately         |

> **Note:** In the event the **CEO** or **Managing Director** becomes unavailable or leaves the company, the remaining executive temporarily assumes full responsibility for all critical disaster recovery and ISMS decisions. All necessary credentials and documentation are stored in a **shared LastPass vault** to ensure uninterrupted operations and access.


## **8. Testing and Review (ISO Clause 8.1 & 9.1)**

- **Testing Frequency:** Yearly (full disaster recovery drill) with monthly backup restoration tests
- **Test Components:** Server restoration, VPN failover, LastPass recovery
- **Review Cycle:** **Annual** or after any major incident or infrastructure change
- **Responsible for Testing:** Managing Director



## **9. Compliance and Recordkeeping (ISO Clause 9.2 & 9.3)**

| **Record**    | **Retention Period** | **Storage Location** | **Responsible Owner** |   |
| ------------- | -------------------- | -------------------- | --------------------- | - |
| Backups       | 3 years              | NAS                  | Team Lead Developer   |   |
| Incident Logs | 3 years              | Google Drive         | Managing Director     |   |
|               |                      |                      |                       |   |

### **Compliance with Standards:**

**ISO/IEC 27001:2022** (Clauses 9.2, 9.3,)\
**GDPR (Article 32: Security of Processing)**



---

# Asset Management Policy

## 1. Purpose

This policy defines procedures for managing and protecting Rate's information assets, ensuring compliance with ISO/IEC 27001:2022.

## 2. Scope

Applies to all digital, physical, and cloud-based assets accessed by Rate employees, contractors, and third parties.

## 3. Asset Inventory and Ownership

- **Asset Inventory:** Managed by the Managing Director, covering hardware, software, cloud services, and backups.
- **Asset Ownership and Management:**
  - **Hardware:** Owned and maintained by the Team Lead Developer.
  - **Software & Cloud Services:** Owned by the Managing Director, with maintenance delegated to relevant teams.
  - **Data (including backups):** Owned by the Team Lead Developer; Managing Director oversees classification and access.
  - Each asset in the inventory must have a designated owner listed with their responsibilities documented in the inventory file.

- **Role Assignments:**
  - **Hardware:** Team Lead Developer.
  - **Software/Cloud Services:** Managing Director.
  - **Data (including backups):** Team Lead Developer and Asset Owners.
- **Documentation:** Logs include asset classification, ownership, and review records.
- **Asset Classification:**
  - Assets are categorized into the following levels:
    - **Public** – Information freely available to the public.
    - **Internal** – Non-sensitive company information meant for employees.
    - **Confidential** – Restricted data with controlled access.
    - **Restricted** – Highly sensitive data requiring strict security measures.
  - **All assets in the inventory must be classified accordingly** and updated in the asset inventory list.
  - Asset classification must be reviewed annually to ensure proper security controls are in place.

## 4. Acceptable Use and Protection Measures

- **Device Security:** Full disk encryption and automatic updates are mandatory.
- **Data Storage:** Role-based access controls protect sensitive data.
- **Backups:** Daily backups with **monthly restoration tests and an annual full validation check**.

## 5. Access Control and Data Security (Annex A.9)

- **Access Management:** Controlled by the team lead with CEO approval for high-privilege roles.
- **Log Retention:** Access logs are retained for **one year** to align with compliance requirements.
- **Access Revocation:** Immediate action for role changes or departures, with records documented.
- **Remote Access:** VPN is required for development server access.

## 6. Data Retention and Disposal (Annex A.8, A.11)

- **Retention Periods:** Backups retained for **one month for standard data, one year for critical logs** .
- **Secure Disposal:** Hardware is securely wiped and destroyed.
- **Disposal Records:** Logs include date, method, approver details, and retention for three years.

## 7. Monitoring and Review (Annex A.12, A.15)

- **Audit Documentation:** Managed by the Managing Director, documenting findings, corrective actions, and dates.
- **Policy Review:** Annually conducted with updates and actions logged.
- **Audit Record Retention:** All audit reports and supporting documents retained.

## 8. Roles and Responsibilities (Annex A.7, A.6)

- **Managing Director:** Manages inventory, risk assessments, audit logs, and ensures Statement of Applicability (SoA) mappings are current.
- **Team Lead Developer:** Conducts asset reviews, oversees backups, and verifies disposal records.
- **Asset Owners:** Maintain classification records and ensure security controls are applied.
- **Employees:** Follow policies, and report security issues.


## Secure Development & Change Management

This section describes Rate’s secure development and change management process, aligning with ISO/IEC 27001:2022 Annex A.8.28, A.8.29, and A.14.2.8.

### 1. Development Process Overview

Rate follows an Agile development methodology using the **Kanban method** to manage software changes. The process is visualized on a customer support board with distinct swimlanes and status columns.

**Customer support Columns:**
- Backlog
- Scoped
- Risk Analysis
- Ready for development
- In Progress
- Add to Knowledge Base
- Ready to test
- Ready to deploy
- Inform Stakeholders
- Done

Developers work from right to left to keep the board flowing efficiently. Cards are assigned to one responsible person at a time.

### 2. Secure Development Practices

- Rate uses **two isolated environments**: a **development** and a **production** environment.
- **Live data** is never used in development except with explicit customer consent.
- Developers must adhere to **OWASP secure coding practices for .NET**.
- Code is committed to version control daily.
- After development, issues and solutions are documented in the knowledge base.
- Testing is performed before deployment.
- All changes must be **approved by the Team Lead Developer** before deployment.

### 3. Urgent or Blocked Tasks

- Urgent tasks are prioritized and fast-tracked through the workflow.
- Cards can be blocked at any point pending information or decisions.

### 4. Documentation and Retention

- Each card includes a short description of changes and test results.
- Final versions are archived once deployment and stakeholder communication are completed.
- All production changes are recorded in the **[Change Management Log](https://docs.google.com/spreadsheets/d/1aTAYJK-ycFjJh9wI8hkGKIsSFxHTPhW5TxiL7bMx1hA/edit?gid=2142384983#gid=2142384983)** .

---

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

## Applicable ISO 27001:2022 Controls

| **Annex A Control (2022)** | **Control Title**                                                        | **Justification**                                            | **Related Policy/Process**                               | **Responsible Role**                   |
|----------------------------|--------------------------------------------------------------------------|--------------------------------------------------------------|----------------------------------------------------------|----------------------------------------|
| A.5.1                      | Policies for information security                                        | Required for ISMS governance.                                | Information Security Policy                               | CEO                                    |
| A.5.3                      | Segregation of duties                                                    | Ensures accountability and avoids conflicts of interest.     | ISMS Roles & Responsibilities                             | CEO, Managing Director                 |
| A.6.1                      | Screening                                                                | Prevents insider threats through background verification.    | Access Control Policy (Onboarding Process)                | Managing Director                      |
| A.6.2                      | Terms and conditions of employment                                       | Ensures employees understand their security responsibilities.| Access Control Policy                                     | Managing Director                      |
| A.6.3                      | Information security awareness, education and training                   | Promotes ongoing security awareness among staff.             | Access Control Policy (Training Process)                  | Managing Director                      |
| A.5.9                      | Inventory of information and other associated assets                     | Prevents data loss by ensuring all assets are accounted for. | Asset Management Policy                                   | Managing Director, Team Lead Developer |
| A.5.10                     | Acceptable use of information and other associated assets                | Enforces proper handling and usage of assets.                | Asset Management Policy                                   | Managing Director                      |
| A.5.11                     | Return of assets                                                         | Ensures retrieval of assets upon employee exit.              | Asset Management Policy                                   | Managing Director                      |
| A.5.15                     | Access control                                                           | Reduces risk of unauthorized access.                         | Access Control Policy                                     | Team Lead Developer                    |
| A.5.16                     | Identity management                                                      | Manages user identities securely.                            | Access Control Policy                                     | Team Lead Developer                    |
| A.5.17                     | Authentication information                                               | Protects authentication credentials.                         | Access Control Policy                                     | Team Lead Developer                    |
| A.5.18                     | Access rights                                                            | Regularly reviews and updates access rights.                 | Access Control Policy                                     | Team Lead Developer                    |
| A.5.19                     | Information security in supplier relationships                           | Ensures security responsibilities clearly defined for suppliers.| Supplier Security & Contractual Obligations             | Managing Director                      |
| A.5.20                     | Addressing information security within supplier agreements               | Ensures suppliers adhere to contractual security requirements.| Supplier Security & Contractual Obligations              | Managing Director                      |
| A.7.1                      | Physical security perimeter                                              | Prevents unauthorized physical access.                       | Asset Management Policy                                   | Managing Director                      |
| A.7.2                      | Physical entry                                                           | Controls physical entry to sensitive areas.                  | Asset Management Policy                                   | Managing Director                      |
| A.8.7                      | Protection against malware                                               | Ensures system integrity and protection from malicious software.| BCDR Plan, Access Control Policy                        | Team Lead Developer                    |
| A.8.8                      | Management of technical vulnerabilities                                  | Reduces risk through timely patching and updates.            | BCDR Plan, Access Control Policy                          | Team Lead Developer                    |
| A.8.9                      | Configuration management                                                 | Maintains secure system configurations.                      | BCDR Plan, Access Control Policy                          | Team Lead Developer                    |
| A.8.13                     | Information backup                                                       | Ensures data recovery capability.                            | BCDR Plan                                                 | Team Lead Developer                    |
| A.8.20                     | Networks security                                                        | Secures network boundaries and communications.               | Access Control Policy                                     | Team Lead Developer                    |
| A.8.25                     | Secure development life cycle                                            | Integrates security into the software development process.   | Secure Development & Change Management                    | Team Lead Developer                    |
| A.8.26                     | Application security requirements                                        | Ensures applications meet security standards.                | Secure Development & Change Management                    | Team Lead Developer                    |
| A.8.28                     | Secure coding                                                            | Promotes secure coding practices.                            | Secure Development & Change Management                    | Team Lead Developer                    |


## **3. Justification for Exclusions**

These exclusions are based on:

* The absence of relevant business operations requiring these controls.
* The use of alternative security measures to mitigate associated risks.
* The reliance on cloud-based infrastructure, reducing physical security concerns.

The following Annex A controls were evaluated and determined to be **not applicable** to Rate’s ISMS scope. Justifications are based on the organization’s operations, infrastructure, and risk assessment results.

| Annex A Control | Control Title                                                 | Justification                                                                                |
| --------------- | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| A.5.2           | Information security roles and responsibilities               | Roles and responsibilities already clearly defined in existing policy documents.             |
| A.5.4           | Management responsibilities                                   | Covered under established ISMS documentation and governance processes.                       |
| A.5.5           | Contact with authorities                                      | No regulatory requirement or direct communication needed with authorities.                   |
| A.5.6           | Contact with special interest groups                          | No direct involvement with industry special interest groups.                                 |
| A.5.7           | Threat intelligence                                           | Managed through existing security and vulnerability management processes.                    |
| A.5.8           | Information security in project management                    | Integrated into secure development practices; no separate project management control needed. |
| A.5.12          | Classification of information                                 | Assets classification documented in Asset Management Policy.                                 |
| A.5.13          | Labelling of information                                      | Covered by standard access control and cloud-based management practices.                     |
| A.5.14          | Information transfer                                          | Minimal external information transfer; secured by encryption and access controls.            |
| A.5.21          | Managing information security in the ICT supply chain         | Managed by supplier agreements and contract security clauses.                                  |
| A.5.22          | Monitoring, review and change management of supplier services | Included under Supplier Security & Contractual Obligations.                                  |
| A.5.23          | Information security for use of cloud services                | Already explicitly addressed by individual cloud service providers (Google, Hetzner, etc.).  |
| A.5.28          | Collection of evidence                                        | Incident response processes include evidence documentation.                                  |
| A.5.30          | ICT readiness for business continuity                         | BCDR plan adequately covers ICT readiness.                                                   |
| A.5.37          | Documented operating procedures                               | Procedures documented as needed within specific policy documents.                            |
| A.6.4           | Disciplinary process                                          | Managed under general HR policies.                                                           |
| A.6.5           | Responsibilities after termination or change of employment    | Covered by onboarding/offboarding processes in Access Control Policy.                        |
| A.6.6           | Confidentiality or non-disclosure agreements                  | Employees sign NDAs upon employment, documented in HR processes.                             |
| A.6.7           | Remote working                                                | Remote work securely managed via cloud-based applications and VPN.                           |
| A.6.8           | Information security event reporting                          | Already addressed within Incident Management and Response Plan.                              |
| A.7.3           | Securing offices, rooms and facilities                        | Office security managed through physical access control procedures.                          |
| A.7.4           | Physical security monitoring                                  | Physical security managed via building infrastructure.                                       |
| A.7.5           | Protecting against physical and environmental threats         | Data centers managed externally (Hetzner) with strong physical protections.                  |
| A.7.6           | Working in secure areas                                       | No designated secure areas requiring additional controls.                                    |
| A.7.7           | Clear desk and clear screen                                   | Managed under general office practices and device security policies.                         |
| A.7.8           | Equipment siting and protection                               | Managed externally by cloud providers and minimal local hardware.                            |
| A.7.9           | Security of assets off-premises                               | All critical assets cloud-based with strong security controls.                               |
| A.7.10          | Storage media                                                 | No significant use of removable storage media.                                               |
| A.7.11          | Supporting utilities                                          | Managed by cloud provider SLA.                                                               |
| A.7.12          | Cabling security                                              | Managed externally by infrastructure providers.                                              |
| A.7.13          | Equipment maintenance                                         | Managed externally or minimal equipment requiring maintenance.                               |
| A.7.14          | Secure disposal or re-use of equipment                        | Minimal physical hardware; secure disposal already practiced.                                |
| A.8.1           | User endpoint devices                                         | Managed via access control and device encryption standards.                                  |
| A.8.2           | Privileged access rights                                      | Managed under access control policy.                                                         |
| A.8.3           | Information access restriction                                | Managed via existing RBAC implementation.                                                    |
| A.8.4           | Access to source code                                         | Managed via GitHub access and secure development practices.                                  |
| A.8.5           | Secure authentication                                         | Already implemented with strong password and MFA policies.                                   |
| A.8.6           | Capacity management                                           | Managed by cloud service providers' SLAs.                                                    |
| A.8.10          | Information deletion                                          | Managed under existing data retention and deletion policies.                                 |
| A.8.11          | Data masking                                                  | Not required due to minimal handling of sensitive personal data.                             |
| A.8.12          | Data leakage prevention                                       | Managed through access control, RBAC, and cloud-based protections.                           |
| A.8.14          | Redundancy of information processing facilities               | Managed by cloud providers' redundancy and disaster recovery measures.                       |
| A.8.15          | Logging                                                       | Managed under existing system and cloud logging mechanisms.                                  |
| A.8.16          | Monitoring activities                                         | Managed under established alerting and monitoring procedures.                                |
| A.8.17          | Clock synchronization                                         | Managed automatically by cloud services.                                                     |
| A.8.18          | Use of privileged utility programs                            | Limited scope, managed under privileged access controls.                                     |
| A.8.19          | Installation of software on operational systems               | Strictly controlled and managed by automated processes.                                      |
| A.8.21          | Security of network services                                  | Managed externally by cloud providers.                                                       |
| A.8.22          | Segregation in networks                                       | Cloud provider responsibilities and network configurations in place.                         |
| A.8.23          | Web filtering                                                 | Managed through existing network and endpoint controls.                                      |
| A.8.27          | Secure system architecture and engineering principles         | Managed under secure development processes.                                                  |
| A.8.29          | Security testing in development and acceptance                | Managed through existing secure development lifecycle.                                       |
| A.8.30          | Outsourced development                                        | No outsourced software development.                                                          |
| A.8.31          | Separation of development, test and production environments   | Clearly separated by existing processes and GitHub workflows.                                |
| A.8.32          | Change management                                             | Managed under existing secure development and deployment procedures.                         |
| A.8.33          | Test information                                              | Minimal test data, already securely managed.                                                 |
| A.8.34          | Protection of information systems during audit and testing    | Secure testing practices already in place.                                                   |



---

## **4. Control Review and Updates**
The **Statement of Applicability (SoA)** is reviewed and updated:
- **Annually** or **whenever significant changes occur** in **technology, business processes, or risk landscape**.
- **During internal audits** as part of Rate’s **Continuous Improvement Process**.
- **When new risks are identified** that require control modifications.
- **Upon regulatory changes** affecting information security compliance (**e.g., GDPR updates**).

---

# Compliance & Security Governance

## 1. Legal & Regulatory Requirements

Rate is committed to ensuring compliance with all applicable **legal, regulatory, and contractual obligations** related to information security. The following regulations and industry standards apply:

### **Applicable Laws & Regulations**

- **General Data Protection Regulation (GDPR)** – Governs data protection and privacy for EU residents.
- **ISO/IEC 27001:2022** – International standard for information security management.
- **Any contractual agreements that impose security obligations** on Rate.

### **Compliance Review & Tracking**

The **Managing Director** is responsible for reviewing applicable laws and regulatory changes **annually** and ensuring our policies are updated accordingly.

---

# Privacy & Data Protection Policy

## 1. Purpose

This Privacy & Data Protection Policy defines how Rate collects, stores, processes, and protects personal data in compliance with **GDPR** and relevant data protection regulations.

## 2. Scope

This policy applies to all personal data collected from customers, employees, and third parties interacting with Rate's services.

## 3. Data Collection & Processing

- **Purpose of Data Collection:** Rate collects personal data strictly for providing survey analytics and user account management.
- **Data Processing Basis:** Data is processed based on **legitimate business interest, contractual necessity, or user consent**.

## 4. Data Subject Rights

Users have the right to:

- **Access** their personal data.
- **Request corrections or updates** to inaccurate information.
- **Request deletion** of personal data ("right to be forgotten").
- **Restrict processing** under certain conditions.
- **Obtain a copy** of their personal data.

### **How to Submit a Request**

Users can submit requests via email at **[********[support@rate.nl](mailto\:support@rate.nl)********]**, and we will respond **within 30 days**.

## 5. Data Retention & Secure Deletion

- Personal data is retained for **12 months** unless legally required otherwise.
- Upon request or expiration, data is **securely erased.**
- Backup data is **retained for up to 1 year**, after which it is securely deleted.

## 6. Compliance & Review

The **Managing Director** is responsible for reviewing and updating this policy **annually**.

---

# Supplier Security & Contractual Obligations

## 1. Purpose

This section defines **security obligations for third-party suppliers** who access Rate's data or infrastructure.

## 2. supplier List & Review Process

All third-party suppliers handling Rate’s sensitive data must be reviewed and approved.

| **supplier Name**       | **Service Provided**         | **Data Accessed**               | **Security Compliance**         | **Review Frequency** | **Responsible Owner**  |
|----------------------|----------------------------|--------------------------------|--------------------------------|--------------------|------------------|
| **Hetzner Cloud**     | Server Hosting             | Customer Survey Data           | ISO 27001 Certified             | Annually           | Managing Director  |
| **Google Workspace**  | Email, Docs, Cloud Storage | Internal Business Data         | GDPR Compliant                  | Annually           | Managing Director  |
| **GitHub**           | Source Code Repository     | Internal Codebase              | SOC 2 Type II, ISO 27001        | Annually           | Team Lead Developer |
| **LastPass**         | Password Manager           | Encrypted Password Storage     | SOC 2 Type II, GDPR Compliant   | Annually           | CEO |
| **Exact Online**     | HR & Financial System      | Employee & Financial Data      | ISO 27001, GDPR Compliant       | Annually           | Managing Director  |
| **Stack Overflow**   | Developer Collaboration    | Internal knowledge base      | Data Encrypted in Transit       | Annually           | Managing Director |
| **Freshdesk**       | Customer Support System    | Customer Service Data          | ISO 27001, GDPR Compliant       | Annually           | Managing Director  |
| **Trello**         | Project Management         | Internal Business Data         | SOC 2, GDPR Compliant           | Annually           | Managing Director  |

## 3. Security Responsibilities

### Hetzner Cloud
- Ensure physical security and access control of data centers.
- Maintain infrastructure security and server updates.
- Regular backups and disaster recovery.
- Immediate notification of security breaches.

### Google Workspace
- Data encryption in transit and at rest.
- Regular security assessments and compliance with GDPR.
- Immediate breach notification and transparent incident reporting.

### GitHub
- Protection of source code repositories.
- Compliance with secure coding and version control best practices.
- Regular audits and incident management procedures.

### LastPass
- Secure storage of encrypted passwords.
- Robust access control and multi-factor authentication.
- Regular security assessments and breach notifications.

### Exact Online
- Secure handling of financial and employee data.
- Compliance with GDPR and ISO 27001.
- Immediate notification of security incidents.

### Stack Overflow
- Protection of internal knowledge data.
- Data encryption in transit.
- Notification of any security incidents or vulnerabilities.

### Freshdesk
- Secure management of customer service data.
- Data encryption and compliance with GDPR.
- Regular audits and prompt incident notifications.

### Trello
- Secure project management data handling.
- Compliance with SOC 2 and GDPR.
- Notification and management of security incidents.

---

## 4. Security Clauses for supplier Contracts

All contracts with suppliers must include the following security obligations:

- **Compliance with ISO 27001 & GDPR**.
- **Data encryption during storage and transmission**.
- **Breach notification within 24 hours**.
- **Regular security audits & access control reviews**.

**supplier agreements are reviewed annually** to ensure compliance.

---



---

# Internal Audit Program

## 1. Purpose

The **Internal Audit Program** ensures that Rate’s security policies, controls, and ISMS implementation align with **ISO/IEC 27001:2022** and contribute to continuous improvement.

## 2. Audit Frequency & Planning Process

Rate conducts **internal audits annually** to verify compliance with ISO 27001 requirements.

### **Audit Planning**

Each year, a structured **audit plan** is developed by the **Managing Director** and approved by the **CEO**. The plan includes:

- **Audit Scope**: All ISMS policies, procedures, controls, and the Statement of Applicability (SoA)
- **Audit Objectives**: 
  - Confirm the effectiveness of implemented controls  
  - Detect non-conformities and improvement opportunities  
  - Validate risk treatment implementation
- **Schedule**: Annual audit, with flexibility to conduct follow-ups or focused audits if needed
- **Criteria**: ISO 27001:2022 clauses, Annex A controls, internal policies, and risk treatment outcomes
- **Audit Independence**: Auditors are assigned to areas where they are not directly responsible
- **Documentation**: The audit plan, evidence, and findings are stored securely in Google Drive

### **Audit Process**

1. **Review Policies & Controls** – Assess ISMS documents and controls.
2. **Verify Implementation** – Check access logs, backups, training records, and compliance reports.
3. **Identify Non-Conformities** – Document issues and assign severity ratings.
4. **Report & Corrective Actions** – Assign responsibilities and deadlines for resolution.
5. **Follow-Up (if needed)** – Verify that corrective actions were completed.

## 3. Internal Audit Log

| **Audit Date** | **Reviewed By**   | **Findings**             | **Corrective Actions**        |
| -------------- | ----------------- | ------------------------ | ----------------------------- |


## 4. Review & Updates

Audit findings are reviewed by the **CEO**, and all corrective actions must be implemented **within 30 days**. Audit plans and outcomes are reviewed annually or when significant changes occur.



# Corrective Actions & Non-Compliance Log

## 1. Purpose

This section defines how **non-compliance issues** are identified, recorded, and resolved **within 30 days**.

## 2. Non-Compliance Handling Process

1. **Identify Issue:** Any non-compliance is **logged**.
2. **Assign Responsibility:** A team member is assigned to fix the issue.
3. **Set a Deadline:** Issues must be resolved **within 30 days**.
4. **Verify Resolution:** The CEO approves resolution before closing.

## 3. Non-Compliance Log

| **Issue**             | **Detected Date** | **Assigned To**     | **Resolution Date** | **Status** |
| --------------------- | ----------------- | ------------------- | ------------------- | ---------- |


**Corrective actions are reviewed annually** by the CEO.

## 4. External Audit 2024 – Corrective Actions

For reference and audit traceability, the corrective actions taken in response to the **2024 ISO 27001 external audit** are documented and tracked in the following log:

 **[2024 ISO Audit – Corrective Actions Log](https://docs.google.com/spreadsheets/d/158OZ0o3GnyeTbsZXJwQG2oTLb0GeGbNR/edit?gid=529622322#gid=529622322)**  


---

# Management Review

## 1. Purpose

To ensure that Rate's ISMS remains effective, compliant, and continuously improving through structured and well-documented reviews by top management. This process aligns with **ISO 27001:2022 Clause 9.3**.

## 2. Review Frequency

- Conducted **annually**, and after any **major incident**, significant **change in business operations**, or **updates in legal or regulatory requirements**.

## 3. Review Agenda (Inputs)

The management review shall include:

- Status of actions from previous reviews
- Results of internal audits and corrective actions
- ISMS performance metrics and KPI achievement
- Status of security incidents and risk treatment
- Effectiveness of controls and security objectives
- Feedback from stakeholders and users
- Opportunities for continual improvement
- Changes in internal/external issues relevant to the ISMS
- Adequacy of resources and assigned roles

## 4. Review Outputs (Decisions & Actions)

The review will result in:

- Decisions on **updates to policies, procedures, and risk treatment**
- Modifications to **ISMS objectives** and KPIs
- Approval of **corrective actions and improvement plans**
- Assignment of new **responsibilities or resources**
- Validation of ISMS scope and SoA applicability

All **decisions and actions are recorded** in the **Management Review Minutes** and **Corrective Actions Log**, with clear **due dates and owners**.

## 5. Responsibilities

| Role             | Responsibility                                                       |
|------------------|----------------------------------------------------------------------|
| **CEO**          | Chairs the meeting, approves decisions, ensures alignment with strategy |
| **Managing Director** | Prepares agenda, records minutes, tracks action items              |

## 6. Documentation and Retention

- **Meeting minutes** and decisions are stored in **Google Drive** under ISMS records.
- Retained for **3 years** as audit evidence.




---

# ISMS Performance Metrics

## 1. Purpose

This section defines key **performance indicators (KPIs)** to measure the effectiveness of Rate's ISMS in alignment with its **information security objectives**, as required by **ISO/IEC 27001:2022 Clause 9.1**.

## 2. Metrics and Alignment with Objectives (KPI)

| **Metric**                    | **Description**                                                                 | **Target**              | **Related ISMS Objective**                                      | **Review Frequency** |
|------------------------------|---------------------------------------------------------------------------------|--------------------------|------------------------------------------------------------------|----------------------|
| Security Awareness Completion | Percentage of employees who completed training                                 | 100%                     | All employees complete annual awareness training                | Annually             |
| Backup Integrity              | Success rate of monthly backup restorations                                     | ≥ 90%                    | Backups tested monthly with at least 90% success rate           | Monthly              |
| Access Control Violations     | Number of unauthorized access attempts detected                                | 0 per year               | Limit unauthorized access incidents to zero                     | Annually             |
| Incident Response Time        | Time taken to contain and resolve security incidents                           | < 4 hours                | Ensure quick response to security events                        | Annually             |
| User Access Reviews           | Percentage of systems reviewed for access permissions annually                 | 100%                     | Annual access review for all systems                            | Annually             |
| Audit Non-Conformities        | Number of major non-conformities found during internal audits                  | 0 major issues           | Complete annual internal audit and resolve findings in 30 days  | Annually             |

## 3. Reporting and Review

- The **Managing Director** compiles ISMS performance reports annually.
- Metrics are reviewed during **Management Review Meetings**.
- If KPIs fall below targets, **corrective actions** are initiated and logged.




# ISMS Review & Approval Log

This log tracks the review and approval history of all core ISMS documents and policies, including who reviewed them, when they were last approved, whether formal approval is required. This ensures traceability, accountability, and compliance with ISO/IEC 27001:2022.

| Section/Policy                             | Last Reviewed | Reviewed By         |  Requires Approval | Approved By       | Approval Date | Status        | Notes                                                    |
|-------------------------------------------|---------------|----------------------|--------------------|--------------------|----------------|---------------|----------------------------------------------------------|
| Information Security Policy               | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Policy aligns with ISO 27001; no changes needed         |
| Access Control Policy                     | 2025-05-16    | Team Lead Developer  |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Covers all access processes; onboarding flow clarified  |
| Incident Management & Response Plan       | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | PIR and reporting procedures confirmed                   |
| BCDR Plan                                 | 2025-05-16    | Team Lead Developer  |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Testing, failover, and contact details reviewed          |
| Asset Management Policy                   | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Asset classification and retention verified              |
| Secure Development & Change Management    | 2025-05-16    | Team Lead Developer  |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Dev process, approvals, and versioning validated         |
| Risk Assessment & Treatment Plan          | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Risk matrix, SoA mapping, and treatments are complete    |
| Statement of Applicability (SoA)          | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Controls mapped and exclusions justified                 |
| Legal & Regulatory Compliance             | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Laws, ISO clauses, and contract requirements reviewed    |
| Privacy & Data Protection Policy          | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | GDPR rights handling and retention confirmed             |
| Supplier Security & Contractual Oblig.    | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | supplier list, clauses, and reviews up to date             |
| Internal Audit Program                    | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Scope, independence, and findings process reviewed       |
| Corrective Actions & Non-Compliance Log   | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Log format, deadlines, and responsibilities confirmed     |
| Management Review                         | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | Agenda, outcomes, and meeting notes process verified     |
| ISMS Performance Metrics                  | 2025-05-16    | Managing Director    |  ✅ Yes              | CEO                | 2025-05-19     | ✅ Approved    | KPIs aligned with ISMS goals and tracked annually        |



---

# ISMS Annual Audit Calendar

| Date                   | Activity                                      | Owner                   | Frequency           |
|------------------------|-----------------------------------------------|-------------------------|---------------------|
| May 20                 | Security Awareness Training                   | Managing Director       | Annual              |
| Jun 01                 | Review ISMS Performance Metrics               | Managing Director       | Annual              |
| Jul 01                 | Access Control Review                         | Team Lead Developer     | Annual/ when some one leaves              |
| Jul 05                 | supplier Security Reviews                       | Team Lead Developer     | Annual              |
| **10th of every month**| Backup Restore Test                           | Team Lead Developer     | Monthly             |
| Jun 16                 | Internal ISO 27001 Audit                      | Managing Director       | Annual              |
| Jun 24                 | Management Review Meeting                     | CEO & Managing Director | Annual              |
| Jul 25, Feb 25         | Lastpass full backup to NAS                    | CEO & Managing Director | Annual              |
| Jul 25                 | Business Continuity & Disaster Recovery Drill (Including lastpass recovery) | CEO & Managing Director | Annual              |




