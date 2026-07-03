# Simulation Configuration Reference

**Document ID:** SIM-CONFIG-001  
**Project:** Elizabeth's Phishing Simulation for June 2026  
**Author:** Elizabeth Amoo  
**Date:** July 1, 2026

---

## Full Configuration Details

### Technique Selection
- **Framework:** MITRE ATT&CK
- **Technique:** Link to Malware
- **Technique ID:** T1566.002
- **Description:** Attacker hosts malicious file on trusted platform (SharePoint, Dropbox) and sends link via email. User opens link and executes malware.

---

### Simulation Identity
- **Name:** Elizabeth's Phishing Simulation for June 2026
- **Description:** Phishing Simulation for Malware
- **Type:** Social Engineering
- **Platform:** Email

---

### Payload Details
- **Payload Name:** DHL Parcel Tracker (LinkToMalwareFile)
- **Language:** English
- **Predicted Compromise Rate:** 18.08 percent
- **Lure Type:** Delivery notification impersonation
- **Why DHL:** High open rate due to user familiarity with parcel tracking emails

---

### Target Scope
- **Targeting Method:** Include only specific users and groups
- **Total Targeted:** 45 users or groups
- **Excluded Users:** 0
- **Rationale:** Scoped simulation allows controlled measurement without affecting entire organization

---

### Training Configuration
- **Training Content:** Microsoft training experience (Recommended)
- **Assignment Method:** Assign training for me (Recommended)
- **Trigger:** Automatic on user interaction with payload
- **Basis:** Microsoft assigns training based on user previous simulation history and learning pathways

---

### Landing Page
- **Type:** Global landing page
- **Template:** Microsoft Landing Page Template 1
- **Language:** English
- **Purpose:** Educate users immediately after they interact with the phishing payload
- **Payload Indicators:** Not enabled (not applicable to Link to Malware technique)

---

### End User Notifications
| Notification Type | Template | Purpose |
|------------------|----------|---------|
| Positive reinforcement | Microsoft default positive reinforcement notification | Reward users who did not click |
| Training assignment | Microsoft default training assignment notification | Notify users who clicked that training is assigned |
| Training reminder | Microsoft default training reminder notification | Remind users to complete assigned training |

---

### Launch Configuration
- **Launch Type:** Immediate
- **Launch Date:** July 1, 2026 at 3:30:36 PM
- **End Date:** July 3, 2026 at 3:30:36 PM
- **Duration:** 2 days
- **Region Aware Timezone Delivery:** Disabled
- **Payload Removal from Inboxes:** Not configured

---

### Review Summary
- **Delivery Platform:** Email
- **Technique:** Link to Malware
- **Payload:** DHL Parcel Tracker (LinkToMalwareFile)
- **Target Users:** 45 users or groups
- **Excluded Users:** 0
- **Status:** Simulation scheduled for launch — confirmed
