# Information Security Management System (ISMS) Manual  

## 1. Introduction
   - Purpose and Objectives of the ISMS
   - Scope of the ISMS
   - Definitions and Abbreviations

## 2. Core ISMS Documents
   - Information Security Policy   
   - Risk Assessment and Risk Treatment Process
   - Risk Treatment Plan
   - Access Control Policy
   - Incident Management and Response Plan
   - Business Continuity and Disaster Recovery Plan
   - Asset Management and Data Protection Policy

## 3. Statement of Applicability



## 4. Compliance and Performance Monitoring
   - Legal and Regulatory Compliance
   - Internal Audits and Continuous Improvement
   - Nonconformities and Corrective Actions
   - Performance Measurement and Management Reviews

## 5. Annexes and Supporting Documents
   - List of Policies and Procedures
   - Risk Assessment and Treatment Records
   - Audit and Review Reports
   - Any Other Supporting Documentation


---


## 1. Introduction

### Purpose and Objectives of the ISMS

Rate is committed to safeguarding the confidentiality, integrity, and availability of all physical and electronic information assets. Our Information Security Management System (ISMS) is designed to manage information security risks effectively, ensuring business continuity and minimizing potential threats.

## Scope of the ISMS

The ISMS encompasses all processes, systems, and personnel involved in the development, maintenance, and delivery of our survey platform services. This includes:

- **Physical Location:** Our single office premises.
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

Rate is committed to:

- Protecting information assets against unauthorized access, disclosure, alteration, or destruction.
- Ensuring the availability of information to authorized users when needed.
- Complying with applicable legal, regulatory, and contractual obligations.
- Continually improving the Information Security Management System (ISMS).

## 4. Roles and Responsibilities

In accordance with ISO/IEC 27001:2022 Clause 5.3 and Annex A.5.2, the following roles and responsibilities are defined:

### 4.1. Chief Executive Officer (CEO)

- **Accountability**: Holds overall accountability for the ISMS.
- **Responsibilities**:
  - Ensure strategic alignment of the ISMS with business objectives.
  - Provide necessary resources for ISMS implementation and maintenance.
  - Promote a culture of information security within the organization.
  - Oversee compliance with regulatory and security standards.

### 4.2. Managing Director

- **Accountability**: Oversees the implementation and operation of the ISMS.
- **Responsibilities**:
  - Develop and maintain information security policies and procedures.
  - Conduct organization-wide risk assessments and manage risk treatment plans.
  - Ensure compliance with information security policies and applicable laws.
  - Report ISMS performance to top management.
  - Support operational security measures and access control strategies.

### 4.3. Team Lead Developer

- **Accountability**: Ensures secure software development practices.
- **Responsibilities**:
  - Lead the development team in implementing secure coding practices and ensuring software security.
  - Enforce security policies within the software development lifecycle.
  - Conduct periodic code reviews and security assessments to identify vulnerabilities.
  - Manage and monitor security compliance related to development infrastructure.
  - Act as a point of contact for security incidents related to software and development infrastructure.

### 4.4. Developers

- **Accountability**: Implement secure coding practices.
- **Responsibilities**:
  - Follow secure coding standards and guidelines.
  - Assist in enforcing access control and authentication processes within the development environment.
  - Support security compliance by maintaining documentation and adhering to best practices.
  - Identify and report potential software vulnerabilities to the Team Lead Developer.
  - Assist in responding to security incidents by providing technical expertise and remediation support.

### 4.5. All Employees

- **Accountability**: Adhere to information security policies and procedures.
- **Responsibilities**:
  - Protect information assets within their control.
  - Report security incidents or weaknesses promptly.
  - Participate in information security training and awareness programs.


## 5. Information Security Principles

Rate adopts the following principles to guide its information security efforts:

- **Confidentiality**: Ensuring that information is accessible only to those authorized to have access.
- **Integrity**: Safeguarding the accuracy and completeness of information and processing methods.
- **Availability**: Ensuring that authorized users have access to information and associated assets when required.

## 6. Risk Management

Rate will implement a risk management process that includes:

- Identifying information security risks.
- Assessing the potential impact and likelihood of risks.
- Implementing appropriate controls to mitigate risks.
- Monitoring and reviewing risks regularly.

## 7. Compliance

