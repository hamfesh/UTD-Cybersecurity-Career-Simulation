# Cybersecurity Career Simulation Projects
This repository contains completed projects from career simulation exercises, demonstrating both hands-on technical skills and professional documentation.

---

### 1. Splunk Configuration File Hardening
**Overview:**
A security hardening project for Splunk’s `config.conf` file, completed as part of a career simulation. The goal was to address excessive permissions, ensure integrity monitoring, and produce an executive-level report.

**Key Actions:**
- Located the correct `config.conf` file on the system.
- Identified insecure global file permissions.
- Applied least-privilege settings (`chmod 700`, `chown root`).
- Established a baseline file hash using `md5sum` (*note: in production, use stronger algorithms such as SHA-256*).
- Made authorized modifications and re-verified with a new hash.
- Created and stored secure backups in a designated directory.

**Skills Demonstrated:**
- Linux file system navigation and search (`find`, `cd`).
- Permission and ownership hardening.
- Integrity monitoring and baseline creation.
- Backup creation and storage.
- Executive-level cybersecurity reporting.

**Project File:** [📄 Splunk Config File Hardening Report](Splunk_Config_File_Hardening.pdf)

---

### 2. IT Onboarding Runbook (Windows Active Directory)
**Overview:**
A standardized runbook for onboarding new hires into a Windows Server Active Directory environment, ensuring consistent configuration, security, and usability.

**Key Actions:**
- Joined a workstation to an Active Directory domain.
- Created new user accounts and departmental groups.
- Configured a departmental shared folder with NTFS and share permissions.
- Created an Organizational Unit (OU) and linked targeted Group Policy Objects (GPOs).
- Implemented GPO restrictions (disable CMD, remove Run menu, add startup message).
- Reviewed security logs and ran PowerShell verification scripts.

**Skills Demonstrated:**
- Active Directory user, group, and OU management.
- Group Policy configuration and enforcement.
- Windows file sharing and permission setup.
- PowerShell scripting for system verification.
- Clear procedural IT documentation.

**Project File:** [📄 IT Onboarding Runbook](IT-Onboarding-Runbook.pdf)

---

### Repository Structure
```markdown
📦 UTD-Cybserscuirty-Career-Simulation
 ├── Splunk_Config_File_Hardening.pdf
 ├── IT-Onboarding-Runbook.pdf
 └── README.md
