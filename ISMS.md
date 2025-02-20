# Information Security Management System (ISMS) Manual  

## 1. Introduction
   - Purpose and Objectives of the ISMS
   - Scope of the ISMS
   - Definitions and Abbreviations

## 2. Core ISMS Documents
   - Information Security Policy   
   - Risk Assessment and Risk Treatment Plan
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
  - Approve risk assessments and the Risk Treatment Plan (RTP).
  - Oversee **incident management and resolution** for critical security incidents.
  - Ensure periodic **reviews of security incidents and ISMS effectiveness**.

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

### 4.3. Team Lead Developer

- **Accountability**: Ensures secure software development practices and cybersecurity risk mitigation.
- **Responsibilities**:
  - Lead the development team in implementing secure coding practices and ensuring software security.
  - Enforce security policies within the software development lifecycle.
  - Conduct periodic code reviews and security assessments to identify vulnerabilities.
  - Manage and monitor security compliance related to development infrastructure.
  - Ensure **SSL certificate renewal** is managed through **automatic renewal or alerts**.
  - Investigate and provide technical remediation for **security incidents** affecting development environments.

### 4.4. Developers

- **Accountability**: Implement secure coding practices and access controls.
- **Responsibilities**:
  - Follow secure coding standards and guidelines.
  - Enforce access control and authentication processes within the development environment.
  - Support security compliance by maintaining documentation and adhering to best practices.
  - Identify and report potential software vulnerabilities to the Team Lead Developer.
  - Assist in responding to security incidents by providing technical expertise and remediation support.
  - Implement and enforce **access control measures** in compliance with **Annex A.9**.

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
- Monitoring and reviewing risks **annually and after significant security incidents or infrastructure changes**.

## 7. Access Control

In accordance with **Annex A.9 - Access Control**, Rate enforces the following security measures:

- **Role-based access control (RBAC)** is implemented for all systems.
- **Firewall rules and VPN access restrictions** are enforced to protect critical infrastructure.
- **Alternative access methods** to production servers are maintained to ensure availability in case of VPN failures.

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

**Approved by**: [CEO Name]  
**Date**: [Approval Date]

---
# Risk Assessment and Risk Treatment Plan

This document outlines the identified risks, their likelihood and impact, and the appropriate risk treatment actions in accordance with **ISO 27001:2022**.

---

## **1. Risk Categorization**

### **1.1 Data Security Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Unauthorized access to customer database** | Medium | High | Developers | Mitigate | Enforce strict **access controls** using a **firewall** and strong authentication mechanisms. | A.9 Access Control | Acceptable if **strong passwords are enforced and the firewall is active**. |
| **Data loss from a server crash** | Medium | High | Developers | Mitigate | Ensure **automatic backups** to NAS and **perform regular backup tests**. | A.12 Backup Policy | Acceptable if **offsite backups are tested annually**. |
| **Insider threats (employee mishandling data)** | Low | High | Managing Director | Mitigate | Implement **role-based access control (RBAC)** and log all sensitive actions. | A.7 Human Resource Security | Acceptable if **RBAC is enforced & reviewed annually**. |

---

### **1.2 Infrastructure Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Server crash causing service disruption** | Medium | High | Developers | Mitigate | Implement **regular database and code backups**. Monitor server health and set **automated alerts**. | A.17 Business Continuity | Acceptable if **regular backups are performed and automatic alerts are configured**. |
| **Losing physical or internet access to head office (VPN, backups, development server)** | Medium | High | Developers | Mitigate | Ensure **production server firewall rules** can be modified securely **without VPN access**. Maintain **alternative access** methods. | A.13 Network Security | Acceptable if **alternative means of accessing production servers exist**. |
| **NAS Storage corruption or damage** | Medium | High | Tech Lead Developer | Mitigate | Conduct a **yearly backup integrity check**. | A.12 Backup Policy | Acceptable if **yearly backups pass integrity checks**. |

---

### **1.3 Human Resource Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Critical employee suddenly leaving** | Medium | Medium | Managing Director | Mitigate | Document **all key processes**, ensure **secure password storage**, and implement **role-based access restrictions**. | A.7 Human Resource Security | Acceptable if **a knowledge base is maintained and access controls are enforced**. |
| **Developer’s laptop lost, stolen, or damaged** | Medium | Medium | Tech Lead Developer | Mitigate | Enforce **cloud-based storage with encryption** and use **secure password managers**. | A.8 Asset Management | Acceptable if **all critical data is securely stored in the cloud**. |

---