Rate is committed to complying with all applicable legal, regulatory, and contractual requirements related to information security. This includes, but is not limited to, data protection laws and industry standards.

## 8. Management Commitment

In alignment with ISO/IEC 27001:2022 Clause 5.1, Rate's top management is committed to:

- Continual improvement of the ISMS to enhance information security performance.
- Providing adequate resources to establish, implement, maintain, and improve the ISMS.
- Integrating information security requirements into the organization's processes and strategic direction.

## 9. Incident Reporting and Response

In accordance with ISO/IEC 27001:2022 Clause 16.1.1, Rate has established a formal Incident Response Plan (IRP) that includes:

- **Incident Identification**: All employees are responsible for reporting suspected information security incidents immediately to the Information Security Manager (ISM).
- **Incident Classification**: The ISM will assess and classify the incident based on its severity and impact.
- **Incident Escalation**: Significant incidents will be escalated to the Managing Director and, if necessary, to the CEO and Security Committee.
- **Incident Resolution**: The ISM, in collaboration with relevant personnel, will coordinate the response to and resolution of the incident.
- **Post-Incident Review**: After resolution, a review will be conducted to identify lessons learned and implement improvements to prevent recurrence.

## 10. Policy Review and Approval

In compliance with ISO/IEC 27001:2022 Clause 5.1.2, this Information Security Policy shall be:

- **Reviewed**: The Information Security Manager (ISM) is responsible for reviewing this policy at least annually or when significant changes occur.
- **Approved**: The policy must be approved by the Chief Executive Officer (CEO) and the Security Committee to ensure its relevance and effectiveness.

**Approved by**: [CEO Name]

**Date**: [Approval Date]

---

# Risk Assessment and Risk Treatment Process

This document outlines the identified risks, their likelihood and impact, and the appropriate risk treatment actions in accordance with **ISO 27001:2022**.


## **1. Risk Categorization**

### **1.1 Data Security Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Unauthorized access to customer database** | Medium | High | Managing Director | Mitigate | Enforce **MFA**, strict **access controls**, and database **access logging**. | A.9 Access Control | Risk is acceptable if **all access logs are monitored** and **MFA is enforced**. |
| **Data loss from a server crash** | Medium | High | Tech Lead Developer | Mitigate | Ensure **automatic backups** to NAS and cloud storage. Perform **regular backup tests**. | A.12 Backup Policy | Acceptable if **offsite backup is tested monthly**. |
| **Insider threats (employee mishandling data)** | Low | High | Managing Director | Mitigate | Implement **role-based access control (RBAC)** and log all sensitive actions. Conduct **employee security training**. | A.7 Human Resource Security | Acceptable if **RBAC is enforced & logs are reviewed quarterly**. |


### **1.2 Infrastructure Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Server crash causing service disruption** | Medium | High | Tech Lead Developer | Mitigate | Deploy **failover server** on Hetzner. Monitor server health. Implement **automated alerts**. | A.17 Business Continuity | Acceptable if **failover system is tested quarterly**. |
| **Losing physical or internet access to head office (VPN, backups, development server)** | Medium | High | Managing Director | Mitigate | Configure **alternative VPN access** (e.g., cloud-based VPN, backup ISP). Maintain **offsite backups**. | A.13 Network Security | Acceptable if **backup ISP & VPN alternative is in place**. |
| **NAS Storage corruption or damage** | Medium | High | Tech Lead Developer | Mitigate | Implement **RAID** for redundancy, conduct **monthly backup integrity checks**. | A.12 Backup Policy | Acceptable if **RAID & offsite backups are maintained**. |


### **1.3 Human Resource Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Critical employee suddenly leaving** | Medium | Medium | Managing Director | Mitigate | Document **all key processes**, ensure **passwords are stored securely** and access controls prevent single-person dependency. | A.7 Human Resource Security | Acceptable if **knowledge transfer plan is in place**. |
| **Developer’s laptop lost, stolen, or damaged** | Medium | Medium | Tech Lead Developer | Mitigate | Enforce **full disk encryption**, **remote wipe capabilities**, and strong **device access controls**. | A.8 Asset Management | Acceptable if **encryption & remote wipe are enforced**. |


