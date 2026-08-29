# Domain 4: Security Operations (28%)

Notes, workflows, and reference sheets covering logging, continuous monitoring, baseline configurations, identity lifecycle, asset management, and incident response.

## 📋 Table of Contents
- [4.1 Logging and Monitoring Frameworks](#41-logging-and-monitoring-frameworks)
- [4.2 Identity and Access Management Operations](#42-identity-and-access-management-operations)
- [4.3 Configuration and Asset Management](#43-configuration-and-asset-management)
- [4.4 Vulnerability Management Processes](#44-vulnerability-management-processes)
- [4.5 Incident Response and Recovery Steps](#45-incident-response-and-recovery-steps)
- [4.6 Digital Forensics Basics](#46-digital-forensics-basics)

---

## 4.1 Logging and Monitoring Frameworks
Collecting and analyzing telemetry data across corporate environments to discover malicious indicators.

*   **SIEM (Security Information and Event Management):** Centralizes, aggregates, and correlates log data from firewalls, servers, and routers to provide real-time alerts.
*   **SOAR (Security Orchestration, Automation, and Response):** Takes SIEM insights a step further by automating incident response tasks using customized scripts called *playbooks*.
*   **Log Types to Monitor:**
    *   *System Logs:* Track OS events, service startups, and device drivers.
    *   *Security Logs:* Track login attempts, privilege adjustments, and policy changes.
    *   *Application Logs:* Track specific software errors, transaction logs, and database queries.
*   **Time Synchronization (NTP):** Using Network Time Protocol is vital so that timestamps match precisely across all systems during log correlation and tracking.

## 4.2 Identity and Access Management Operations
Managing the onboarding, maintenance, and deletion of user permissions securely.

*   **Identity Lifecycle:** Covering Provisioning (creating accounts), Maintenance (adjusting permissions when roles change), and Deprovisioning (immediately disabling accounts upon termination).
*   **Access Reviews:** Periodically auditing permissions to ensure users haven't accumulated unneeded privileges over time (*privilege creep*).
*   **Federated Identity:** Allowing a user to log in across different corporate domains using a single identity (e.g., using a corporate Google account to log into third-party SaaS apps via SAML or OIDC).

## 4.3 Configuration and Asset Management
Establishing baseline configurations and knowing every asset active on the corporate network.

*   **Configuration Baselines:** A secure operational standard that every server, workstation, or appliance must meet before deployment.
*   **Change Management:** A structured process (Submit $\rightarrow$ Review $\rightarrow$ Approve $\rightarrow$ Document) to evaluate potential security impacts before altering a production system.
*   **Asset Inventory:** Maintaining detailed lists of all physical hardware and digital software. Unmanaged, forgotten items become easy targets for attackers.

## 4.4 Vulnerability Management Processes
Proactively finding, prioritizing, and fixing software or process security weaknesses.

*   **Vulnerability Scanning:** Using automated tools (e.g., Nessus) to check systems for known unpatched flaws, open ports, and default configurations.
    *   *Credentialed Scans:* Scanner uses administrative credentials to log in and look deeply inside the OS for configurations and patch levels. Highly accurate.
    *   *Non-Credentialed Scans:* Scanner inspects the machine from the outside over the network. Simulates what an external hacker sees.
*   **Penetration Testing (Ethical Hacking):** Active, authorized simulation of an attack to breach defenses.
*   **Patch Management:** The systematic acquisition, testing, and installation of software updates to eliminate discovered vulnerabilities.

## 4.5 Incident Response and Recovery Steps
The systematic process structured to contain and recover from active security breaches.

### The Incident Response Lifecycle (NIST Framework)
1.  **Preparation:** Creating policies, establishing an incident response team (CIRT), and securing tools *before* a breach happens.
2.  **Detection and Analysis:** Monitoring indicators to determine if an event is an actual security incident.
3.  **Containment, Eradication, and Recovery:**
    *   *Containment:* Isolating infected machines from the network to stop the breach from spreading.
    *   *Eradication:* Removing malware, deleting bad accounts, and cleaning up systems.
    *   *Recovery:* Restoring systems to clean operational states using verified backups.
4.  **Post-Incident Activity (Lessons Learned):** Documenting what went wrong, analyzing the team's performance, and updating controls to prevent recurrence.

## 4.6 Digital Forensics Basics
Preserving and analyzing evidence after a security breach for internal review or legal action.

*   **Order of Volatility:** Collecting evidence from the fastest-disappearing state to the most permanent. Gather evidence in this exact order:
    1.  CPU Cache and Registers
    2.  Routing Tables, ARP Cache, Process Tables, Kernel Statistics
    3.  System Memory (RAM)
    4.  Temporary File Systems
    5.  Disk Storage (SSD, HDD)
    6.  Remote Logging and Monitoring Data
    7.  Physical Topology and Media (Archival backups, printouts)
*   **Chain of Custody:** A meticulous, unbroken document log tracking exactly who collected, handled, transferred, and stored a piece of physical or digital evidence.

---

### 📝 Domain 4 Study Checklist
- [ ] Memorize the strict order of volatility from most to least volatile
- [ ] Understand the differences between credentialed and non-credentialed vulnerability scans
- [ ] Explain the sequential steps of the NIST incident response lifecycle
- [ ] Contrast SIEM (collection/correlation) with SOAR (automation/response)