### **1.4 Cybersecurity Risks**
| **Risk** | **Likelihood** | **Impact** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Reference** | **Risk Acceptance Criteria** |
|---|---|---|---|---|---|---|---|
| **Virus or ransomware attack on company devices** | Medium | Medium | Tech Lead Developer | Mitigate | Install **enterprise-grade antivirus software**, enable **automatic updates**, and conduct **regular security training**. | A.12 Malware Protection | Acceptable if **endpoint protection is always enabled and updated**. |
| **Losing access to LastPass (password manager)** | Low | High | CEO | Mitigate | Maintain a **bi-yearly backup of critical passwords** in an **encrypted and secure location**. | A.9 Access Control | Acceptable if **backup plan is tested annually**. |
| **SSL certificate expiry for platform or website** | High | Medium | Tech Lead Developer | Mitigate | Enable **automatic SSL renewal** or set up **early expiration alerts**. | A.14 System Security | Acceptable if **automatic renewal is active or renewal reminders are in place**. |

---

## **2. Risk Review and Approval**
- **Risk Assessment Reviewed By:** Managing Director  
- **Risk Treatment Plan Approved By:** CEO  
- **Date of Last Review:** [Insert Date]  

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
- The Tech Lead provisions access and conducts **annual access reviews**.
- Developers are responsible for ensuring secure implementation of access control measures within the systems they develop.
- Records are maintained for audit purposes.

## 5. Authentication and Password Management
- **Password Policy:** Minimum 12 characters, 90-day expiration, and secure storage in LastPass.

## 6. Monitoring and Logging
- **Logs:** Collected from all on-premises and cloud systems.
- **Review Frequency:** The Tech Lead reviews logs annually.
- **Retention:** Logs are retained for at least one year.

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
- **Tech Lead:** Manages access, reviews logs annually, and oversees configurations.
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
- **Annual backup testing is required** to ensure reliability, in alignment with the Risk Treatment Plan (RTP).

## 6. Documentation and Reporting
- All incidents must be logged, including:
  - Incident ID
  - Date and time of detection
  - Description and impact
  - Actions taken
  - Resolution date
- Incident logs are maintained for at least **3 years** in Google Drive.

## 7. Roles and Responsibilities
### **7.1. Employees**
- Report security incidents immediately.
- Cooperate with investigations and follow security protocols.

### **7.2. Tech Lead**
- Leads **technical containment and resolution** of incidents.
- Reviews and maintains incident logs.
- Coordinates security improvements post-incident.

### **7.3. Managing Director**
- **Leads overall incident response efforts**, ensuring proper execution of containment, eradication, and recovery steps.
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
- **Incident reviews are conducted annually** to match the Risk Treatment Plan (RTP).

## 10. Compliance and Reporting
- Incident logs are retained for **3 years** in Google Drive.
- The plan adheres to **ISO/IEC 27001:2022** and **GDPR** requirements.

*Note: Employees will be notified of policy updates.*


---

# Business Continuity and Disaster Recovery Plan (BCDRP)  
**Aligned with ISO/IEC 27001:2022 and Integrated with Risk Assessment and Treatment Plan**  


## **1. Purpose**  
This plan outlines procedures for maintaining business operations and recovering from disruptions at **Rate**, ensuring continuity of services and rapid recovery from disasters. It incorporates controls from the Risk Assessment and Treatment Plan (RARTP).


## **2. Scope**  
Covers all systems, employees, cloud services, and processes supporting **Rate's platform and operations**.  


## **3. Key Contacts**  
- **Disaster Recovery Team:**  
  - **CEO (Head)** – Primary decision-maker  
  - **Managing Director** – Operations and communications  
  - **Team Lead Developer** – Technical recovery lead  
- **Contact Email:** info@rate.nl  
- **Emergency Contact Phone Number:** 010 – 822 52 22  


## **4. Critical Systems and Dependencies**  
| **System/Service** | **Provider** | **Backup Location** | **RTO** | **RPO** | **Owner** |
|--------------------|-------------|-------------------|--------|--------|---------|
| **Production Hosting** | Hetzner (Primary) | NAS & Cloud | 4 hours | 30 minutes | Team Lead Developer |
| **Secondary Hosting (Provider Failure)** | Azure | Cloud | 4 hours | 30 minutes | Team Lead Developer |
| **Source Code Repository** | GitHub | Cloud with integrity checks | 1 hour | Real-time | Team Lead Developer |
| **Backups** | NAS (Remote) & Cloud | Monthly restoration tests | N/A | 30 minutes | Team Lead Developer |
| **VPN & Remote Access** | Local VPN on Dev Server | N/A | Immediate | None | Managing Director |
| **Communication Tools** | Google Workspace (email, docs) | Google Cloud | Immediate | None | Managing Director |
| **HR and Compliance System** | Exact Online | Cloud | 2 hours | 1 hour | Managing Director |
| **Password Manager** | LastPass | Encrypted Cloud | 1 hour | 30 minutes | CEO |


