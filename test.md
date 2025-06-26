| Risk | Likelihood | Impact | Risk Owner | Treatment Option | Mitigation Actions | Annex A Reference | Risk Acceptance Criteria | Financial Impact | Initial Risk Score | Control Effectiveness | Residual Risk Score | Risk Accepted | Management Approval |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Unauthorized access to customer database | Medium | High | Developers | Mitigate | Enforce strict access controls using a firewall and strong authentication mechanisms. | A.8.1 User authentication<br> A.8.2 Privileged access rights<br> A.8.3 Information access restriction | Acceptable if strong passwords are enforced and the firewall is active. | 500000 | <span style="color:#FFD700; font-weight:bold">6</span> | 4 | <span style="color:#90EE90; font-weight:bold">2</span> | No | Pending |
| Data loss from a server crash | Medium | High | Developers | Mitigate | Ensure automatic backups to NAS and perform regular backup tests. | A.8.12 Data backup | Acceptable if offsite backups are tested annually. | 300000 | <span style="color:#FFD700; font-weight:bold">6</span> | 5 | <span style="color:#90EE90; font-weight:bold">1</span> | Yes | Approved |
| Insider threats (employee mishandling data) | Low | High | Managing Director | Mitigate | Implement role-based access control (RBAC) and log all sensitive actions. | A.8.2 Privileged access rights<br> A.5.18 Access rights<br> A.8.15 Logging | Acceptable if RBAC is enforced & reviewed annually. | 400000 | <span style="color:#FFD700; font-weight:bold">4</span> | 3 | <span style="color:#90EE90; font-weight:bold">1</span> | No | Pending |
| Server crash causing service disruption | Medium | High | Developers | Mitigate | Implement regular database and code backups. Monitor server health and set automated alerts. | A.8.12 Data backup<br> A.8.16 Monitoring activities | Acceptable if regular backups are performed and automatic alerts are configured. | 350000 | <span style="color:#FFD700; font-weight:bold">6</span> | 4 | <span style="color:#90EE90; font-weight:bold">2</span> | No | Pending |
| Losing physical or internet access to head office (VPN, backups, development server) | Medium | High | Developers | Mitigate | Ensure production server firewall rules can be modified securely without VPN access. Maintain alternative access methods. | A.8.20 Networks security<br> A.7.4 Physical security monitoring | Acceptable if alternative means of accessing production servers exist. | 250000 | <span style="color:#FFD700; font-weight:bold">6</span> | 3 | <span style="color:#FFD700; font-weight:bold">3</span> | No | Pending |
| NAS Storage corruption or damage | Medium | High | Team Lead Developer | Mitigate | Conduct a yearly backup integrity check. | A.8.12 Data backup | Acceptable if yearly backups pass integrity checks. | 200000 | <span style="color:#FFD700; font-weight:bold">6</span> | 4 | <span style="color:#90EE90; font-weight:bold">2</span> | Yes | Approved |
| Critical employee suddenly leaving | Medium | Medium | Managing Director | Mitigate | Document all key processes in the internal knowledge base, ensure secure password storage in LastPass, and implement role-based access restrictions. | A.6.1 Responsibilities before, during, and after employment | Acceptable if a knowledge base is maintained and access controls are enforced. | 150000 | <span style="color:#FFD700; font-weight:bold">4</span> | 3 | <span style="color:#90EE90; font-weight:bold">1</span> | No | Pending |
| Developer’s laptop lost, stolen, or damaged | Medium | Medium | Team Lead Developer | Mitigate | Enforce cloud-based storage with encryption and use secure password managers. | A.5.10 Acceptable use of information and assets<br> A.8.10 Storage media | Acceptable if all critical data is securely stored in the cloud. | 100000 | <span style="color:#FFD700; font-weight:bold">4</span> | 4 | <span style="color:#90EE90; font-weight:bold">0</span> | Yes | Approved |
| Sudden departure of CEO or Managing Director | Low | High | CEO / Managing Director | Mitigate | Store all critical credentials in a shared LastPass vault. Define succession roles and document recovery steps. | A.6.1 Responsibilities before, during, and after employment<br> A.8.3 Information access restriction | Acceptable if full access continuity is documented and roles are reassigned within 1 day. | 300000 | <span style="color:#FFD700; font-weight:bold">4</span> | 3 | <span style="color:#90EE90; font-weight:bold">1</span> | No | Pending |
| Virus or ransomware attack on company devices | Medium | Medium | Team Lead Developer | Mitigate | Install enterprise-grade antivirus software, enable automatic updates, and conduct regular security training. | A.8.7 Protection against malware<br> A.6.3 Information security awareness, education, and training | Acceptable if endpoint protection is always enabled and updated. | 400000 | <span style="color:#FFD700; font-weight:bold">4</span> | 3 | <span style="color:#90EE90; font-weight:bold">1</span> | No | Pending |
| Losing access to LastPass (password manager) | Low | High | CEO | Mitigate | Maintain a bi-yearly backup of critical passwords in an encrypted and secure location. | A.8.1 User authentication<br> A.8.12 Data backup | Acceptable if backup plan is tested annually. | 200000 | <span style="color:#FFD700; font-weight:bold">4</span> | 4 | <span style="color:#90EE90; font-weight:bold">0</span> | Yes | Approved |
| SSL certificate expiry for platform or website | High | Medium | Team Lead Developer | Mitigate | Enable automatic SSL renewal or set up early expiration alerts. | A.8.24 Use of cryptography<br> A.8.23 Web filtering | Acceptable if automatic renewal is active or renewal reminders are in place. | 150000 | <span style="color:#FFD700; font-weight:bold">6</span> | 5 | <span style="color:#90EE90; font-weight:bold">1</span> | Yes | Approved |



