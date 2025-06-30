## 2. Risk Assessment

### 2.1. Data Security & Privacy Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 1 | Customer, Rate           | Developers, Managing Director | Data confidentiality, integrity, availability | Irresponsible handling or unauthorized access to customer/end-user data | Partially | Claims, reputational damage, loss of trust, regulatory penalties, possible termination of business relationship | High 🔴 | Medium 🟡 | High | A.5.13, A.5.20, A.8.3, A.8.12 |
| 2 | Rate employees           | Managing Director | Secure handling of employee data | Insider threats (employee mishandling data) | Partially | Confidential data exposure, compliance breach, reputational damage | High 🔴 | Low 🟢 | Medium | A.8.2, A.5.18, A.8.15 |
| 3 | Rate employees           | Rate              | Secure handling of HR, payroll, contracts | Mishandling of employee personal data (HR, payroll, contracts, ID) | Mostly | Claims, reputational damage, legal/regulatory penalties, loss of trust | High 🔴 | Medium 🟡 | High | A.5.13, A.6.1, A.8.3 |
| 4 | Respondent               | Rate              | Protection of survey/health data | Mishandling of respondent data (including health info) | Mostly | Claims, reputational damage, customer loss, regulatory penalties | High 🔴 | Medium 🟡 | High | A.5.13, A.8.3, A.8.12 |
| 5 | Rate                     | Rate              | Acceptable use of AI tools | Data leakage via AI tools (e.g., ChatGPT) | Partially | Business or personal data copied into external AI, leading to data breach | High 🔴 | Medium 🟡 | High | A.5.10, A.6.3 |

---

### 2.2. Platform, Infrastructure & Availability Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 6 | Rate                     | Developers, Team Lead Developer | Platform and data availability | Platform/server failure or data loss (internal & customer impact) | Mostly | Service/data unavailable, business interruption, customer/end-user dissatisfaction, reputational damage | High 🔴 | Medium 🟡 | High | A.8.12, A.8.16, A.17.1 |
| 7 | Rate                     | Developers        | Access to production systems | Losing access to head office systems | Partially | Inability to maintain/restore services, operational delays | High 🔴 | Medium 🟡 | High | A.8.20, A.7.4 |
| 8 | Rate                     | Team Lead Developer | Data backup integrity | NAS storage corruption or damage | Mostly | Loss of business data, inability to recover information | High 🔴 | Medium 🟡 | High | A.8.12 |
| 9 | Rate                     | Managing Director | Cloud service continuity | Cloud provider (Hetzner) suffers a major outage or data loss | Mostly | Loss of service and data availability, business interruption | High 🔴 | Low 🟢 | Medium | A.5.21, A.5.30 |
| 10 | Rate                    | Internet Provider | Internet connectivity | Internet provider outage or degradation | Mostly | Productivity loss, inability to access cloud/SaaS, customer impact | High 🔴 | Medium 🟡 | High | A.8.20, A.7.4 |
| 11 | Rate employees          | Rate              | Telework infrastructure | Telework infrastructure failure (VPN/device/connectivity) | Mostly | Productivity loss, delayed projects, inability to work remotely | High 🔴 | Medium 🟡 | High | A.5.10, A.8.1 |
| 12 | Trainer                 | Rate              | Training environment availability | Demo/training environment unavailable for trainers | Partially | Training cannot take place, onboarding and customer support delayed | High 🔴 | Medium 🟡 | High | A.8.20, A.8.16, A.17.1 |
| 13 | Rate                    | Developers        | Supported platform | Rate platform runs on unsupported/outdated Kentico version | Partially | Security vulnerabilities, data breach, compliance failure, high maintenance cost | High 🔴 | High 🔴 | High | A.8.9, A.8.25, A.8.27 |

---

