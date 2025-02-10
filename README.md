**Introduction**

At Rate, we are committed to safeguarding the confidentiality, integrity, and availability of all physical and electronic information assets throughout our organization. This Information Security Management System (ISMS) manual outlines the policies, procedures, and controls implemented to manage information security risks effectively. Our goal is to ensure business continuity, minimize business risk, and maximize return on investments and business opportunities.

This manual is structured to provide a comprehensive overview of our ISMS, detailing the scope, objectives, risk assessment methodologies, and the various controls in place to protect our information assets. It serves as a reference point for all stakeholders to understand our approach to information security and their roles within it.

The following sections will guide you through the specific components of our ISMS.


# Information Security Management System (ISMS) Documentation for Rate

1. **Context of the Organization** (Clause 4)
2. **Leadership** (Clause 5)
3. **Planning** (Clause 6)
4. **Support** (Clause 7)
5. **Operation** (Clause 8)
6. **Performance Evaluation** (Clause 9)
7. **Improvement** (Clause 10)



# 1. Context of the Organization (Clause 4)

## 4.1 Understanding the Organization and Its Context

Rate is a small software company specializing in providing a platform for collecting customer surveys and satisfaction metrics. Our primary operations involve:

- Developing and maintaining our survey platform.
- Managing customer accounts and their respective data.
- Ensuring the security and integrity of collected survey responses.

We recognize that information security is vital to maintaining customer trust and meeting regulatory requirements. Therefore, we are committed to implementing an Information Security Management System (ISMS) that aligns with our organizational context and addresses relevant internal and external issues.

## 4.2 Understanding the Needs and Expectations of Interested Parties 

To ensure the effectiveness of our ISMS, we have identified the following interested parties and their expectations:

- **Customers**: Expect confidentiality and integrity of their survey data.
- **Employees**: Seek a secure working environment and protection of personal information.
- **Regulatory Bodies**: Require compliance with applicable data protection laws and regulations.
- **Suppliers and Partners**: Anticipate secure handling of shared information and adherence to contractual obligations.

## 4.3 Determining the Scope of the ISMS 

The scope of our ISMS encompasses all processes, systems, and personnel involved in the development, maintenance, and delivery of our survey platform services. This includes:

- **Physical Location**: Our single office premises.
- **Assets**: Servers, databases, backups, company laptops, and network infrastructure.
- **Information**: Customer survey data and employee personal information.
- **Activities**: Data collection, processing, storage, and analysis related to customer surveys.

## 4.4 Information Security Management System 

Rate has established, implemented, and is committed to maintaining and continually improving an ISMS in accordance with the ISO/IEC 27001:2022 standard. Our ISMS framework is designed to manage and mitigate risks to our information assets, ensuring their confidentiality, integrity, and availability. This system includes policies, procedures, and controls tailored to our organizational context and the needs of our interested parties.


# 2. Leadership (Clause 5)

## 5.1 Leadership and Commitment

The leadership of **Rate** demonstrates its commitment to establishing, implementing, maintaining, and continually improving the Information Security Management System (ISMS) in accordance with ISO/IEC 27001:2022. The leadership ensures:

- The ISMS aligns with the strategic direction and business objectives of Rate.
- Information security requirements are integrated into the company's processes.
- Adequate resources are available to implement and maintain the ISMS.
- Responsibilities and authorities for information security are assigned and communicated within the organization.
- A culture of continuous improvement in information security is promoted.

## 5.2 Information Security Policy

Rate has established an Information Security Policy that:
- Is appropriate to the organization’s purpose and context.
- Provides a framework for setting information security objectives.
- Includes commitments to fulfilling applicable requirements and continuous improvement.
- Is communicated within the organization and available to relevant interested parties.

The policy is reviewed periodically to ensure its effectiveness and relevance.

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

All employees are responsible for following the information security policies and reporting security incidents or weaknesses.

The leadership of Rate ensures that roles and responsibilities are well understood and that employees have the necessary competencies and resources to fulfill their information security obligations.

# Clause 6: Planning

## 6.1 Actions to Address Risks and Opportunities

Rate.nl has established a **risk management framework** to identify, assess, and mitigate information security risks. This ensures continuous improvement of security measures and alignment with business objectives.

