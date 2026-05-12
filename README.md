<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>


# osTicket - Ticket Lifecycle: Intake Through Resolution
*This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.*

### Executive Summary
This project outlines the full lifecycle of a mission-critical support ticket within the **osTicket** platform. I simulated a high-pressure service scenario involving a total system outage for a banking client. This walkthrough demonstrates the technical workflow from **initial intake** to **executive communication**, **cross-departmental triage**, and **system restoration**.

___

### Environments and Technologies Used 
- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop Protocol** (RDP)
- **Internet Information Services** (IIS)
- **osTicket Ticketing System**

### Operating Systems Used 
- **Windows 10** (21H2)

### Ticket Lifecycle Stages 
1. **Intake**: User reporting and initial ticket creation.
2. **Observation & Triage**: Identifying urgency and establishing technical parameters.
3. **Communication & Resolution**: Technical troubleshooting and stakeholder management.
4. **Restoration**: Verification of service and ticket closure.

## Lifecycle Implementation Steps

**Step 1**: **Ticket Intake (End-User Perspective)**

The simulation begins with **Karen**, the head of a banking firm, reporting that her employees are unable to access the online banking portal. This is categorized as a "Report a Problem" topic with a summary stating the entire mobile/online system is down.

<img width="889" height="684" alt="image" src="https://github.com/user-attachments/assets/72c0ff37-ea2f-42b5-8815-2294610a30d0" />

---

**Step 2**: **Triage and Triage (SysAdmin Perspective)**

Logging in as **John (SysAdmin)**, I observed the ticket properties. Recognizing the severity, I manually escalated the ticket's priority to **Emergency** and set the **SLA Plan to Sev-A (1 hour, 24/7 response)**.

To ensure the right hands were on the issue, I reassigned the ticket from general Support to the **Online Banking Department** and assigned it specifically to **Agent Jane Doe**.

<img width="1223" height="769" alt="image" src="https://github.com/user-attachments/assets/3a76d01f-5cad-4828-81bf-de57712f5925" />

---

**Step 3**: **Resolution and Communication**

As **Jane Doe**, I addressed the outage by coordinating between the banking team and the vendor. After initiating a direct conversation with Karen to gather details and offer reassurance, the technical root cause was identified as a recent system update.

I coordinated a **rollback of the changes**, verified system functionality, and updated the ticket thread with a full post-mortem.


