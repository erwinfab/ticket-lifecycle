<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>


# osTicket - Ticket Lifecycle: Intake Through Resolution
*This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.*

### Executive Summary
This project outlines the full lifecycle of a mission-critical support ticket within the **osTicket** platform. I simulated a high-pressure service scenario involving a total system outage for a banking client. This walkthrough demonstrates the technical workflow from **initial intake** to **executive communication**, **cross-departmental triage**, and **system restoration**.

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

The simulation begins with **Karen**, the head of a banking firm, reporting that her employees are unable to access the online banking portal. This is categorized as a "General Inquiry/Other" topic with a summary stating the entire mobile/online system is down.

<img width="889" height="684" alt="image" src="https://github.com/user-attachments/assets/72c0ff37-ea2f-42b5-8815-2294610a30d0" />

---

**Step 2**: **Triage and Triage (SysAdmin Perspective)**

Logging in as **John (SysAdmin)**, I observed the ticket properties. Recognizing the severity, I manually escalated the ticket's priority to **Emergency** and set the **SLA Plan to Sev-A (1 hour, 24/7 response)**.

To ensure the right hands were on the issue, I reassigned the ticket from general Support to the **Online Banking Department** and assigned it specifically to **Agent Jane Doe**.

* Priority Level
<img width="894" height="768" alt="image" src="https://github.com/user-attachments/assets/e81b6a95-cf10-477e-bfb8-7bf4059bac80" />

<br/>

* SLA Plan

<img width="895" height="410" alt="image" src="https://github.com/user-attachments/assets/eb928628-b9e2-4e4d-af4b-5c680f926ecc" />

<br/>

* Issue was escalated to system administration/online banking department and assigned to Jane for completion.

 <img width="891" height="454" alt="image" src="https://github.com/user-attachments/assets/06ea614f-cd72-4a36-a206-d18438b789f0" />

---

**Step 3**: **Resolution and Communication**

As **Jane Doe**, I addressed the outage by coordinating between the banking team and the vendor. After initiating a direct conversation with Karen to gather details and offer reassurance, the technical root cause was identified as a recent system update.

I coordinated a **rollback of the changes**, verified system functionality, and updated the ticket thread with a full post-mortem.

* Reviewed the full ticket history as Jane.

<img width="813" height="703" alt="image" src="https://github.com/user-attachments/assets/1a745eb3-bc33-452b-86dd-5b1a3eb8968b" />

<br/>

* Responded as Jane.

<img width="798" height="632" alt="image" src="https://github.com/user-attachments/assets/28655e6d-0dde-4fca-b10a-7e413557341d" />

<br/>

<img width="809" height="257" alt="image" src="https://github.com/user-attachments/assets/4af40434-b7d3-41a6-b655-8e238c7a006d" />

<br/>

* Resolved issue and closed the ticket.

<img width="810" height="796" alt="image" src="https://github.com/user-attachments/assets/415dfde9-2fad-4f68-b8c1-63d37f5617aa" />

