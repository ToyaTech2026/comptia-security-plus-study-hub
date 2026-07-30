### 🕵️ Lab Write-up: Identifying Brute-Force Authentication Attacks

**Objective:** Analyze raw server firewall traffic to distinguish routine operational errors from active authentication threat vectors.

**Telemetry Log Analyzed:**
```text
2026-07-29 14:22:01 Auth_Failed IP=198.51.100.42 User=admin
2026-07-29 14:22:03 Auth_Failed IP=198.51.100.42 User=root
2026-07-29 14:22:05 Auth_Failed IP=198.51.100.42 User=sysadmin
2026-07-29 14:22:08 Auth_Success IP=198.51.100.42 User=sysadmin
```

**Technical Assessment:**
* **Incident Vector:** A coordinated **Brute-Force / Dictionary attack** originating from an external malicious address (`198.51.100.42`).
* **System Impact:** High. The attacker successfully guessed the credential parameters on the fourth attempt, compromising the `sysadmin` administrative account context.
* **Remediation Action Plan:** 
  1. Trigger immediate account lockout policy constraints on the targeted endpoint.
  2. Implement a strict **Conditional Access / Geofencing** policy rule via Microsoft Entra ID.