### 2.3. Human Resource & Organizational Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 14 | Rate employees          | Managing Director | Knowledge retention, succession | Critical employee suddenly leaving | Partially | Loss of knowledge, operational inefficiency, delays | Medium 🟡 | Medium 🟡 | Medium | A.6.1 |
| 15 | Rate employees          | CEO / Managing Director | Leadership continuity | Sudden departure of CEO/MD | Mostly | Loss of leadership, possible loss of access to critical systems | High 🔴 | Low 🟢 | Medium | A.6.1, A.8.3 |
| 16 | Rate employees          | Employees         | Knowledge retention, training costs | High employee turnover leads to loss of knowledge and increased training costs | Partially | Increased costs, operational delays, possible security gaps during onboarding/offboarding | Medium 🟡 | Medium 🟡 | Medium | A.6.1, A.7.2 |

---

### 2.4. Endpoint, Device & Remote Work Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 17 | Rate employees          | Team Lead Developer | Device security | Developer’s laptop lost/stolen/damaged | Mostly | Loss of sensitive data, potential data breach | Medium 🟡 | Medium 🟡 | Medium | A.5.10, A.8.10 |
| 18 | Rate                    | Team Lead Developer | Data transfer security | Use of removable media (USB drives) for data transfer | Fully avoided | Data leakage, malware introduction | High 🔴 | Low 🟢 | Medium | A.8.10, A.8.12 |
| 19 | Rate employees          | Managing Director | Remote work security | Remote work leads to home network compromise | Mostly | Unauthorized access to company data via insecure home WiFi | High 🔴 | Medium 🟡 | High | A.6.7, A.8.1 |
| 20 | Rate employees          | Managing Director | Device management | Use of unmanaged/personal devices for company data (no AV, improper storage) | Partially | Malware infection, data breach, data leakage, device unusable | High 🔴 | Medium 🟡 | High | A.8.7, A.8.10 |

---

### 2.5. Cybersecurity & Access Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 21 | Rate                    | Team Lead Developer | Malware protection | Virus/ransomware attack on devices | Mostly | System compromise, data loss, downtime, financial loss | Medium 🟡 | Medium 🟡 | Medium | A.8.7, A.6.3 |
| 22 | Rate                    | CEO                | Password management | Losing access to LastPass | Mostly | Loss of access to critical credentials, operational disruption | High 🔴 | Low 🟢 | Medium | A.8.1, A.8.12 |
| 23 | Rate                    | Team Lead Developer | Certificate management | SSL certificate expiry | Mostly | Website/app inaccessible, loss of trust, possible data exposure | Medium 🟡 | High 🔴 | High | A.8.24, A.8.23 |
| 24 | Rate                    | Managing Director, Team Lead Developer | Cyber resilience | External attack (hacking, DDoS, etc.) disrupts business or leaks data | Mostly | Service downtime, data breach, reputational and financial loss | High 🔴 | Medium 🟡 | High | A.8.7, A.8.8, A.8.20 |
| 25 | Rate                    | Rate employees     | Policy compliance | Non-compliance with InfoSec policy/protocols | Partially | Security incident due to employee negligence or ignorance | High 🔴 | Medium 🟡 | High | A.7.2, A.7.3 |
| 26 | Rate                    | VPN Provider       | Remote access reliability | VPN connection unreliable or not auditable | Mostly | Claims, reputational damage, customer loss | High 🔴 | Medium 🟡 | High | A.8.20, A.5.21 |
| 27 | Rate                    | WiFi Provider      | Network access control | Unauthorized admin access via WiFi | Mostly | Unauthorized access, data breach | High 🔴 | Medium 🟡 | High | A.8.20, A.8.1 |
| 28 | Rate                    | Rate               | Authentication compliance | Unable to enforce 2FA (ISO/NEN requirement) | Partially | Data breach, loss of certification | High 🔴 | Medium 🟡 | High | A.8.1, A.8.3 |

---

