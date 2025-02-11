## 4.1 Understanding the Organization and Its Context

Rate is a small software company specializing in providing a platform for collecting customer surveys and satisfaction metrics. Our primary operations involve:

- Developing and maintaining our survey platform.
- Managing customer accounts and their respective data.
- Ensuring the security and integrity of collected survey responses.

## 5.3 Organizational Roles, Responsibilities, and Authorities

The leadership of Rate assigns and communicates the necessary roles and responsibilities for the ISMS:

- **Chief Executive Officer (CEO):**
  - Holds overall accountability for the ISMS.
  - Ensures strategic alignment with business goals and information security requirements.
  - Responsible for high-level risk management.
  - Oversees overall compliance with regulatory and security standards.

- **Managing Director:**
  - Oversees ISMS implementation and its integration into business operations.
  - Ensures compliance with security policies and regulatory requirements.
  - Manages and maintains the ISMS framework and associated policies.
  - Conducts organization-wide risk assessments and ensures mitigation measures are in place.
  - Supports operational security measures and access control strategies.

- **Team Lead Developer:**
  - Leads the development team in implementing secure coding practices and ensuring software security.
  - Enforces security policies within the software development lifecycle.
  - Conducts periodic code reviews and security assessments to identify vulnerabilities.
  - Manages and monitors security compliance related to development infrastructure.
  - Acts as a point of contact for security incidents related to software and development infrastructure.

- **Developers:**
  - Follow secure coding standards and implement software security measures.
  - Assist in enforcing access control and authentication processes within the development environment.
  - Support security compliance by maintaining documentation and adhering to best practices.
  - Identify and report potential software vulnerabilities to the Team Lead Developer.
  - Assist in responding to security incidents by providing technical expertise and remediation support.


## 7.1 Resources

Rate.nl ensures the availability of adequate resources to support the implementation, maintenance, and improvement of its Information Security Management System (ISMS). The company utilizes the following resources:

- **Hosting & Cloud Security**: Rate.nl hosts its platform on **Hetzner (VMs)** and implements security measures such as:
  - Regular security updates and patch management.
  - Access controls to restrict unauthorized access.
  - Secure backups and monitoring for threat detection.

- **Password Management**: Rate.nl uses **LastPass** for securely storing and managing shared credentials.

- **Data & Document Security**:
  - **Google Drive**: Used for securely storing internal documents, policies, and ISMS-related information.
  - **Access Control**: Documents are restricted based on role-based permissions.

- **Security Tools**:
  - **Google Workspace**: Enforces security policies such as two-factor authentication (2FA), data encryption, and access control for emails, documents, and collaboration tools.
  - **Freshdesk**: Implements security controls to protect customer support interactions, including role-based access and secure ticket handling.
  - **Trello, Miro, Stack Overflow**: Used for project management and collaboration but do not store sensitive security-related data. Secure access policies are followed where applicable.

- **Physical & Network Security**:
  - **Access Cards**: Required for entering **Groothandelsgebouw** office space.
  - **Office Keys**: Provided to designated employees for securing physical workspace.
  - **Headsets**: Issued for employees working in remote or office environments.
  - **WiFi Networks**:
    - **Rate.nl Employee WiFi**: Secured with strong encryption and access control.
    - **Guest WiFi**: Separate network for visitors with restricted access.

- **IT Assets & Compliance**:
  - **Laptops**: Each employee is provided with a company-managed laptop with security controls.
  - **Exact Online**: Used for HR and compliance-related record-keeping.
  - **GitHub**: Source code management platform with enforced security policies.

- **Backup Strategy**:
  - **NAS Backup**: Full daily backups of the database from the **Hetzner production server** to an internal NAS system for disaster recovery.


## 8.4 System Maintenance and Monitoring

Rate.nl implements a structured approach for system maintenance and security monitoring:
- **Software Updates**:
  - System updates are configured to be **automatic** to ensure security patches are applied timely.
  - Employees are responsible for maintaining their assigned **company laptops** up to date.
- **Manual Vulnerability Assessment**:
  - **System & Software Configurations Review**: Regularly verify firewall rules, SSH access, and active services.
  - **Software & Patch Audits**: Check for outdated OS, CMS, and third-party libraries.
  - **Code Review**: Assess security risks such as hardcoded credentials, SQL injection risks, and weak authentication methods.
  - **Web Application Security Checks**: Validate authentication, session security, and input sanitization.
  - **Access Log Review**: Analyze failed login attempts and unusual activities.
  - All findings are documented, prioritized (Critical, High, Medium, Low), and remediated accordingly.
- **Log Monitoring**:
  - **Kentico CMS log monitoring** is used to track system activities and security-related events.

## 8.5 Third-Party Security Considerations

Rate.nl utilizes third-party services such as **Hetzner, Google Workspace, and Freshdesk**, where security is **guaranteed by the service providers** as part of their offerings. The company:
- Relies on third-party security controls as defined in their **terms of service and compliance documentation**.
- Regularly reviews security practices of critical providers to ensure continued compliance with industry standards.
- Ensures that internal security policies align with best practices when interacting with third-party services.
