| Risk | Likelihood | Impact | Risk Owner | Treatment Option | Mitigation Actions | Annex A Reference (2022) | Risk Acceptance Criteria |
|---|---|---|---|---|---|---|---|
| Unauthorized access to customer database | Medium 🟡 | High 🔴 | Developers | Mitigate | Enforce strict access controls using a firewall and strong authentication mechanisms. Refer to the Access Control Policy – Sections 3 & 4. | A.8.1 User authentication <br> A.8.2 Privileged access rights <br> A.8.3 Information access restriction | Acceptable if strong passwords are enforced and the firewall is active. |
| Data loss from a server crash | Medium 🟡 | High 🔴 | Developers | Mitigate | Ensure automatic backups to NAS and perform regular backup tests. Refer to the Business Continuity and Disaster Recovery Plan – Section 5.1. | A.8.12 Data backup | Acceptable if offsite backups are tested annually. |
| Insider threats (employee mishandling data) | Low 🟢 | High 🔴 | Managing Director | Mitigate | Implement role-based access control (RBAC) and log all sensitive actions. Refer to the Access Control Policy – Section 3 and Incident Plan – Section 6. | A.8.2 Privileged access rights <br> A.5.18 Access rights <br> A.8.15 Logging | Acceptable if RBAC is enforced & reviewed annually. |



| Risk | Likelihood | Impact | Risk Owner | Treatment Option | Mitigation Actions | Annex A Reference (2022) | Risk Acceptance Criteria |
|---|---|---|---|---|---|---|---|
| Server crash causing service disruption | Medium 🟡 | High 🔴 | Developers | Mitigate | Implement regular database and code backups. Monitor server health and set automated alerts. Refer to the BCDR Plan – Section 5.1 & 6.1. | A.8.12 Data backup <br> A.8.16 Monitoring activities | Acceptable if regular backups are performed and automatic alerts are configured. |
| Losing physical or internet access to head office (VPN, backups, development server) | Medium 🟡 | High 🔴 | Developers | Mitigate | Ensure production server firewall rules can be modified securely without VPN access. Maintain alternative access methods. Refer to the Access Control Policy – Section 7 and BCDR Plan – Section 6.3. | A.8.20 Networks security <br> A.7.4 Physical security monitoring | Acceptable if alternative means of accessing production servers exist. |
| NAS Storage corruption or damage | Medium 🟡 | High 🔴 | Team Lead Developer | Mitigate | Conduct a yearly backup integrity check. Refer to the BCDR Plan – Section 5.1 & 8 for test and retention validation procedures. | A.8.12 Data backup | Acceptable if yearly backups pass integrity checks. |



| Risk | Likelihood | Impact | Risk Owner | Treatment Option | Mitigation Actions | Annex A Reference (2022) | Risk Acceptance Criteria |
|---|---|---|---|---|---|---|---|
| Critical employee suddenly leaving | Medium 🟡 | Medium 🟡 | Managing Director | Mitigate | Document all key processes in the internal knowledge base, ensure secure password storage in LastPass, and implement role-based access restrictions as defined in the Access Control Policy. | A.6.1 Responsibilities before, during, and after employment | Acceptable if a knowledge base is maintained and access controls are enforced. |
| Developer’s laptop lost, stolen, or damaged | Medium 🟡 | Medium 🟡 | Team Lead Developer | Mitigate | Enforce cloud-based storage with encryption (per Asset Management Policy) and use secure password managers as defined in the Access Control Policy. | A.5.10 Acceptable use of information and assets <br> A.8.10 Storage media | Acceptable if all critical data is securely stored in the cloud. |
| Sudden departure of CEO or Managing Director | Low 🟢 | High 🔴 | CEO / Managing Director | Mitigate | Store all critical credentials in a shared LastPass vault. Define succession roles and document recovery steps in the BCDRP. | A.6.1 Responsibilities before, during, and after employment <br> A.8.3 Information access restriction | Acceptable if full access continuity is documented and roles are reassigned within 1 day. |


| Risk | Likelihood | Impact | Risk Owner | Treatment Option | Mitigation Actions | Annex A Reference (2022) | Risk Acceptance Criteria |
|---|---|---|---|---|---|---|---|
| Virus or ransomware attack on company devices | Medium 🟡 | Medium 🟡 | Team Lead Developer | Mitigate | Install enterprise-grade antivirus software, enable automatic updates, and conduct regular security training as outlined in the Access Control Policy. | A.8.7 Protection against malware <br> A.6.3 Information security awareness, education, and training | Acceptable if endpoint protection is always enabled and updated. |
| Losing access to LastPass (password manager) | Low 🟢 | High 🔴 | CEO | Mitigate | Maintain a bi-yearly backup of critical passwords in an encrypted and secure location, documented in the Access Control Policy. | A.8.1 User authentication <br> A.8.12 Data backup | Acceptable if backup plan is tested annually. |
| SSL certificate expiry for platform or website | High 🔴 | Medium 🟡 | Team Lead Developer | Mitigate | Enable automatic SSL renewal or set up early expiration alerts as described in the Access Control Policy. | A.8.24 Use of cryptography <br> A.8.23 Web filtering | Acceptable if automatic renewal is active or renewal reminders are in place. |




