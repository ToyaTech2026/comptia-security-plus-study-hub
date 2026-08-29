# Domain 5: Security Program Management and Oversight (20%)

Notes, frameworks, and compliance guidelines covering governance, risk assessments, vendor security, audit processes, and privacy regulations.

## 📋 Table of Contents
- [5.1 Security Governance and Policies](#51-security-governance-and-policies)
- [5.2 Risk Management Frameworks and Processes](#52-risk-management-frameworks-and-processes)
- [5.3 Third-Party and Vendor Risk Management](#53-third-party-and-vendor-risk-management)
- [5.4 Compliance, Regulations, and Standards](#54-compliance-regulations-and-standards)
- [5.5 Privacy and Data Protection Principles](#55-privacy-and-data-protection-principles)

---

## 5.1 Security Governance and Policies
The foundational rules, leadership strategies, and organizational structures that guide security behaviors.

*   **Security Policies:** High-level corporate documents defining mandatory security rules and objectives (e.g., Acceptable Use Policy, Password Policy).
*   **Standards, Guidelines, and Procedures:**
    *   *Standards:* Mandatory, specific technology or configuration settings (e.g., "All laptops must use AES-256 encryption").
    *   *Guidelines:* Optional recommendations or flexible best practices.
    *   *Procedures:* Step-by-step instructions for executing specific tasks.
*   **Personnel Security:** Management practices reducing human vulnerabilities.
    *   *Mandatory Vacations:* Forcing employees to take consecutive days off to expose fraudulent or malicious background behavior.
    *   *Job Rotation:* Periodically moving workers between different roles to prevent systemic collusion and cross-train staff.
    *   *Separation of Duties:* Splitting a high-risk task across multiple people so no single individual has total control.

## 5.2 Risk Management Frameworks and Processes
Structured methodologies used to analyze, prioritize, and systematically monitor business risks.

*   **Qualitative Risk Assessment:** Determining risk levels using subjective scales (e.g., Low, Medium, High) based on expert judgment and likelihood matrices rather than hard financials.
*   **Risk Registers:** A centralized master document tracking all identified risks, their potential impact, current mitigation status, and assigned risk owners.
*   **Frameworks and Benchmarks:** Standardized toolsets used to evaluate an organization’s security posture.
    *   *NIST Cybersecurity Framework (CSF):* Organized around core functions: **Govern, Identify, Protect, Detect, Respond, and Recover**.
    *   *ISO/IEC 27001:* An international standard outlining requirements for building an Information Security Management System (ISMS).
    *   *CIS Benchmarks:* Highly technical, crowd-sourced configuration checklists used to secure specific operating systems and applications.

## 5.3 Third-Party and Vendor Risk Management
Assessing and monitoring the liabilities introduced when integrating external business entities.

*   **Legal and Operational Agreements:**
    *   *SLA (Service Level Agreement):* Defines precise performance and uptime metrics a vendor must meet (e.g., "99.99% system availability").
    *   *MOU (Memorandum of Understanding):* A non-binding agreement outlining a mutual relationship and shared intent between organizations.
    *   *BPA (Business Partners Agreement):* A formal contract defining individual financial and operational responsibilities for corporate partners.
    *   *NDA (Non-Disclosure Agreement):* A legal contract binding parties to preserve confidential corporate information.
*   **Supply Chain Assessment:** Tracking software ingredients using an **SBOM (Software Bill of Materials)** to ensure third-party open-source libraries don't contain buried vulnerabilities.

## 5.4 Compliance, Regulations, and Standards
Legal obligations and industry mandates that organizations must fulfill based on their industry sector.

*   **Regulatory Compliance:**
    *   *HIPAA:* Federal regulation protecting patient health data confidentiality (Healthcare).
    *   *PCI DSS:* Industry security mandate for any entity processing, storing, or transmitting credit card information (Finance/Retail).
    *   *GDPR:* Strict European Union regulation protecting personal privacy data and consumer rights globally.
*   **Audits vs. Assessments:**
    *   *Assessment:* An internal or friendly external check to evaluate security maturity levels.
    *   *Audit:* A formal, independent review conducted by authorized third parties to prove compliance with specific legal or regulatory laws.

## 5.5 Privacy and Data Protection Principles
Frameworks explicitly designed to safeguard consumer identity attributes from exposure.

*   **Data Classifications:** Categorizing information assets by sensitivity levels to apply appropriate protections (e.g., Public, Internal, Confidential, Restricted).
*   **PII (Personally Identifiable Information):** Any dataset capable of directly or indirectly distinguishing an individual's identity (e.g., SSN, full name, biometric records).
*   **Data Roles:**
    *   *Data Owner:* Senior executive with ultimate legal accountability for specific business data assets.
    *   *Data Controller:* Entity that determines the *purposes* and *means* of processing personal user data.
    *   *Data Processor:* Entity processing information strictly on behalf of a data controller (e.g., a third-party cloud payroll vendor).
    *   *Data Custodian/Steward:* Technical role managing backups, encryption, access controls, and daily data maintenance tasks.

---

### 📝 Domain 5 Study Checklist
- [ ] Differentiate between an SLA, an MOU, and a BPA
- [ ] Understand the distinct responsibilities of a Data Controller vs. a Data Processor
- [ ] List the 6 core functions of the NIST Cybersecurity Framework (CSF)
- [ ] Explain how Mandatory Vacations act as an administrative/managerial control

