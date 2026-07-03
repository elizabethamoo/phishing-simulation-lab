# Phishing Simulation — Microsoft Defender Attack Simulation Training

**Project Type:** Security Awareness / Threat Simulation  
**Platform:** Microsoft Defender XDR — Attack Simulation Training  
**Author:** Elizabeth Amoo  
**Date:** July 1, 2026  
**Status:** Simulation Scheduled and Launched

---

## Project Overview

This project documents a phishing simulation campaign designed and executed using Microsoft Defender XDR Attack Simulation Training. The simulation tests organizational resilience against social engineering attacks by sending a realistic phishing email to targeted users and measuring how many users interact with the malicious payload.

This type of simulation is a core responsibility of a Security Operations Center (SOC) analyst and security awareness team. It aligns with industry frameworks including MITRE ATT&CK and NIST Cybersecurity Framework (Identify and Protect functions).

---

## Tools and Platforms Used

| Tool | Purpose |
|------|---------|
| Microsoft Defender XDR | Unified SIEM and XDR security platform |
| Attack Simulation Training | Phishing simulation campaign management |
| Microsoft Sentinel | Security information and event management |
| MITRE ATT&CK Framework | Attack technique classification |
| Microsoft Entra ID | User and group targeting |

---

## Simulation Configuration

| Field | Details |
|-------|---------|
| Simulation Name | Elizabeth's Phishing Simulation for June 2026 |
| Delivery Platform | Email |
| Attack Technique | Link to Malware (MITRE ATT&CK T1566) |
| Payload | DHL Parcel Tracker — LinkToMalwareFile |
| Predicted Compromise Rate | 18.08 percent |
| Target Users | 45 users and groups |
| Excluded Users | None |
| Launch Date | July 1, 2026 at 3:30 PM |
| End Date | July 3, 2026 at 3:30 PM |
| Duration | 2 days |
| Training Assignment | Microsoft recommended — auto-assigned on click |
| Landing Page | Microsoft Landing Page Template 1 |

---

## Attack Technique — MITRE ATT&CK T1566 Phishing

The simulation used the Link to Malware technique, which is classified under MITRE ATT&CK Technique T1566.002 — Phishing via Spearphishing Link.

**How this attack works:**

A malicious actor creates a legitimate-looking email notification — in this case impersonating DHL parcel delivery. The email contains a link that directs the user to a file hosted on a trusted file sharing platform such as SharePoint, Dropbox, or OneDrive. When the user clicks the link and opens the file, malware is executed on their device.

**Why DHL was chosen as the lure:**

DHL delivery notifications are one of the most widely used phishing lures in current threat campaigns because:
- Users regularly receive legitimate parcel notifications
- The email format is familiar and expected
- The urgency of package tracking prompts immediate action
- The 18.08 percent predicted compromise rate reflects real-world effectiveness

---

## Simulation Workflow

### Step 1 — Select Attack Technique
Reviewed MITRE ATT&CK-based technique options including Credential Harvest, Malware Attachment, Link in Attachment, and Link to Malware. Selected Link to Malware based on current threat landscape relevance.

### Step 2 — Name and Describe Simulation
Assigned a clear simulation name and description for audit trail documentation and reporting purposes.

### Step 3 — Select Payload
Reviewed global and tenant payloads. Selected DHL Parcel Tracker payload from the global payload library. Reviewed predicted compromise rate of 18.08 percent to set baseline expectations.

### Step 4 — Target Users
Selected 45 specific users from the organization. Used the Include only specific users and groups option rather than targeting all users, allowing for scoped measurement and controlled rollout.

### Step 5 — Exclude Users
Reviewed exclusion options. No users excluded from this simulation campaign.

### Step 6 — Assign Training
Selected Microsoft training experience (Recommended) with automatic training assignment. Users who interact with the phishing payload are automatically enrolled in security awareness training modules based on their previous simulation history and learning pathways.

### Step 7 — Configure Phish Landing Page
Selected Microsoft Landing Page Template 1 as the post-click education page. This page informs users they clicked a simulated phishing link and provides immediate security awareness guidance.

### Step 8 — Configure End User Notifications
Configured three notification types:
- Positive reinforcement notification for users who did not click
- Training assignment notification for users who did click
- Training reminder notification for incomplete training

### Step 9 — Set Launch Details
Configured simulation to launch immediately. Set 2-day duration ending July 3, 2026. Region-aware timezone delivery was not enabled for this simulation.

### Step 10 — Review and Submit
Reviewed all simulation settings including delivery platform, technique, payload, target users, and launch schedule. Submitted simulation for launch.

---

## Expected Outcomes and Metrics to Monitor

After the simulation ends on July 3, 2026, the following metrics will be available in the Reports tab:

| Metric | Description |
|--------|-------------|
| Compromise rate | Percentage of users who clicked the malicious link |
| Reporting rate | Percentage of users who reported the phishing email |
| Training completion rate | Percentage of compromised users who completed assigned training |
| Repeat clickers | Users who have clicked in previous simulations |
| Department breakdown | Compromise rate by department or group |

**Benchmark:** The predicted compromise rate of 18.08 percent means approximately 8 out of 45 targeted users are expected to click the payload. A successful security awareness program aims to reduce this rate by 50 percent or more over repeated simulation cycles.

---

## SOC Relevance and Skills Demonstrated

This project demonstrates the following SOC analyst skills:

- Understanding and applying the MITRE ATT&CK framework to real simulation scenarios
- Configuring and managing phishing simulation campaigns in Microsoft Defender XDR
- Targeting and scoping simulations to specific user groups
- Designing security awareness training workflows triggered by user behavior
- Measuring organizational phishing susceptibility using industry-standard metrics
- Documenting security operations activities following professional runbook standards

---

## Connection to Cybersecurity Frameworks

| Framework | Relevance |
|-----------|----------|
| MITRE ATT&CK | Technique T1566 — Phishing used as simulation basis |
| NIST CSF — Identify | Understanding organizational vulnerability to phishing |
| NIST CSF — Protect | Security awareness training and user education |
| NIST CSF — Detect | Measuring user reporting rates as detection capability |
| ISO 27001 — A.7.2.2 | Information security awareness, education and training |

---

## Platform Overview — Microsoft Defender XDR

Microsoft Defender XDR is the unified SIEM and XDR platform used by enterprise SOC teams worldwide. Key components visible in this project:

- **Microsoft Sentinel** — Cloud-native SIEM for log collection, threat detection, and incident response
- **Attack Simulation Training** — Security awareness simulation and measurement platform
- **Identities** — User and account monitoring via Microsoft Entra ID
- **Endpoints** — Device security monitoring and response
- **Email and Collaboration** — Email threat protection and simulation
- **Cloud Apps** — Cloud application security monitoring

---

## Files in This Project

```
phishing-simulation/
├── README.md                          (this file)
├── simulation-config.md               (detailed configuration reference)
├── mitre-attack-reference.md          (MITRE ATT&CK technique details)
└── screenshots/                       (simulation screenshots)
    ├── 01-defender-home.png
    ├── 02-simulation-dashboard.png
    ├── 03-select-technique.png
    ├── 04-payload-selection.png
    ├── 05-target-users.png
    ├── 06-assign-training.png
    ├── 07-landing-page.png
    ├── 08-notifications.png
    ├── 09-launch-details.png
    └── 10-simulation-launched.png
```

---

## Author

**Elizabeth Amoo** | Brampton, ON, Canada  
IT Support Specialist transitioning into Cybersecurity and SOC Analysis  
LinkedIn: linkedin.com/in/elizabethamoo  
Portfolio: github.com/elizabethamoo/helpdesk-home-lab
