# MITRE ATT&CK Reference — Phishing Simulation

**Document ID:** MITRE-REF-001  
**Author:** Elizabeth Amoo  
**Date:** July 1, 2026

---

## What is MITRE ATT&CK?

MITRE ATT&CK (Adversarial Tactics, Techniques, and Common Knowledge) is a globally recognized framework that documents how real-world attackers behave. It is maintained by MITRE Corporation and is used by SOC analysts, threat hunters, and red teams worldwide to understand, detect, and respond to cyber attacks.

Every attack technique in the framework has a unique ID, description, and documented real-world usage by threat actors.

---

## Technique Used in This Simulation

### T1566 — Phishing
**Tactic:** Initial Access  
**Description:** Adversaries may send phishing messages to gain access to victim systems. Phishing is an attempt to trick targets into providing credentials or executing malicious code.

---

### T1566.002 — Phishing: Spearphishing Link
**Technique ID:** T1566.002  
**Tactic:** Initial Access  
**Platform:** Linux, macOS, Windows, Office 365, SaaS  

**How it works:**  
The attacker sends a targeted email containing a malicious link. In this simulation the link directs users to a file hosted on a trusted file sharing platform. When the user opens the file, malicious code is executed.

**Why it is effective:**  
- Uses trusted platforms (SharePoint, Dropbox, OneDrive) to bypass email filters
- Leverages familiar sender impersonation (DHL in this case)
- Creates urgency that reduces critical thinking (parcel delivery notification)
- 18.08 percent predicted compromise rate reflects real-world effectiveness

---

## Other Techniques Available in Microsoft Defender Simulation

| Technique | MITRE ID | Description |
|-----------|----------|-------------|
| Credential Harvest | T1566.002 | Fake login page captures username and password |
| Malware Attachment | T1566.001 | Malicious file attached directly to email |
| Link in Attachment | T1566.001 + T1566.002 | Link embedded inside an attached document |
| Link to Malware | T1566.002 | Link to malware file hosted on trusted platform |

---

## MITRE ATT&CK Tactics Relevant to SOC Analysis

Understanding where phishing fits in the full attack lifecycle is essential for SOC analysts:

| Stage | Tactic | What Happens |
|-------|--------|-------------|
| 1 | Reconnaissance | Attacker researches the target organization and employees |
| 2 | Resource Development | Attacker creates fake emails, domains, and payloads |
| 3 | Initial Access | Phishing email is sent — this is where T1566 occurs |
| 4 | Execution | User clicks link and malware runs on their device |
| 5 | Persistence | Attacker establishes foothold to maintain access |
| 6 | Privilege Escalation | Attacker gains higher level access |
| 7 | Defense Evasion | Attacker hides activity from security tools |
| 8 | Credential Access | Attacker steals passwords and account credentials |
| 9 | Lateral Movement | Attacker moves to other systems in the network |
| 10 | Exfiltration | Attacker steals and removes sensitive data |

A Tier 1 SOC analyst focuses primarily on detecting stages 3 through 6 before the attacker progresses further.

---

## How SOC Analysts Use MITRE ATT&CK

- Map incoming alerts to specific MITRE techniques to understand what the attacker is doing
- Use the framework to write detection rules in SIEM tools like Microsoft Sentinel
- Reference technique IDs in incident reports for standardized communication
- Identify gaps in detection coverage by checking which techniques have no alerts configured
- Use threat intelligence to prioritize which techniques are most actively used by current threat actors

---

## Resources

- MITRE ATT&CK Official Framework: attack.mitre.org
- T1566 Phishing full details: attack.mitre.org/techniques/T1566
- Microsoft Defender Attack Simulation Training docs: learn.microsoft.com/en-us/defender-office-365/attack-simulation-training