### **1.4 Cybersecurity Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Virus or ransomware attack on company devices** | Medium | High | Tech Lead Developer | Mitigate | Install **endpoint protection**, enable **automatic updates**, enforce **least privilege access**, and conduct **phishing training**. | A.12 Malware Protection | Acceptable if **endpoint protection is always updated**. |
| **Losing access to LastPass (password manager)** | Low | High | Managing Director | Mitigate | Maintain a **backup of critical passwords** in a separate, **secure** location (e.g., encrypted cloud storage). Use **offline password vault** as a backup. | A.9 Access Control | Acceptable if **backup plan is tested annually**. |
| **LastPass breach (exposing all stored passwords)** | Low | High | Managing Director | Mitigate | Enable **zero-knowledge encryption**, enforce **strong unique passwords**, rotate passwords periodically. Consider **an alternative password manager** for redundancy. | A.9 Access Control | Acceptable if **password rotation & secondary storage is in place**. |
| **SSL certificate expiry for platform or website** | High | Medium | Tech Lead Developer | Mitigate | Enable **automatic SSL renewal** with monitoring alerts. Track expiration dates with reminders. | A.14 System Security | Acceptable if **automatic renewal & monitoring alerts are active**. |


## **2. Risk Review and Approval**
- **Risk Assessment Reviewed By:** Managing Director  
- **Risk Treatment Plan Approved By:** CEO  
- **Date of Last Review:** [Insert Date]  

This document will be **reviewed annually** and after any significant changes to our infrastructure, services, or risk landscape.


## **Next Steps**
- Monitor and update this risk register **at least once per year**.  
- Implement periodic **risk assessments** and track mitigation progress.  
- Ensure security awareness training aligns with identified risks.

---


# Risk Treatment Plan (RTP)

## 1. Purpose
This Risk Treatment Plan (RTP) outlines the actions required to mitigate identified risks to Rate’s information security assets. It aligns with the **ISO 27001:2022** standard, specifically Clause **6.1.3(d)**, and ensures that appropriate security controls are implemented, assigned, and monitored.

## 2. Risk Treatment Overview
This plan is based on the **Risk Assessment and Risk Treatment Process**, which identified key security risks and their impact on Rate’s operations. Each risk treatment action is assigned a responsible owner, implementation deadline, and approval status.

## 3. Risk Treatment Plan Table

| **Risk** | **Treatment Option** | **Mitigation Actions** | **Responsible Person** | **Implementation Deadline** | **Status** |
|---|---|---|---|---|---|
| Unauthorized access to customer database | Mitigate | Enforce **MFA**, strict **access controls**, and **database access logging** | CTO | [Date] | Pending |
| Data loss from a server crash | Mitigate | Ensure **automatic backups** to NAS and cloud storage, test backups periodically | IT Manager | [Date] | Pending |
| Insider threats (employee mishandling data) | Mitigate | Implement **RBAC**, log sensitive actions, conduct **employee security training** | Security Officer | [Date] | Pending |
| Third-party service breaches (Trello, Freshdesk, etc.) | Mitigate | Restrict sharing of sensitive data, enable **MFA**, and review security settings | Security Officer | [Date] | Pending |
| Server crash causing service disruption | Mitigate | Deploy **failover server** on Hetzner, monitor server health, implement **automated alerts** | IT Manager | [Date] | Pending |
| Losing access to head office (VPN, backups, development server) | Mitigate | Configure **alternative VPN access**, maintain **offsite backup** | IT Manager | [Date] | Pending |
| NAS Storage corruption or damage | Mitigate | Implement **RAID**, conduct **monthly backup integrity checks** | IT Manager | [Date] | Pending |
| Critical employee suddenly leaving | Mitigate | Document **key processes**, ensure **password manager access control** | HR Manager | [Date] | Pending |
| Developer’s laptop lost, stolen, or damaged | Mitigate | Enforce **full disk encryption**, **remote wipe**, and strong **device access controls** | Security Officer | [Date] | Pending |
| Virus or ransomware attack | Mitigate | Install **endpoint protection**, enforce **automatic updates**, **least privilege access**, phishing training | IT Manager | [Date] | Pending |
| Losing access to LastPass (password manager) | Mitigate | Maintain **backup of critical passwords** in **secure location**, use **offline vault** | Security Officer | [Date] | Pending |
| LastPass breach (exposing passwords) | Mitigate | Enable **zero-knowledge encryption**, enforce **password rotation**, consider **alternative password manager** | Security Officer | [Date] | Pending |
| SSL certificate expiry for platform | Mitigate | Enable **automatic SSL renewal**, monitor expiration dates | IT Manager | [Date] | Pending |

