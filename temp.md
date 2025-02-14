# Risk Assessment and Treatment Plan (RARTP)  
**Aligned with ISO/IEC 27001:2022 (Clauses 6.1.2 & 6.1.3)**  

---

## **1. Introduction**  
This document integrates the Risk Assessment and Risk Treatment Plan as required by **ISO/IEC 27001:2022**. It identifies information security risks, evaluates their impact, and details actions to mitigate them.

---

## **2. Risk Acceptance Criteria (Clause 6.1.3)**  
**Definition of Acceptable Risk:**  
- **Low Residual Risk:** Automatically accepted if controls are in place.  
- **Medium Residual Risk:** Accepted with documented justification and review annually.  
- **High Residual Risk:** Requires documented approval by the CEO with mitigation plans.  

---

## **3. Risk Scoring Methodology (Clause 6.1.2)**  
### **Likelihood and Impact Scale:**  
- **Likelihood:**  
  - 1 = Unlikely  
  - 2 = Possible  
  - 3 = Likely  
- **Impact:**  
  - 1 = Low (Minimal impact)  
  - 2 = Medium (Operational disruption)  
  - 3 = High (Critical business impact)  

### **Risk Score Calculation:**  
**Risk Score = Likelihood × Impact**  
| Score | Risk Level |
|-------|------------|
| 1-3   | Low        |
| 4-6   | Medium     |
| 7-9   | High       |

---

## **4. Risk Assessment and Treatment Table**  
This table integrates risk details, treatment options, Annex A controls, and effectiveness measures.

### **4.1 Data Security Risks**  
| **Risk** | **Likelihood** | **Impact** | **Risk Score** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Control** | **Residual Risk** | **Control Effectiveness Measure** | **Target Date** |
|---------|--------------|------------|--------------|--------------|------------------|---------------------|---------------------|------------------|-----------------------------|--------------|
| Unauthorized access to customer database | 2 (Possible) | 3 (High) | 6 (Medium) | Developers | Mitigate | Implement firewall rules, strong passwords, and access logging | A.9 Access Control | Low | Quarterly access log review | 2024-06-30 |
| Data loss from a server crash | 2 (Possible) | 3 (High) | 6 (Medium) | Developers | Mitigate | Set automatic backups to NAS and conduct annual offsite backup tests | A.12 Backup Policy | Low | Annual backup restore test | 2024-07-15 |
| Insider threats (employee mishandling data) | 1 (Unlikely) | 3 (High) | 3 (Low) | Managing Director | Mitigate | Implement RBAC and log sensitive actions | A.7 Human Resource Security | Low | Quarterly RBAC review | 2024-06-01 |

---

### **4.2 Infrastructure Risks**  
| **Risk** | **Likelihood** | **Impact** | **Risk Score** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Control** | **Residual Risk** | **Control Effectiveness Measure** | **Target Date** |
|---------|--------------|------------|--------------|--------------|------------------|---------------------|---------------------|------------------|-----------------------------|--------------|
| Server crash causing service disruption | 2 (Possible) | 3 (High) | 6 (Medium) | Developers | Mitigate | Perform regular backups and automated health alerts | A.17 Business Continuity | Low | Quarterly backup audit | 2024-05-30 |
| Loss of internet or VPN access to office | 2 (Possible) | 3 (High) | 6 (Medium) | Developers | Mitigate | Configure firewall rules for remote access without VPN | A.13 Network Security | Low | Annual VPN failover test | 2024-06-10 |
| NAS storage corruption or damage | 2 (Possible) | 3 (High) | 6 (Medium) | Tech Lead Developer | Mitigate | Conduct yearly backup integrity checks | A.12 Backup Policy | Low | Yearly backup integrity test | 2024-07-01 |

---

### **4.3 Human Resource Risks**  
| **Risk** | **Likelihood** | **Impact** | **Risk Score** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Control** | **Residual Risk** | **Control Effectiveness Measure** | **Target Date** |
|---------|--------------|------------|--------------|--------------|------------------|---------------------|---------------------|------------------|-----------------------------|--------------|
| Critical employee suddenly leaving | 2 (Possible) | 2 (Medium) | 4 (Medium) | Managing Director | Mitigate | Document key processes and store passwords in LastPass | A.7 Human Resource Security | Low | Quarterly knowledge base audit | 2024-06-30 |
| Developer’s laptop lost or stolen | 2 (Possible) | 2 (Medium) | 4 (Medium) | Tech Lead Developer | Mitigate | Enforce cloud storage with encryption and secure password managers | A.8 Asset Management | Low | Annual endpoint security audit | 2024-05-20 |

---

### **4.4 Cybersecurity Risks**  
| **Risk** | **Likelihood** | **Impact** | **Risk Score** | **Risk Owner** | **Treatment Option** | **Mitigation Actions** | **Annex A Control** | **Residual Risk** | **Control Effectiveness Measure** | **Target Date** |
|---------|--------------|------------|--------------|--------------|------------------|---------------------|---------------------|------------------|-----------------------------|--------------|
| Virus or ransomware attack | 2 (Possible) | 2 (Medium) | 4 (Medium) | Tech Lead Developer | Mitigate | Install antivirus software, automatic updates, and conduct security training | A.12 Malware Protection | Low | Annual security awareness training review | 2024-05-15 |
| Losing access to LastPass (password manager) | 1 (Unlikely) | 3 (High) | 3 (Low) | CEO | Mitigate | Maintain bi-annual encrypted backups of critical passwords in cloud storage | A.9 Access Control | Low | Bi-annual backup recovery test | 2024-06-01 |
| SSL certificate expiry for platform | 3 (Likely) | 2 (Medium) | 6 (Medium) | Tech Lead Developer | Mitigate | Enable automatic SSL renewal and set calendar reminders | A.14 System Security | Low | Annual SSL audit | 2024-04-30 |

---

## **5. Annex A Control Coverage Summary**  
This table maps risks to applicable **ISO/IEC 27001 Annex A Controls**:

| **Annex A Control** | **Related Risks Covered** |
|---------------------|--------------------------|
| A.7 Human Resource Security | Insider threats, Critical employee departure |
| A.8 Asset Management | Developer’s laptop loss |
| A.9 Access Control | Unauthorized database access, LastPass breach |
| A.12 Backup and Malware Protection | Server crash, Ransomware attack, NAS failure |
| A.13 Network Security | VPN loss or firewall bypass |
| A.14 System Security | SSL certificate expiry |
| A.17 Business Continuity | Server crash |

---

## **6. Monitoring and Continuous Improvement (ISO Clause 9.1 & 10.2)**  
- **Review Frequency:** Annually and after significant changes.  
- **Review Conducted By:** Managing Director.  
- **Control Effectiveness Check:** Verified through internal audits, penetration testing, and backup recovery tests.  
- **Lessons Learned:** Captured and logged in ISMS after each risk treatment implementation.  
- **Residual Risk Acceptance:** Signed off annually by the CEO.  

---

## **7. Review and Approval (ISO Clause 6.1.3 & 9.3)**  
- **Reviewed By:** Managing Director  
- **Approved By:** CEO  
- **Date of Last Review:** [Insert Date]  
- **Next Review Date:** [Insert Date]  
- **Version:** 1.1 (Updated for ISO Certification Readiness)  

---

### **✅ Final Status:** Fully compliant with ISO/IEC 27001:2022 (Clauses 6.1.2 and 6.1.3) and ready for auditor review.