### Risk Management Framework
1. **Identify Risks** – Regularly assess threats related to data confidentiality, availability, and integrity.
2. **Assess Risks** – Categorize risks based on likelihood and impact.
3. **Mitigate Risks** – Implement security controls to address identified risks.
4. **Monitor and Review** – Conduct periodic risk assessments to ensure ongoing security compliance.

## 6.2 Information Security Objectives and Planning to Achieve Them

Rate.nl has defined the following **security objectives**:
- **Ensure system availability** – Maintain high uptime and prevent service disruptions.
- **Protect data confidentiality** – Safeguard sensitive customer and business data.
- **Ensure GDPR compliance** – Implement and enforce data protection measures.
- **Improve security awareness** – Conduct employee training and awareness sessions.

### Implementation Plan
- **Assign Responsibilities** – Ensure that roles and responsibilities for security measures are clearly defined.
- **Set Measurable Goals** – Define key performance indicators (KPIs) to track progress.
- **Review Performance** – Conduct internal audits and assessments.
- **Continuous Improvement** – Update security policies and controls as needed.

## 6.3 Planning of Changes

Rate.nl has established a structured process to manage security-related changes efficiently:
- **Change Evaluation** – Assess security impact before implementing changes.
- **Approval Process** – Ensure management reviews and approves critical changes.
- **Implementation and Monitoring** – Deploy changes securely and track their effectiveness.
- **Documentation and Compliance** – Maintain records to ensure ongoing GDPR compliance and alignment with security objectives.

# Clause 7: Support

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

## 7.2 Competence

To ensure security effectiveness, Rate.nl has implemented a **basic competency evaluation framework**, including:
- **Role-based security knowledge**: Employees are trained on security responsibilities relevant to their roles.
- **Periodic assessments**: Regular internal evaluations will be conducted to measure employee understanding of security policies.
- **Annual security reviews**: Formal reviews are conducted to verify employees' comprehension and adherence to security policies.
- **Continuous learning**: Employees are encouraged to stay updated on security trends through external resources and internal training.

## 7.3 Awareness

Rate.nl has established a **security training plan** to ensure all employees are aware of information security policies and their responsibilities:
- **Onboarding Training**: New employees receive a basic introduction to the ISMS and security policies.
- **Ongoing Awareness Campaigns**: Periodic security reminders and training sessions are conducted.
- **Phishing and Social Engineering Awareness**: Employees are educated on recognizing and reporting suspicious activities.

## 7.4 Communication

Effective communication is essential to maintain information security. Rate.nl follows these communication practices:
- **Internal Communication**: Security updates, policies, and incident reports are shared with employees through email and internal meetings.
- **External Communication**: Security-related discussions with clients, partners, and authorities follow defined policies to ensure confidentiality and compliance.
- **Incident Reporting**: Employees report security incidents promptly to the designated authority within the organization.

## 7.5 Documented Information

Rate.nl ensures proper management of security-related documentation, including:
- **Security Policies and Procedures**: Maintained and updated periodically to reflect security changes.
- **Access Logs and Incident Reports**: Documented for tracking security activities and improvements.


# Clause 8: Operation

## 8.1 Operational Planning and Control

Rate.nl ensures that information security processes are planned, implemented, and controlled in alignment with ISO 27001:2022. The company follows structured approaches for managing security operations, including:
- Ensuring compliance with documented security policies.
- Monitoring security risks and addressing vulnerabilities.
- Maintaining operational procedures for security-related tasks.

## 8.2 Change Management

Rate.nl maintains a **Change Management Log** stored in **Google Drive** to document and track system changes. The change management process includes:
- **Recording all significant changes** affecting security or system performance.
- **Reviewing and approving changes** before implementation.
- **Testing changes** to ensure no adverse impact on security or functionality.
- **Monitoring changes post-implementation** to address unforeseen risks.

## 8.3 Incident Management

Rate.nl follows a **structured incident response process** to detect, report, and mitigate security incidents efficiently. The process includes:
1. **Detection & Reporting** – Employees must report suspected security incidents immediately.
2. **Assessment & Classification** – Incidents are classified based on severity and potential impact.
3. **Response & Containment** – Affected systems or accounts may be isolated to prevent further damage.
4. **Investigation & Remediation** – Root causes are identified, and corrective actions are applied.
5. **Documentation & Review** – Each incident is logged, and lessons learned are used to improve security controls.

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