## 4. Review and Approval
This Risk Treatment Plan is subject to **annual review** and updates whenever there are significant changes to Rate’s infrastructure, business operations, or security landscape.

- **Reviewed by:** [Security Officer Name]  
- **Approved by:** [CEO Name]  
- **Date of Approval:** [Insert Date]  
- **Next Review Date:** [Insert Date]  

## 5. Monitoring and Follow-Up
The security team will track progress on all risk treatments and ensure timely implementation of each mitigation action. Any delays or deviations will be documented and addressed in security management meetings.

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
  - WiFi Networks: "Rate.nl employee," "Rate.nl guest," and "KH_OFFICES"
- **Cloud Applications and Providers:** Google Drive, Google Workspace, GitHub, Stack Overflow, Exact Online, WordPress, and Hetzner Cloud
- **Remote Access Systems:** Remote Desktop Server, Local VPN (Hetzner), and employee-managed laptops


## 3. Access Control Principles
- **Least Privilege:** Limit access to the minimum necessary for tasks.
- **Need-to-Know:** Restrict sensitive data access.
- **Role-Based Access Control (RBAC):** Assign permissions based on job roles.
- **Separation of Duties:** Divide security-sensitive responsibilities.


## 4. User Access Management
### **4.1. Registration and De-registration**
- **Registration:** Requests are submitted to the Tech Lead via email. CEO approval is required for high-privilege access. Requests are stored in email records, which serve as documentation.
- **De-registration:** The CEO instructs the Tech Lead via email to revoke access upon role change or departure.
- **Documentation:** Access approvals and removals are retained in email records.

### **4.2. Provisioning and Review**
- The Tech Lead provisions access and conducts quarterly access reviews.
- Records are maintained for audit purposes.


## 5. Authentication and Password Management
- **2FA Implementation:**
  - **Cloud Apps (e.g., Google Workspace, GitHub):** SSO with 2FA
- **Password Policy:** Minimum 12 characters, 90-day expiration, and secure storage in LastPass


## 6. Monitoring and Logging
- **Logs:** Collected from all on-premises and cloud systems.
- **Review Frequency:** The Tech Lead reviews logs quarterly.
- **Retention:** Logs are retained for at least one year.


## 7. Third-Party and Cloud Access Control
- Third-party access is not currently granted.
- Cloud administrators are the Tech Lead and Managing Director.
- Cloud provider security settings are configured to standard compliance.


## 8. Physical Access Control
- Building entry requires key card access.
- Office access is secured by key.
- NAS and Development Server are stored under lock.
- Production servers are cloud-hosted on Hetzner.


## 9. Responsibilities
- **Tech Lead:** Manages access, reviews logs quarterly, and oversees configurations.
- **CEO:** Approves sensitive access requests and enforces compliance.
- **All Employees:** Maintain laptop security and promptly report incidents.


## 10. Policy Review
The policy undergoes annual review or immediate revision after major changes.

## 11. Compliance
Non-compliance may result in disciplinary actions or legal consequences.

*Note: Employees will be notified of all policy updates.*


---


# Incident Management and Response plan

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
- Employees must report incidents immediately via email to the Tech Lead.
- High-severity incidents should be escalated to the CEO and Managing Director.
- Incident details should include date, time, affected systems, and a brief description.

### **4.2. External Reporting**
- If customer data is affected, the CEO will communicate with impacted parties.
- Regulatory bodies (e.g., GDPR authorities) will be notified if required by law.

## 5. Incident Response Phases
### **5.1. Identification**
- Incidents are detected through system monitoring, employee reports, and automated alerts.
- The Tech Lead reviews logs from cloud providers (Google Workspace, Hetzner) and on-premises systems.

### **5.2. Containment**
- Immediate actions include disabling compromised accounts and revoking VPN access.
- Affected devices should be isolated from corporate networks.

### **5.3. Eradication**
- The root cause of the incident is identified and mitigated.
- Systems are patched, malware is removed, and security gaps are addressed.