### 2.6. Supplier, Contractual & Third-Party Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 29 | Rate                    | Managing Director | Supplier/third-party data protection | Supplier/third-party mishandling of sensitive data (hosting, payroll, trainers, CRM, support, Mailstreet, etc.) | Mostly | Claims, reputational damage, customer loss, regulatory penalties | High 🔴 | Medium 🟡 | High | A.5.19, A.5.20 |
| 30 | Rate                    | Security company, landlord, staff | Physical security | Physical intrusion (burglary) | Mostly | Unauthorized access to premises, theft or destruction of assets/information | High 🔴 | Medium 🟡 | High | A.7.1, A.7.2, A.7.3, A.7.4 |
| 31 | Rate                    | Security company, landlord | Fire safety | Fire prevention/detection failure | Mostly | Fire or smoke causes service interruption, loss of information/assets | High 🔴 | Medium 🟡 | High | A.7.5, A.7.8, A.7.11 |
| 32 | Rate                    | Security company, landlord | NAS security | Insufficient NAS security for health information | Partially | Unauthorized access to personal health data on NAS | High 🔴 | Medium 🟡 | High | A.8.10, A.8.12, A.8.3 |
| 33 | Customer                | Rate              | Contractual clarity | Lack of formal, documented delivery and payment obligations with customers | Partially | Financial loss, legal disputes, unclear responsibilities, security gaps | High 🔴 | Medium 🟡 | High | A.5.20, A.5.21, A.5.23 |
| 34 | Customer                | Rate              | User management by customer | Customer user management errors (need-to-know not enforced by customer) | Partially | Unauthorized access to information by customer users; Rate may be liable | High 🔴 | Medium 🟡 | High | A.8.2, A.8.3, A.5.20 |
| 35 | Rate                    | Customer          | Acceptable use by customer | Customer or end-user misuses Rate system | Partially | Reputational damage to Rate, possible legal action | High 🔴 | Medium 🟡 | High | A.5.20, A.5.21 |
| 36 | Rate                    | Hosting Provider  | Hosting availability/SLA | Hosting downtime or excessive data loss (MUD/MGV exceeded) | Mostly | Claims, reputational damage, customer loss | High 🔴 | Medium 🟡 | High | A.5.21, A.5.30, A.8.12 |
| 37 | Rate                    | VPN Provider      | VPN reliability | VPN connection unreliable or not auditable | Mostly | Claims, reputational damage, customer loss | High 🔴 | Medium 🟡 | High | A.8.20, A.5.21 |
| 38 | Rate                    | WiFi Provider     | WiFi security | Unauthorized admin access via WiFi | Mostly | Unauthorized access, data breach | High 🔴 | Medium 🟡 | High | A.8.20, A.8.1 |
| 39 | Rate                    | Trainers/Extra Services/Support/CRM Providers | Supplier data protection | Supplier mishandles customer or health data | Mostly | Claims, reputational damage, customer loss | High 🔴 | Medium 🟡 | High | A.5.19, A.5.20 |

---

### 2.7 Business Continuity & Emerging Risks

| # | Main Group (Stakeholder) | Requirement Owner | Issue/Requirement Addressed | Risk | How well is this being met? | Effect (consequence if not met) | Impact (Value of effect) | Likelihood | Risk Level | Annex A Reference (2022) |
|---|--------------------------|-------------------|-----------------------------|------|-----------------------------|----------------------------------|------------------------|------------|-----------|-------------------------|
| 40 | Rate                    | Rate              | Business continuity (pandemic) | Pandemic (e.g., Covid-19) disrupts business continuity | Mostly | Loss of income, operational disruption, need for team reorganization | High 🔴 | Medium 🟡 | High | A.5.30, A.17.1 |


# 3. Risk Treatment Plan

