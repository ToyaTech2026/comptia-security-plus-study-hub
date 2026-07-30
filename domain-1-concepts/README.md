# Domain 1.0: General Security Concepts 🛡️

## 1. The CIA Triad Lifecycle
Every security policy I implement must enforce at least one pillar of the CIA Triad:
*   **Confidentiality:** Ensuring data is only viewable by authorized users. 
    *   *Implementation:* Enforced via AES-256 encryption at rest and TLS 1.3 in transit.
*   **Integrity:** Ensuring data has not been altered or corrupted.
    *   *Implementation:* Enforced using SHA-256 cryptographic hashing algorithms.
*   **Availability:** Ensuring systems are up and accessible to users when needed.
    *   *Implementation:* Enforced using load balancers, cloud redundancy, and high-availability VNets.

## 2. Zero Trust Architecture (ZTA) Core Tenets
Moving away from legacy perimeter security, I approach all cloud designs with a Zero Trust mindset:
1.  **Verify Explicitly:** Always authenticate and authorize based on all available data points (identity, location, device health).
2.  **Use Least Privilege Access:** Limit user access with Just-In-Time (JIT) and Just-Enough-Access (JEA) policies via Azure RBAC.
3.  **Assume Breach:** Minimize lateral movement by segmenting networks, encrypting end-to-end traffic, and monitoring system telemetry continuously.

