# Domain 3: Security Architecture (18%)

Notes, diagrams, and reference sheets covering network security, cloud infrastructures, secure application development, and physical security design.

## 📋 Table of Contents
- [3.1 Secure Network Architecture Concepts](#31-secure-network-architecture-concepts)
- [3.2 Secure Appliance and Component Deployment](#32-secure-appliance-and-component-deployment)
- [3.3 Cloud and Virtualization Architecture](#33-cloud-and-virtualization-architecture)
- [3.4 Secure Application Development and Deployment](#34-secure-application-development-and-deployment)
- [3.5 Resilience and High Availability Architecture](#35-resilience-and-high-availability-architecture)
- [3.6 Physical Security Controls](#36-physical-security-controls)

---

## 3.1 Secure Network Architecture Concepts
Designing corporate network perimeters to segregate traffic and block unauthorized access.

*   **Network Segmentation:** Splitting a network into smaller, isolated subnetworks to contain breaches and optimize traffic control.
    *   *Virtual Local Area Network (VLAN):* Logically separating devices on the same physical switch.
    *   *Demilitarized Zone (DMZ) / Screened Subnet:* A perimeter subnetwork containing public-facing services (Web, Mail, DNS) isolated from the internal network.
*   **Air Gapping:** A physical security measure ensuring a secure computer network is completely isolated from unsecured networks, such as the public internet.
*   **Software-Defined Networking (SDN):** Separating the network's control plane (routing decisions) from the data plane (packet forwarding) for centralized, programmable management.

## 3.2 Secure Appliance and Component Deployment
Proper placement and configuration of specialized hardware and software components.

*   **Firewalls:** Filters incoming and outgoing network traffic based on security rules.
    *   *Stateless:* Filters packets based on IP address and ports alone.
    *   *Stateful:* Tracks the context and state of active network connections.
    *   *Next-Generation Firewall (NGFW):* Adds deep-packet inspection, application-level context, and integrated IPS.
    *   *Web Application Firewall (WAF):* Explicitly inspects HTTP/HTTPS traffic to prevent web-based attacks (e.g., SQL Injection, XSS).
*   **IDS vs. IPS:**
    *   *Intrusion Detection System (IDS):* Monitors network traffic passively and alerts administrators to suspicious activity (**Detective**).
    *   *Intrusion Prevention System (IPS):* Sits inline with traffic and actively blocks malicious packets (**Preventive**).
*   **Proxies:** Acts as an intermediary between a client and a server.
    *   *Forward Proxy:* Protects and anonymizes internal clients accessing the internet.
    *   *Reverse Proxy:* Routes internet traffic to internal backend web servers, handling load balancing and SSL decryption.

## 3.3 Cloud and Virtualization Architecture
Security frameworks for hosted resources, multi-tenant boundaries, and managed infrastructure.

*   **Cloud Service Models:**
    *   *Infrastructure as a Service (IaaS):* Provider manages hardware; user manages OS, apps, and data (e.g., AWS EC2).
    *   *Platform as a Service (PaaS):* Provider manages hardware and OS; user manages apps and data (e.g., Heroku, AWS Elastic Beanstalk).
    *   *Software as a Service (SaaS):* Provider manages everything; user simply consumes the software over the web (e.g., Microsoft 365, Salesforce).
*   **Cloud Deployment Models:** Public, Private, Hybrid (combining public and private), and Community (shared between organizations with common goals).
*   **Virtualization Risks:**
    *   *VM Escape:* An attacker breaks out of a guest virtual machine to interact directly with the underlying hypervisor or host OS.
    *   *VM Sprawl:* The uncontrolled creation of virtual machines without proper lifecycle tracking, leading to unpatched, forgotten assets.

## 3.4 Secure Application Development and Deployment
Coding mindsets and testing phases used to limit software vulnerabilities.

*   **Development Life Cycle Models:** DevOps and DevSecOps (integrating automated security testing continuously directly into the CI/CD pipeline).
*   **Secure Coding Protections:**
    *   *Input Validation:* Verifying that user input conforms to strict specifications before processing it (crucial for blocking SQLi and XSS).
    *   *Output Encoding:* Sanitizing user data before rendering it back to a browser screen.
*   **Application Testing Environments:**
    *   *Development:* Where developers write code.
    *   *Test/QA:* Where code functionality is tested.
    *   *Staging:* A perfect mirror of production used to test deployment steps before going live.
    *   *Production:* The live system utilized by end-users.
*   **Analysis Methods:**
    *   *Static Application Security Testing (SAST):* Inspects source code for vulnerabilities without executing the program.
    *   *Dynamic Application Security Testing (DAST):* Evaluates a running application from the outside by simulating external attacks.

## 3.5 Resilience and High Availability Architecture
Systems designed to handle disasters, physical corruption, or high traffic spikes without going down.

*   **Redundancy Mechanisms:**
    *   *Load Balancing:* Distributing incoming traffic across multiple backend servers to prevent overload and ensure availability.
    *   *RAID (Redundant Array of Independent Disks):* Grouping multiple physical hard drives to protect data against drive failures.
*   **Site Resilience Options:**
    *   *Hot Site:** A fully operational, real-time mirrored facility. Can take over services within minutes of a disaster.
    *   *Warm Site:* Contains necessary hardware and network connections, but requires restoring backups and configuring apps before activation.
    *   *Cold Site:* An empty shell facility with power and HVAC. Requires days or weeks to move hardware in and configure from scratch.

## 3.6 Physical Security Controls
Tangible items protecting the physical facilities housing digital assets.

*   **Perimeter Defenses:** Fencing, barricades, bollards (concrete pillars blocking vehicles), and security lighting.
*   **Access Control:** Mantrap/Access Control Vestibule (double-door entry spaces designed to catch tailgaters), biometric turnstiles, and smart card badges.
*   **Monitoring & Suppression:** CCTV cameras, security guards, and specialized HVAC/Fire suppression systems (FM-200 or pre-action dry-pipe systems to avoid water damage to servers).

---

### 📝 Domain 3 Study Checklist
- [ ] Understand the difference between IaaS, PaaS, and SaaS
- [ ] Draw a mental diagram of traffic flowing into a corporate network via a Screened Subnet (DMZ)
- [ ] Memorize the exact functional differences between a WAF and a standard firewall
- [ ] Contrast SAST and DAST analysis approaches