## 3.1 Data Security & Privacy Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 1 | Irresponsible handling or unauthorized access to customer/end-user data (availability, integrity, confidentiality) | Mitigate | Strict access control, encryption, regular audits, customer contract clauses, incident response plan | Developers, Managing Director | Access control, encryption, audit | Controls in place, regular audits, contract clauses reviewed annually | Yes | Low 🟢 | Low 🟢 | Acceptable if all controls are enforced and regularly audited. | Ongoing |
| 2 | Insider threats (employee mishandling data) | Mitigate | Implement role-based access control (RBAC) and log all sensitive actions. Refer to the Access Control Policy – Section 3 and Incident Plan – Section 6. | Managing Director | RBAC & logging | RBAC enforced; logs are reviewed, but not always timely. | Partially implemented – log review process improvement scheduled for Q3 2025 | Low 🟢 | Low 🟢 | Acceptable if RBAC is enforced & reviewed annually. | Q3 2025 |
| 3 | Mishandling of employee personal data (HR, payroll, contracts, ID) | Mitigate | Access to HR data restricted, encryption, regular audits, staff awareness training | Rate | Access control, encryption, audit | Controls in place, regular audits, training completed | Yes | Low 🟢 | Low 🟢 | Acceptable if controls are enforced and audited. | Ongoing |
| 4 | Mishandling of respondent data (including health info) | Mitigate | Data minimization, access control, encryption, retention policy, staff training | Rate | Data protection, retention, access control | Controls in place, training delivered, retention policy enforced | Yes | Low 🟢 | Low 🟢 | Acceptable if all controls and retention policy are enforced. | Ongoing |
| 5 | Data leakage via AI tools (e.g., ChatGPT) | Mitigate | Policy prohibits sharing sensitive data with AI tools, awareness training, monitoring | Rate | Acceptable use policy, training | Policy in place, training delivered, monitoring enabled | Yes | Low 🟢 | Low 🟢 | Acceptable if policy is enforced and staff trained. | Ongoing |

---

## 3.2 Platform, Infrastructure & Availability Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 6 | Platform/server failure or data loss (internal & customer impact) | Mitigate | High-availability hosting, uptime monitoring, backup and recovery, BCDR tested annually | Developers, Team Lead Developer | HA hosting, BCDR, monitoring | Uptime monitoring in place, BCDR plan tested annually | Yes | Low 🟢 | Low 🟢 | Acceptable if uptime >99.9% and BCDR is tested. | Ongoing |
| 7 | Losing access to head office systems | Mitigate | Ensure production server firewall rules can be modified securely without VPN access. Maintain alternative access methods. Refer to the Access Control Policy – Section 7 and BCDR Plan – Section 6.3. | Developers | Alternative access | Alternative access is available but not tested in the last 6 months. | Test scheduled for Q3 2025 | Medium 🟡 | Medium 🟡 | Acceptable if alternative means of accessing production servers exist. | Q3 2025 |
| 8 | NAS storage corruption or damage | Mitigate | Conduct a yearly backup integrity check. Refer to the BCDR Plan – Section 5.1 & 8 for test and retention validation procedures. | Team Lead Developer | Backup integrity | Yearly integrity checks are performed and documented. | Yes | Low 🟢 | Low 🟢 | Acceptable if yearly backups pass integrity checks. | Ongoing |
| 9 | Cloud provider (Hetzner) suffers a major outage or data loss | Transfer | Rely on Hetzner's SLA for uptime/data recovery; maintain regular backups and business interruption insurance. | Managing Director | Cloud SLA, insurance | SLA in place, insurance policy active, regular backup tests performed. | Yes | Medium 🟡 | Low 🟢 | Acceptable if SLA/insurance covers downtime and all backups pass annual tests. | Ongoing |
| 10 | Internet provider outage or degradation | Transfer | SLA with provider, backup 4G/5G hotspot for emergencies, regular provider review | Internet Provider | Provider SLA, backup connectivity | SLA in place, backup hotspot available, provider reviewed annually | Yes | Medium 🟡 | Low 🟢 | Acceptable if SLA and backup connectivity are maintained. | Ongoing |
| 11 | Telework infrastructure failure (VPN/device/connectivity) | Mitigate | Provide company laptops, enforce VPN, regular device maintenance, remote support | Rate | Device management, VPN | Laptops issued, VPN enforced, support available | Yes | Low 🟢 | Low 🟢 | Acceptable if all remote endpoints are managed and VPN is enforced. | Ongoing |
| 12 | Demo/training environment unavailable for trainers | Mitigate | Maintain dedicated demo environment, regular availability checks, fallback plan | Rate | Demo environment management | Demo system monitored, fallback procedures documented | Yes | Low 🟢 | Low 🟢 | Acceptable if demo environment is monitored and fallback exists. | Ongoing |
| 13 | Rate platform runs on unsupported/outdated Kentico version | Mitigate | Upgrade plan for Kentico, vulnerability management, regular patching, migration project scheduled | Developers | Patch management, upgrade plan | Upgrade project scheduled, vulnerability scans performed | In progress | Medium 🟡 | Medium 🟡 | Acceptable if migration is completed and platform is supported. | Ongoing |