### **5.4. Recovery**
- Systems are restored from backups, and normal operations resume.
- Data integrity is verified on Google Drive, Exact Online, and production servers.

### **5.5. Lessons Learned**
- A post-incident review is conducted to document findings and update policies.
- Security improvements are implemented to prevent recurrence.

## 6. Documentation and Reporting
- All incidents must be logged, including:
  - Incident ID
  - Date and time of detection
  - Description and impact
  - Actions taken
  - Resolution date
- Incident logs are maintained for at least **3 years** in Google Drive.
- Reports are reviewed quarterly to identify trends and improve response efforts.

## 7. Roles and Responsibilities
### **7.1. Employees**
- Report security incidents immediately.
- Cooperate with investigations and follow security protocols.

### **7.2. Tech Lead**
- Leads incident detection, containment, and resolution.
- Reviews and maintains incident logs.
- Coordinates security improvements post-incident.

### **7.3. Managing Director**
- Assists in response when the Tech Lead is unavailable.
- Supports log analysis and recovery processes.

### **7.4. CEO**
- Approves major response actions and external reporting.
- Oversees communication with stakeholders and regulatory bodies.

## 8. Communication Plan
- **Internal:** Tech Lead provides updates via email to the CEO and relevant teams.
- **External:** The CEO handles customer notifications and regulatory compliance communication.

## 9. Plan Review and Testing
- The plan is reviewed **annually** or after major incidents.
- Incident response simulations are conducted **bi-annually** to ensure readiness.

## 10. Compliance and Reporting
- Incident logs are retained for **3 years** in Google Drive.
- The plan adheres to **ISO/IEC 27001:2022** and **GDPR** requirements.


*Note: Employees will be notified of policy updates.*

---

# Business Continuity and Disaster Recovery Plan

## 1. Purpose
This plan outlines procedures for maintaining business operations and recovering from disruptions at Rate, ensuring continuity of services and rapid recovery from disasters.

## 2. Scope
Covers all systems, employees, and processes supporting Rate's platform and operations.

## 3. Key Contacts
- **Disaster Recovery Team:** CEO (Head), Managing Director, Team Lead Developer
- **Contact Email:** info@rate.nl
- **Emergency Contact Phone Number:** 010 – 822 52 22

## 4. Critical Systems
- **Cloud Hosting:** Hetzner (primary), Azure (secondary for provider failure)
- **Source Code:** Managed in GitHub
- **Backups:** Stored on NAS (remote) and cloud storage
- **Communication Tools:** Google Workspace (email, documents)

## 5. Backup and Recovery Procedures
- **Database:**
  - Full daily backup (03:00), retained for 1 month (NAS and cloud)
  - Incremental backups every 4 hours (retained 1 month)
  - Transaction log backups every 30 minutes
  - **Testing:** Monthly backup restoration tests
- **Production Folder:** Daily backups (NAS, retained 1 month, tested monthly)
- **Source Code:** Managed in GitHub with integrity checks

## 6. Disaster Scenarios, RTO, and RPO
### **6.1 Production Server Failure (Hetzner)**
- **Action:** Provision new Hetzner server and restore from repository backups
- **Lead:** Team Lead Developer
- **RTO (Recovery Time Objective):** 4 hours
- **RPO (Recovery Point Objective):** 30 minutes (via transaction logs)

### **6.2 Cloud Provider Failure (Hetzner Unavailable)**
- **Action:** Deploy new server on Azure, restore from backups, and notify customers
- **Lead:** Team Lead Developer
- **RTO:** 4 hours
- **RPO:** 30 minutes

### **6.3 Office Internet Outage**
- **Action:** Enable remote work via VPN and Google Workspace
- **Lead:** Managing Director
- **RTO:** Immediate
- **RPO:** None (cloud-based services)

### **6.4 Data Leak or Malware Attack**
- **Action:** Isolate systems, notify Managing Director, and conduct forensic analysis
- **Lead:** Managing Director
- **RTO:** 2 hours
- **RPO:** 30 minutes

### **6.5 Calamities (e.g., Fire, Flood)**
- **Action:** Follow building escape plan (Groothandelsgebouw) and secure backups
- **Lead:** CEO
- **RTO:** As feasible
- **RPO:** 30 minutes (via offsite backups)

