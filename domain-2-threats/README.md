
# Domain 2.0: Threats, Vulnerabilities, and Mitigations ☣️

## 1. Social Engineering Indicators
Attackers rely on human psychological triggers to bypass technical firewalls. I audit infrastructure for susceptibility to these common vectors:
*   **Phishing:** Mass email campaigns containing malicious attachments or deceptive credential-harvesting links.
*   **Spear Phishing:** Highly targeted malicious emails customized using intelligence gathered on a specific organization or individual.
*   **Whaling:** Spear phishing campaigns targeted explicitly at high-profile corporate leadership (CEOs, CFOs).

## 2. Application Layer Vulnerabilities
Modern application security extends past host OS patching. I specialize in identifying and mitigating software-level injection flaws:
*   **SQL Injection (SQLi):** Malicious SQL statements inserted into web form input fields to manipulate backend databases. *Mitigation: Input validation and parameterized queries.*
*   **Prompt Injection:** Adversarial text overrides designed to bypass content safety guardrails in Generative AI systems. *Mitigation: Hardened validation layers and string blocklists built in Python before data ingestion.*