## **5. Backup and Recovery Procedures**  
### **5.1 Database Backups (Critical)**
- **Full Daily Backup:** 03:00 (retained 1 month) – Stored on NAS and cloud  
- **Incremental Backups:** Every 4 hours (retained 1 month)  
- **Transaction Log Backups:** Every 30 minutes (retained 1 month)  
- **Testing:** Monthly restoration from backups with documentation of results  

### **5.2 Production Application Folder Backups**  
- **Full Daily Backup:** 03:00 (retained 1 month) – Stored on NAS and cloud  
- **Testing:** Monthly restoration and integrity checks  

### **5.3 Source Code Backups**  
- **Managed In:** GitHub with real-time synchronization  
- **Testing:** Quarterly integrity verification (hash checks)  

### **5.4 Backup Retention Policy:**  
- **Location:** NAS (remote) and cloud storage  
- **Retention Period:** 1 month for backups, 3 years for logs  
- **Backup Logs Storage:** Google Drive (retained for 3 years)  



## **6. Disaster Scenarios, RTO, and RPO**  
| **Scenario** | **Action Plan** | **Lead** | **RTO (Recovery Time Objective)** | **RPO (Recovery Point Objective)** |
|--------------|----------------|----------|----------------------------------|-----------------------------------|
| **6.1 Production Server Failure (Hetzner)** | Provision a new Hetzner server, restore from repository backups | Team Lead Developer | 4 hours | 30 minutes |
| **6.2 Cloud Provider Failure (Hetzner Unavailable)** | Deploy server on Azure, restore backups, notify customers | Team Lead Developer | 4 hours | 30 minutes |
| **6.3 Office Internet Outage** | Enable remote work via VPN and Google Workspace | Managing Director | Immediate | None |
| **6.4 Data Leak or Malware Attack** | Isolate systems, notify Managing Director, conduct forensic analysis | Managing Director | 2 hours | 30 minutes |
| **6.5 Calamities (Fire, Flood, Physical Theft)** | Follow Groothandelsgebouw escape plan, secure backups offsite | CEO | As feasible | 30 minutes |
| **6.6 Loss of LastPass (Password Manager)** | Restore from encrypted cloud backup, reset passwords for critical systems | CEO | 1 hour | 30 minutes |
| **6.7 SSL Certificate Expiry for Website/Platform** | Enable auto-renewals, set calendar reminders for manual renewal checks | Team Lead Developer | 1 hour | None |


## **7. Roles and Responsibilities**  
| **Role** | **Responsibilities During Disaster** |
|----------|-----------------------------------|
| **CEO (Head of Disaster Recovery Team)** | Authorizes major decisions, communicates with customers and stakeholders |
| **Managing Director** | Oversees recovery operations, manages communications, maintains incident logs |
| **Team Lead Developer** | Executes technical recovery steps, restores servers, maintains backup records |
| **All Employees** | Follow the BCDRP procedures and report security incidents immediately |


## **8. Testing and Review (ISO Clause 8.1 & 9.1)**  
- **Testing Frequency:** Annually (full disaster recovery drill) with monthly backup restoration tests  
- **Test Components:** Server restoration, VPN failover, LastPass recovery, SSL certificate renewal  
- **Documentation:** Maintain test results and lessons learned on Google Drive for 3 years  
- **Review Cycle:** Annually or after any major incident or infrastructure change  
- **Responsible for Testing:** Managing Director  
- **Responsible for Documentation:** Team Lead Developer  


## **9. Continuous Improvement and Lessons Learned (ISO Clause 10.2)**  
- **After-Action Reports (AAR):** Produced after every disaster recovery test or real incident  
- **Lessons Learned:** Logged and reviewed quarterly during ISMS management meetings  
- **Plan Updates:** Adjust BCDRP based on lessons learned and new threats  
- **Plan Review Frequency:** Annual or after significant infrastructure changes  
- **Plan Approver:** CEO  


## **10. Compliance and Recordkeeping (ISO Clause 9.2 & 9.3)**  
| **Record** | **Retention Period** | **Storage Location** | **Responsible Owner** |
|------------|--------------------|---------------------|---------------------|
| Backup Logs | 3 years | Google Drive | Team Lead Developer |
| Incident Logs | 3 years | Google Drive | Managing Director |
| Disaster Recovery Test Reports | 3 years | Google Drive | Managing Director |
| Residual Risk Approvals | 3 years | Google Drive | CEO |
| ISMS Management Review Records | 3 years | Google Drive | Managing Director |

### **Compliance with Standards:**  
 **ISO/IEC 27001:2022** (Clauses 8.1, 9.1, 9.2, 9.3, 10.2)  
 **GDPR (Article 32: Security of Processing)**  



## **11. Review and Approval**  
- **Reviewed By:** Managing Director  
- **Approved By:** CEO  
- **Date of Last Review:** [Insert Date]  
- **Next Scheduled Review:** [Insert Date]  


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
