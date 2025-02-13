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

---

## 3. Access Control Principles
- **Least Privilege:** Limit access to the minimum necessary for tasks.
- **Need-to-Know:** Restrict sensitive data access.
- **Role-Based Access Control (RBAC):** Assign permissions based on job roles.
- **Separation of Duties:** Divide security-sensitive responsibilities.

---

## 4. User Access Management
### **4.1. Registration and De-registration**
- **Registration:** Requests are submitted to the Tech Lead via email and documented. CEO approval is required for high-privilege access.
- **De-registration:** The CEO instructs the Tech Lead to revoke access upon role change or departure.
- **Documentation:** All access requests are recorded in an internal log.

### **4.2. Provisioning and Review**
- The Tech Lead provisions access and conducts quarterly access reviews.
- Records are maintained for audit purposes.

---

## 5. Authentication and Password Management
- **2FA Implementation:**
  - **VPN:** 2FA with mobile OTP authenticator
  - **Cloud Apps (e.g., Google Workspace, GitHub):** SSO with 2FA
  - **Remote Desktop (RDP):** Enforced 2FA through VPN
- **Password Policy:** Minimum 12 characters, 90-day expiration, and secure storage in LastPass

---

## 6. Monitoring and Logging
- **Logs:** Collected from all on-premises and cloud systems.
- **Review Frequency:** The Tech Lead reviews logs quarterly.
- **Retention:** Logs are retained for at least one year.

---

## 7. Third-Party and Cloud Access Control
- Third-party access is not currently granted.
- Cloud administrators are the Tech Lead and Managing Director.
- Cloud provider security settings are configured to standard compliance.

---

## 8. Physical Access Control
- Building entry requires key card access.
- Office access is secured by key.
- NAS and Development Server are stored under lock.
- Production servers are cloud-hosted on Hetzner.

---

## 9. Responsibilities
- **Tech Lead:** Manages access, reviews logs quarterly, and oversees configurations.
- **CEO:** Approves sensitive access requests and enforces compliance.
- **Backup Administrator (in Tech Lead’s Absence):** Authorized to manage access and perform log reviews.
- **All Employees:** Maintain laptop security and promptly report incidents.

---

## 10. Policy Review
The policy undergoes annual review or immediate revision after major changes.

## 11. Compliance
Non-compliance may result in disciplinary actions or legal consequences.

---
*Note: Employees will be notified of all policy updates.*