<table>
  <tr>
    <th>Risk</th>
    <th>Likelihood</th>
    <th>Impact</th>
    <th>Risk Owner</th>
    <th>Treatment Option</th>
    <th>Mitigation Actions</th>
    <th>Annex A Reference</th>
    <th>Risk Acceptance Criteria</th>
    <th>Initial Risk Score</th>
    <th>Control Effectiveness</th>
    <th>Residual Risk Score</th>
    <th>Risk Accepted</th>
    <th>Management Approval</th>
  </tr>
  <tr>
    <td>Unauthorized access to customer database</td>
    <td>Medium</td>
    <td>High</td>
    <td>Developers</td>
    <td>Mitigate</td>
    <td>Enforce strict access controls using a firewall and strong authentication mechanisms.</td>
    <td>A.8.1, A.8.2, A.8.3</td>
    <td>Acceptable if strong passwords are enforced and the firewall is active.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">4</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">2</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Data loss from a server crash</td>
    <td>Medium</td>
    <td>High</td>
    <td>Developers</td>
    <td>Mitigate</td>
    <td>Ensure automatic backups to NAS and perform regular backup tests.</td>
    <td>A.8.12</td>
    <td>Acceptable if offsite backups are tested annually.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">5</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>Yes</td>
    <td>Approved</td>
  </tr>
  <tr>
    <td>Insider threats (employee mishandling data)</td>
    <td>Low</td>
    <td>High</td>
    <td>Managing Director</td>
    <td>Mitigate</td>
    <td>Implement role-based access control (RBAC) and log all sensitive actions.</td>
    <td>A.8.2, A.5.18, A.8.15</td>
    <td>Acceptable if RBAC is enforced & reviewed annually.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">3</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Server crash causing service disruption</td>
    <td>Medium</td>
    <td>High</td>
    <td>Developers</td>
    <td>Mitigate</td>
    <td>Implement regular database and code backups. Monitor server health and set automated alerts.</td>
    <td>A.8.12, A.8.16</td>
    <td>Acceptable if regular backups are performed and automatic alerts are configured.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">4</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">2</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Losing physical or internet access to head office (VPN, backups, development server)</td>
    <td>Medium</td>
    <td>High</td>
    <td>Developers</td>
    <td>Mitigate</td>
    <td>Ensure production server firewall rules can be modified securely without VPN access. Maintain alternative access methods.</td>
    <td>A.8.20, A.7.4</td>
    <td>Acceptable if alternative means of accessing production servers exist.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">3</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">3</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>NAS Storage corruption or damage</td>
    <td>Medium</td>
    <td>High</td>
    <td>Team Lead Developer</td>
    <td>Mitigate</td>
    <td>Conduct a yearly backup integrity check.</td>
    <td>A.8.12</td>
    <td>Acceptable if yearly backups pass integrity checks.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">4</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">2</td>
    <td>Yes</td>
    <td>Approved</td>
  </tr>
  <tr>
    <td>Critical employee suddenly leaving</td>
    <td>Medium</td>
    <td>Medium</td>
    <td>Managing Director</td>
    <td>Mitigate</td>
    <td>Document all key processes in the internal knowledge base, ensure secure password storage in LastPass, and implement role-based access restrictions.</td>
    <td>A.6.1</td>
    <td>Acceptable if a knowledge base is maintained and access controls are enforced.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">3</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Developer’s laptop lost, stolen, or damaged</td>
    <td>Medium</td>
    <td>Medium</td>
    <td>Team Lead Developer</td>
    <td>Mitigate</td>
    <td>Enforce cloud-based storage with encryption and use secure password managers.</td>
    <td>A.5.10, A.8.10</td>
    <td>Acceptable if all critical data is securely stored in the cloud.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">4</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">0</td>
    <td>Yes</td>
    <td>Approved</td>
  </tr>
  <tr>
    <td>Sudden departure of CEO or Managing Director</td>
    <td>Low</td>
    <td>High</td>
    <td>CEO / Managing Director</td>
    <td>Mitigate</td>
    <td>Store all critical credentials in a shared LastPass vault. Define succession roles and document recovery steps.</td>
    <td>A.6.1, A.8.3</td>
    <td>Acceptable if full access continuity is documented and roles are reassigned within 1 day.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">3</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Virus or ransomware attack on company devices</td>
    <td>Medium</td>
    <td>Medium</td>
    <td>Team Lead Developer</td>
    <td>Mitigate</td>
    <td>Install enterprise-grade antivirus software, enable automatic updates, and conduct regular security training.</td>
    <td>A.8.7, A.6.3</td>
    <td>Acceptable if endpoint protection is always enabled and updated.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">3</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>No</td>
    <td>Pending</td>
  </tr>
  <tr>
    <td>Losing access to LastPass (password manager)</td>
    <td>Low</td>
    <td>High</td>
    <td>CEO</td>
    <td>Mitigate</td>
    <td>Maintain a bi-yearly backup of critical passwords in an encrypted and secure location.</td>
    <td>A.8.1, A.8.12</td>
    <td>Acceptable if backup plan is tested annually.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">4</td>
    <td style="text-align:center;">4</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">0</td>
    <td>Yes</td>
    <td>Approved</td>
  </tr>
  <tr>
    <td>SSL certificate expiry for platform or website</td>
    <td>High</td>
    <td>Medium</td>
    <td>Team Lead Developer</td>
    <td>Mitigate</td>
    <td>Enable automatic SSL renewal or set up early expiration alerts.</td>
    <td>A.8.24, A.8.23</td>
    <td>Acceptable if automatic renewal is active or renewal reminders are in place.</td>
    <td style="background-color:#FFD700; font-weight:bold; text-align:center;">6</td>
    <td style="text-align:center;">5</td>
    <td style="background-color:#90EE90; font-weight:bold; text-align:center;">1</td>
    <td>Yes</td>
    <td>Approved</td>
  </tr>
</table>