---

## 3.3 Human Resource & Organizational Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 14 | Critical employee suddenly leaving | Mitigate | Document all key processes in the internal knowledge base, ensure secure password storage in LastPass, and implement role-based access restrictions as defined in the Access Control Policy. | Managing Director | Succession planning | Knowledge base is being updated; password management is fully implemented. | Knowledge base update completion due Q3 2025 | Low 🟢 | Low 🟢 | Acceptable if a knowledge base is maintained and access controls are enforced. | Q3 2025 |
| 15 | Sudden departure of CEO/MD | Mitigate | Store all critical credentials in a shared LastPass vault. Define succession roles and document recovery steps in the BCDRP. | CEO / Managing Director | Succession planning | Succession plan is documented and shared vault is in use; periodic review scheduled. | Yes | Low 🟢 | Low 🟢 | Acceptable if full access continuity is documented and roles are reassigned within 1 day. | Ongoing |
| 16 | High employee turnover leads to loss of knowledge and increased training costs | Mitigate | Maintain internal knowledge base, document key processes, automate onboarding/offboarding | Employees | Knowledge base, onboarding/offboarding | Knowledge base maintained, onboarding/offboarding automated | Yes | Low 🟢 | Low 🟢 | Acceptable if knowledge base is up to date and onboarding/offboarding are automated. | Ongoing |

---

## 3.4 Endpoint, Device & Remote Work Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 17 | Developer’s laptop lost/stolen/damaged | Accept (if all critical data is in the cloud and encrypted, and risk is low) | Enforce cloud-based storage with encryption (per Asset Management Policy) and use secure password managers as defined in the Access Control Policy. | Team Lead Developer | Device security | All critical data is in the cloud and encrypted; password managers rolled out to all staff. | Yes | Low 🟢 | Low 🟢 | Acceptable if all critical data is securely stored in the cloud. | Ongoing |
| 18 | Use of removable media (USB drives) for data transfer | Avoid | Policy prohibits use of removable media; all data transfer via secure, monitored cloud channels. | Team Lead Developer | Removable media ban | Policy enforced, technical controls block USB use on all endpoints. | Yes | Low 🟢 | Low 🟢 | Acceptable if removable media is technically blocked and policy is enforced. | Ongoing |
| 19 | Remote work leads to home network compromise | Accept | All endpoints are encrypted, VPN is mandatory, and security awareness is high. | Managing Director | Remote work controls | Endpoints encrypted, VPN enforced, awareness training completed. | Yes | Low 🟢 | Low 🟢 | Acceptable if all remote endpoints are encrypted and VPN is enforced. | Ongoing |
| 20 | Use of unmanaged/personal devices for company data (no AV, improper storage) | Mitigate | Policy prohibits use of unmanaged devices; endpoint protection and data storage policy enforced, compliance monitored | Managing Director | Endpoint protection, device policy | Policy enforced, compliance monitored | Yes | Low 🟢 | Low 🟢 | Acceptable if only managed devices are used and AV is enforced. | Ongoing |

---

