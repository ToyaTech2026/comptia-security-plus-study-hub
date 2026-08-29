# Domain 2: Threats, Vulnerabilities, and Mitigations (22%)

Notes and reference sheets on malicious actors, software vectors, vulnerabilities, and defense strategies.

## 📋 Table of Contents
- [2.1 Threat Actors and Motivations](#21-threat-actors-and-motivations)
- [2.2 Threat Vector and Attack Surface Concepts](#22-threat-vector-and-attack-surface-concepts)
- [2.3 Types of Vulnerabilities](#23-types-of-vulnerabilities)
- [2.4 Malicious Software (Malware) Types](#24-malicious-software-malware-types)
- [2.5 Social Engineering Attacks](#25-social-engineering-attacks)
- [2.6 Cryptographic Concepts](#26-cryptographic-concepts)

---

## 2.1 Threat Actors and Motivations
Understanding who is attacking and why they are doing it.

*   **Nation-State / APT (Advanced Persistent Threat):** Highly funded, organized, and sophisticated. Driven by espionage, political gain, or strategic disruption.
*   **Hacktivist:** Motivated by ideological, political, or social causes. Often use defacement or DDoS attacks.
*   **Insider Threat:** Current or former employees/contractors with legitimate system access. Driven by sabotage, financial gain, or carelessness.
*   **Cybercriminal / Organized Crime:** Heavily focused on direct financial gain. Primary users of ransomware and data theft rings.
*   **Shadow IT:** Employees deploying unauthorized software or hardware solutions without IT department approval.
*   **Competitors:** Driven by industrial espionage to steal intellectual property or market advantages.

## 2.2 Threat Vector and Attack Surface Concepts
How attackers find and exploit access paths.

*   **Threat Vector:** The path or means by which an attacker gains access to a system (e.g., Email, Wireless networks, Supply chain, Removable media).
*   **Attack Surface:** The sum total of all vulnerable points, entryways, and exposed code in an environment that an attacker could attempt to exploit.
    *   *Reduction Strategies:* Disabling unused ports, turning off unnecessary services, restricting firewalls.

## 2.3 Types of Vulnerabilities
Flaws and weaknesses categorized by origin.

*   **Zero-Day:** A newly discovered vulnerability that is actively exploited before the vendor has released a patch or workaround.
*   **Legacy Systems:** Old software or hardware architectures that are no longer supported or patched by vendors.
*   **Misconfigurations:** System flaws introduces by human error (e.g., Default credentials, unencrypted default protocols, open cloud storage buckets).
*   **Supply Chain Vulnerabilities:** Weaknesses introduced via third-party vendors, suppliers, or outsourced open-source dependencies.

## 2.4 Malicious Software (Malware) Types
Software engineered to cause damage, steal data, or compromise integrity.

*   **Ransomware:** Encrypts user data and demands a financial payout (usually in cryptocurrency) to provide the decryption key.
*   **Trojan:** Malicious code disguised or hidden inside seemingly legitimate, harmless software.
*   **Worm:** Self-replicating malware that spreads across computer networks automatically without human intervention.
*   **Virus:** Malicious code that attaches itself to an executable file and requires human action to execute and spread.
*   **Spyware / Keyloggers:** Background software designed to secretly record user activity, keystrokes, and credentials.
*   **Rootkit:** Deeply embedded malware designed to gain administrative-level (root) access while modifying system files to hide its presence from antivirus tools.
*   **Logic Bomb:** Dormant malicious code triggered only when specific conditions or dates are met (e.g., a specific employee account is deleted).

## 2.5 Social Engineering Attacks
Manipulating human psychology to trick individuals into breaking security protocols.

### Phishing Variations
*   **Phishing:** Generic mass-email blasts targeting random audiences to harvest credentials or infect systems.
*   **Spear Phishing:** Highly targeted, custom-tailored emails aimed at a specific individual or department using gathered intelligence.
*   **Whaling:** Spear phishing explicitly targeting high-value executives (CEOs, CFOs).
*   **Smishing:** Phishing conducted over SMS text messages.
*   **Vishing:** Phishing conducted via voice calls or automated phone systems.

### Physical & Psychological Tactics
*   **Tailgating:** Following an authorized person through a secure doorway without scanning a badge.
*   **Shoulder Surfing:** Physically looking over someone's shoulder to capture passwords, PINs, or sensitive data.
*   **Dumpster Diving:** Sifting through commercial trash bins to find discarded paperwork containing credentials or network maps.
*   **Social Engineering Principles:** Attackers exploit human nature using **Authority**, **Urgency**, **Intimidation**, **Scarcity**, or **Consensus/Social Proof**.

## 2.6 Cryptographic Concepts
The math and protocols used to protect data transit and confidentiality.

*   **Symmetric Encryption:** Uses a single, shared secret key to both encrypt and decrypt data. Fast, used for bulk data (e.g., AES, ChaCha20).
*   **Asymmetric Encryption:** Uses a mathematically linked key pair: a **Public Key** (anyone can see, used to encrypt) and a **Private Key** (kept secret, used to decrypt). Essential for key exchange and digital signatures (e.g., RSA, ECC).
*   **Hashing:** A one-way mathematical function that converts input data into a fixed-length string. Irreversible; used purely to verify integrity (e.g., SHA-2, SHA-3).
*   **Salting:** Adding random data to passwords before they are hashed to defeat precomputed rainbow table attacks.
*   **Cryptographic Obfuscation:** Making code or data intentionally confusing and difficult for humans/tools to reverse-engineer while remaining functional.

***

### 📝 Domain 2 Study Checklist
- [ ] Differentiate between a Worm, a Virus, and a Trojan
- [ ] Practice identifying social engineering principles (Urgency vs. Authority) in practice scenarios
- [ ] Understand the difference between symmetric and asymmetric key management
- [ ] Review common port numbers associated with secure vs. insecure threat vectors


