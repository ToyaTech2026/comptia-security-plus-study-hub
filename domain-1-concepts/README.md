# Domain 1: General Security Concepts (12%)

Notes, cheat sheets, and core definitions for the CompTIA Security+ SY0-701 Exam.

## 📋 Table of Contents
- [1.1 Core Security Imperatives (The CIA Triad)](#11-core-security-imperatives-the-cia-triad)
- [1.2 Safety and Non-Repudiation](#12-safety-and-non-repudiation)
- [1.3 Authentication, Authorization, and Accounting (AAA)](#13-authentication-authorization-and-accounting-aaa)
- [1.4 Security Control Categories and Types](#14-security-control-categories-and-types)
- [1.5 Fundamental Architecture Concepts](#15-fundamental-architecture-concepts)
- [1.6 Risk Management Terminology](#16-risk-management-terminology)
- [1.7 Quantitative Risk Calculations](#17-quantitative-risk-calculations)

---

## 1.1 Core Security Imperatives (The-CIA-Triad)
The fundamental pillars of information security.

*   **Confidentiality:** Prevents unauthorized disclosure of information.
    *   *Controls:* Encryption (AES), Access Control Lists (ACLs), Steganography, Obfuscation.
*   **Integrity:** Ensures data has not been altered, tampered with, or corrupted.
    *   *Controls:* Hashing (SHA-256, MD5), Digital Signatures, Configuration Management.
*   **Availability:** Ensures data and resources are accessible to authorized users when needed.
    *   *Controls:* Redundancy (RAID, clustering), Backups, UPS, Fault Tolerance, Patching.

## 1.2 Safety and Non-Repudiation
Extended core concepts beyond the CIA triad.

*   **Non-Repudiation:** Assures that the sender of data cannot deny sending it, and the recipient cannot deny receiving it.
    *   *Mechanisms:* Digital signatures, asymmetric encryption, immutable audit logs.
*   **Safety:** The physical protection of human life and well-being as the absolute highest priority in security operations.
    *   *Controls:* Fire suppression systems, escape routes, proper lighting, fencing.

## 1.3 Authentication, Authorization, and Accounting (AAA)
The framework for managing identities and access control.

*   **Authentication (Identification):** Verifying a user or system is who they claim to be.
    *   *Factors:*
        *   Something you **know** (Passwords, PINs, security questions).
        *   Something you **have** (Smart cards, hardware tokens, key fobs).
        *   Something you **are** (Biometrics: fingerprints, retina scans).
        *   Something you **do** (Handwriting dynamics, typing cadence).
        *   Somewhere you **are** (IP address, GPS geofencing).
*   **Authorization:** Granting specific permissions, rights, or privileges to authenticated identities.
    *   *Controls:* Role-Based Access Control (RBAC), Attribute-Based Access Control (ABAC).
*   **Accounting (Auditing):** Tracking and logging user actions, session metrics, and resource usage for compliance and forensics.

## 1.4 Security Control Categories and Types
Safeguards used to mitigate risk, classified by how they are implemented and their intent.

### Control Categories (How they are implemented)
*   **Technical (Logical):** Implemented via hardware, software, or firmware.
    *   *Examples:* Firewalls, Antivirus, IDSs, Encryption protocols.
*   **Managerial (Administrative):** Implemented via policies, procedures, and guidelines.
    *   *Examples:* Security policies, background checks, user training, risk assessments.
*   **Operational:** Implemented via human actions and physical security processes.
    *   *Examples:* Security guards, change management, incident response drills.
*   **Physical:** Tangible objects designed to protect an environment.
    *   *Examples:* Locks, fences, gates, barricades, biometric scanners on doors.

### Control Functions (Their specific intent)
*   **Preventive:** Stops an incident before it occurs (e.g., Firewalls, security training, locks).
*   **Detective:** Identifies and alerts to an incident during or after it occurs (e.g., Security logs, CCTV, IDS).
*   **Corrective:** Reverses the impact of an incident and restores normal state (e.g., Backups, system images, patching).
*   **Deterrent:** Discourages adversaries from attempting an attack (e.g., "Warning" signs, fake cameras).
*   **Compensating:** Alternative security controls put in place when primary controls are unavailable or too costly.

## 1.5 Fundamental Architecture Concepts
Architectural mindsets used to build robust secure perimeters.

*   **Defense in Depth (Layered Security):** Deploying multiple, distinct security layers so a single point of failure does not expose critical assets.
*   **Zero Trust Architecture (ZTA):** Eliminating implicit trust. Continually validates every transaction, user, and device.
    *   *Core Pillars:* Explicit verification, least privilege access, assume breach conditions.
*   **Least Privilege:** Restricting users and systems to only the absolute minimum permissions required to perform their daily duties.

## 1.6 Risk Management Terminology
The vocabulary of tracking and defining environmental liabilities.

*   **Threat:** Any potential circumstance or event that can negatively impact an asset.
*   **Vulnerability:** A flaw, bug, or weakness in a system or process that can be exploited by a threat.
*   **Risk:** The probability or likelihood that a threat will exploit a vulnerability. ($\text{Risk} = \text{Threat} \times \text{Vulnerability}$)
*   **Risk Strategies:**
    *   **Mitigation:** Reducing risk using security controls.
    *   **Transference:** Shifting risk to a third party (e.g., buying cybersecurity insurance).
    *   **Avoidance:** Eliminating the risk entirely by stopping the risky activity.
    *   **Acceptance:** Retaining the risk because the cost of fixing it outweighs the potential damage.

## 1.7 Quantitative Risk Calculations
Essential mathematical equations for cost-benefit security planning.

| Metric | Full Name | Definition / Formula |
| :--- | :--- | :--- |
| **AV** | Asset Value | The monetary worth of an asset. |
| **EF** | Exposure Factor | Percentage of asset value lost in a single incident. |
| **SLE** | Single Loss Expectancy | Cost of a single incident. Formula: $\text{AV} \times \text{EF}$ |
| **ARO** | Annualized Rate of Occurrence | Estimated number of times an incident happens per year. |
| **ALE** | Annualized Loss Expectancy | Estimated annual cost of a risk. Formula: $\text{SLE} \times \text{ARO}$ |

***

### 📝 My Study Checklist
- [ ] Memorize the 5 Authentication Factors
- [ ] Understand the difference between Technical, Managerial, and Operational controls
- [ ] Practice calculating SLE and ALE with sample word problems
- [ ] Explain Zero Trust principles in 2 sentences