## 3.5 Cybersecurity & Access Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 21 | Virus/ransomware attack on devices | Mitigate | Install enterprise-grade antivirus software, enable automatic updates, and conduct regular security training as outlined in the Access Control Policy. | Team Lead Developer | Endpoint protection | Antivirus is deployed and updated automatically; training is conducted annually. | Yes | Low 🟢 | Low 🟢 | Acceptable if endpoint protection is always enabled and updated. | Ongoing |
| 22 | Losing access to LastPass | Accept (if backup plan is tested and risk is low) | Maintain a bi-yearly backup of critical passwords in an encrypted and secure location, documented in the Access Control Policy. | CEO | Password backup | Backup process is documented and tested annually; last test successful. | Yes | Low 🟢 | Low 🟢 | Acceptable if backup plan is tested annually. | Ongoing |
| 23 | SSL certificate expiry | Avoid | Enable automatic SSL renewal or set up early expiration alerts as described in the Access Control Policy. | Team Lead Developer | SSL management | Automatic renewal is enabled on all domains; alerts are configured and monitored. | Yes | Low 🟢 | Low 🟢 | Acceptable if automatic renewal is active or renewal reminders are in place. | Ongoing |
| 24 | External attack (hacking, DDoS, etc.) disrupts business or leaks data | Mitigate | Firewall, DDoS protection, vulnerability management, incident response plan | Managing Director, Team Lead Developer | Network security, incident response | Controls in place, regular testing and patching | Yes | Low 🟢 | Low 🟢 | Acceptable if controls are maintained and tested. | Ongoing |
| 25 | Non-compliance with InfoSec policy/protocols | Mitigate | Mandatory annual training, policy sign-off, periodic awareness campaigns | Rate employees | Security awareness, policy sign-off | Training records maintained, sign-off required | Yes | Low 🟢 | Low 🟢 | Acceptable if all employees complete training and sign-off. | Ongoing |
| 26 | VPN connection unreliable or not auditable | Transfer | SLA with VPN provider for uptime and logging; periodic audit of VPN logs | VPN Provider | VPN SLA, logging | SLA in place, logs audited, provider reviewed annually | Yes | Medium 🟡 | Low 🟢 | Acceptable if SLA and logging/audit are enforced. | Ongoing |
| 27 | Unauthorized admin access via WiFi | Mitigate | WiFi provider contract requires MAC/IP filtering, strong authentication, regular review | WiFi Provider | WiFi security controls | MAC/IP filtering enforced, authentication policy in place | Yes | Low 🟢 | Low 🟢 | Acceptable if controls are enforced and reviewed. | Ongoing |
| 28 | Unable to enforce 2FA (ISO/NEN requirement) | Mitigate | 2FA implementation project planned, compensating controls in place, risk accepted short-term | Rate | 2FA project, compensating controls | Project scheduled, compensating controls documented | In progress | Medium 🟡 | Medium 🟡 | Acceptable if compensating controls are in place and 2FA is implemented by deadline. | Ongoing |

---