## 7. Roles and Responsibilities
- **CEO:** Approves major actions and communicates with stakeholders.
- **Managing Director:** Oversees recovery operations and manages recordkeeping.
- **Team Lead Developer:** Executes technical recovery steps and maintains backup records.

## 8. Testing and Review
- **Testing:** Annual disaster recovery drills with backup restoration tests.
- **Review:** Annual updates or after major changes.
- **Lessons Learned:** Document findings from each test and address gaps.

## 9. Compliance and Recordkeeping
- **Backup Retention:** 1 month (NAS/cloud) — Team Lead Developer
- **Incident Logs:** Retained for 3 years (Google Drive) — Managing Director
- **Backup Testing Records:** Retained for 3 years — Team Lead Developer
- **Recordkeeping Oversight:** Managing Director
- **Compliance:** ISO/IEC 27001:2022, GDPR

*Last Updated: [Insert Date]*

---

# Asset Management and Data Protection Policy

## 1. Purpose
This policy defines procedures for managing and protecting Rate's information assets, ensuring compliance with ISO/IEC 27001:2022.

## 2. Scope
Applies to all digital, physical, and cloud-based assets accessed by Rate employees, contractors, and third parties.

## 3. Asset Inventory and Ownership
- **Asset Inventory:** Managed by the Managing Director, covering hardware, software, cloud services, and backups.
- **Asset Owners:** Responsible for security, maintenance, risk assessments, and classification.
- **Role Assignments:**
  - **Hardware:** Team Lead Developer.
  - **Software/Cloud Services:** Managing Director.
  - **Data (including backups):** Team Lead Developer and Asset Owners.
- **Documentation:** Logs include asset classification, ownership, and review records.

## 4. Acceptable Use and Protection Measures
- **Acceptable Use:** Annual acknowledgment of the Acceptable Use Policy is required.
- **Device Security:** Full disk encryption and automatic updates are mandatory.
- **Cloud Security:** 2FA is required for cloud service access.
- **Data Storage:** Role-based access controls protect sensitive data.
- **Backups:** Daily backups with monthly restoration tests.

## 5. Access Control and Data Security (Annex A.9)
- **Access Management:** Controlled by the Tech Lead with CEO approval for high-privilege roles.
- **Access Reviews:** Quarterly reviews by the Managing Director with findings logged.
- **Log Retention:** Access logs are retained for three years.
- **Access Revocation:** Immediate action for role changes or departures, with records documented.
- **Remote Access:** VPN is required for development server access.

## 6. Data Retention and Disposal (Annex A.8, A.11)
- **Retention Periods:** Backups retained for one month; incident logs for three years.
- **Secure Disposal:** Hardware is securely wiped and destroyed.
- **Disposal Records:** Logs include date, method, approver details, and retention for three years.

## 7. Monitoring and Review (Annex A.12, A.15)
- **Log Reviews:** Conducted quarterly, with results, corrective actions, and completion dates recorded.
- **Audit Documentation:** Managed by the Managing Director, documenting findings, corrective actions, and dates.
- **Policy Review:** Annually conducted with updates and actions logged.
- **Audit Record Retention:** All audit reports and supporting documents retained for three years.

## 8. Roles and Responsibilities (Annex A.7, A.6)
- **Managing Director:** Manages inventory, risk assessments, audit logs, and ensures Statement of Applicability (SoA) mappings are current.
- **Team Lead Developer:** Conducts asset reviews, oversees backups, and verifies disposal records.
- **Asset Owners:** Maintain classification records and ensure security controls are applied.
- **Employees:** Follow policies, annually acknowledge requirements, and report security issues.

## 9. Compliance (ISO/IEC 27001 Annex A Controls and SoA Mapping)
This policy aligns with ISO/IEC 27001:2022 Annex A controls, and their applicability is documented in the Statement of Applicability (SoA):
- **A.5:** Information Security Policies
- **A.6:** Organization of Information Security
- **A.7:** Human Resource Security
- **A.8:** Asset Management
- **A.9:** Access Control
- **A.11:** Physical and Environmental Security
- **A.12:** Operations Security (including audit records and corrective action logs)
- **A.15:** Supplier Relationships
- **A.18:** Compliance
- **SoA Link:** Refer to the current Statement of Applicability for specific mappings and control implementations.


*Last Updated: [Insert Date]*

---
