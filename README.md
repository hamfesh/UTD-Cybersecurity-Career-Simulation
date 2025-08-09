# Cybersecurity Career Simulation Projects

This repository showcases hands‑on security work with executive‑ready documentation.

---

## 1) Splunk Configuration File Hardening
**Overview:** Secured Splunk’s `config.conf` after detecting over‑permissive access and missing integrity checks; produced an executive report.
**Key Actions:**
- Located the correct config file and audited permissions.
- Hardened permissions (`chmod 700`, `chown root`).
- Established a baseline integrity hash with `md5sum` *(note: use SHA‑256 in production)*.
- Performed a controlled change and re‑verified the hash.
- Created a secure backup for rapid recovery.

**Skills:** Linux hardening, integrity monitoring, backups, executive reporting  
**Project File:** [📄 Splunk_Config_File_Hardening.pdf](./Splunk_Config_File_Hardening.pdf)

---

## 2) IT Onboarding Runbook (Windows Active Directory)
**Overview:** Standardized new‑hire workstation setup in a Windows AD domain.<br>
**Key Actions:**
- Domain join, AD user/group creation, departmental share with NTFS + share perms.
- OU creation; GPOs: startup banner, disable CMD, remove Run, logon drive map.
- Event Viewer verification and PowerShell checks.

**Skills:** AD admin, GPO, Windows permissions, PowerShell, procedural documentation  
**Project File:** [📄 IT-Onboarding-Runbook.pdf](./IT-Onboarding-Runbook.pdf)

---

## 3) Penetration Test – Career Simulation 3
**Overview:** Executed a full attack chain against a simulated corporate network; documented narrative, findings, and remediation.<br>
**Top Findings:**
- High: Command injection on web app (non‑standard port).
- High: SSH private key exposed on web server.
- High: Windows host vulnerable to SMB exploit; Pass‑the‑Hash viable.
- Medium: Weak password with outdated MD5 hashing.
- Medium: Insufficient segmentation enabled lateral movement.

**Remediation:** Input validation/WAF; remove keys from web root; patch/disable SMBv1; strong passwords + modern hashing (bcrypt/Argon2); MFA; VLAN segmentation + ACLs.  
**Skills:** Nmap, command injection, SSH pivot, John the Ripper, Metasploit (psexec), PTH, executive reporting  
**Project File:** [📄 Penetration_Test_Report_Career_Sim_3.pdf](./Penetration_Test_Report_Career_Sim_3.pdf)

---

## Repository Structure
```text
📦 cybserscuirty-career-simulation
├── Splunk_Config_File_Hardening.pdf
├── IT-Onboarding-Runbook.pdf
├── Penetration_Test_Report_Career_Sim_3.pdf
└── README.md