## 3.6 Supplier, Contractual & Third-Party Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 29 | Supplier/third-party mishandling of sensitive data (hosting, payroll, trainers, CRM, support, Mailstreet, etc.) | Transfer | DPAs and contracts require secure data handling, annual review, right to audit or terminate for breach (suppliers: hosting, payroll, trainers, CRM, support, Mailstreet, etc.) | Managing Director | DPA, contract, audit | DPA signed, audit rights in contract, annual review | Yes | Medium 🟡 | Low 🟢 | Acceptable if DPA and audit are enforced. | Ongoing |
| 30 | Physical intrusion (burglary) | Transfer | Lease/building contract requires landlord to maintain burglary prevention (locks, doors, alarm); office access policy enforced | Security company, landlord, staff | Physical security contract, access policy | Contract in place, access policy enforced, alarm tested | Yes | Medium 🟡 | Low 🟢 | Acceptable if contract and access policy are enforced and alarm is tested. | Ongoing |
| 31 | Fire prevention/detection failure | Transfer | Lease/building contract requires landlord to maintain fire detection and prevention (smoke detectors, extinguishers); BCDR plan includes fire scenario | Security company, landlord | Fire safety contract, BCDR plan | Contract in place, fire safety equipment maintained, BCDR plan tested | Yes | Medium 🟡 | Low 🟢 | Acceptable if contract and BCDR plan are in force and tested. | Ongoing |
| 32 | Insufficient NAS security for health information | Mitigate | NAS is physically secured in locked room, access restricted, strong authentication enforced, regular access reviews | Security company, landlord | Physical security, access control | NAS access logs reviewed, physical access restricted, authentication policy enforced | Yes | Low 🟢 | Low 🟢 | Acceptable if physical and logical access controls are enforced and reviewed. | Ongoing |
| 33 | Lack of formal, documented delivery and payment obligations with customers | Transfer | All customer contracts must include clear deliverables, payment terms, and security responsibilities; legal review required | Customer | Customer contract, legal review | Contract templates used, legal review required for all new agreements | Yes | Low 🟢 | Low 🟢 | Acceptable if all customer contracts are reviewed and signed. | Ongoing |
| 34 | Customer user management errors (need-to-know not enforced by customer) | Transfer | Customer contracts require proper user management; platform enforces RBAC and logs access; customer admin training | Customer | RBAC, contract clause | RBAC enforced, training provided, contract clause in place | Yes | Medium 🟡 | Low 🟢 | Acceptable if RBAC is enforced and customer contracts cover user management. | Ongoing |
| 35 | Customer or end-user misuses Rate system | Transfer | Terms of Service prohibit misuse; monitoring for abuse; contract allows for account suspension | Rate | ToS, abuse monitoring | ToS in place, monitoring enabled, process for suspension documented | Yes | Medium 🟡 | Low 🟢 | Acceptable if ToS and monitoring are enforced. | Ongoing |
| 36 | Hosting downtime or excessive data loss (MUD/MGV exceeded) | Transfer | SLA with hosting provider defines max downtime/data loss; regular review and failover tested | Hosting Provider | Hosting SLA, BCDR | SLA in place, failover tested, provider reviewed annually | Yes | Medium 🟡 | Low 🟢 | Acceptable if SLA is enforced and failover is tested. | Ongoing |
| 37 | VPN connection unreliable or not auditable | Transfer | SLA with VPN provider for uptime and logging; periodic audit of VPN logs | VPN Provider | VPN SLA, logging | SLA in place, logs audited, provider reviewed annually | Yes | Medium 🟡 | Low 🟢 | Acceptable if SLA and logging/audit are enforced. | Ongoing |
| 38 | Unauthorized admin access via WiFi | Mitigate | WiFi provider contract requires MAC/IP filtering, strong authentication, regular review | WiFi Provider | WiFi security controls | MAC/IP filtering enforced, authentication policy in place | Yes | Low 🟢 | Low 🟢 | Acceptable if controls are enforced and reviewed. | Ongoing |
| 39 | Supplier mishandles customer or health data | Transfer | DPA and contract require secure data handling, annual review, right to terminate for breach | Trainers/Extra Services/Support/CRM Providers | DPA, contract, audit | DPA signed, audit rights in contract, annual review | Yes | Medium 🟡 | Low 🟢 | Acceptable if DPA and audit are enforced. | Ongoing |

---

## 3.7 Business Continuity & Emerging Risks

| # | Risk | Treatment Option | Mitigation Actions (Taken measures) | Risk Owner | Control | Controlled? | Implemented? | Impact (residual) | Likelihood (residual) | Risk Acceptance Criteria | Status/Deadline |
|---|------|------------------|-------------------------------------|------------|---------|-------------|--------------|-------------------|-----------------------|------------------------|----------------|
| 40 | Pandemic (e.g., Covid-19) disrupts business continuity | Mitigate | Maintain and test BCDR plan, enable remote work, review pandemic scenarios annually | Rate | BCDR, remote work | BCDR plan includes pandemic, remote work enabled | Yes | Low 🟢 | Low 🟢 | Acceptable if BCDR is tested and remote work is functional. | Ongoing |


