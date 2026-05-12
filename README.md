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

---

### Permission and Escalation Testing

One of the most significant takeaways from this lab was observing how **Role-Based Access Control (RBAC)** affects ticket visibility and system security.

 I tested these boundaries by:

* **Restricted Routing**: Assigning tickets to the **SysAdmins** department and confirming they became inaccessible to general support agents.
* **Elevated Access**: Using the **Admin Panel** to grant specific "View Access" to an agent, allowing them to monitor a ticket's progress without the ability to modify it.
* **Cross-Departmental Collaboration**: Using **Teams** to allow agents from different departments to collaborate on the banking outage without changing their permanent departmental permissions.

---

### What This Project Demonstrates

This project highlights a comprehensive set of skills essential for Help Desk, Desktop Support, and Junior System Administration roles:

* **Ticket Triage & Prioritization**: Identifying business impact to set appropriate SLAs.
* **Department-Based Routing**: Ensuring tickets reach the correct subject matter experts.
* **Access Control & Permissions**: Troubleshooting visibility issues within the platform.
* **End-User Communication**: Managing stakeholder expectations during critical outages.
* **Ticket Lifecycle Management**: Documenting an issue from intake to a verified resolution.

---

### Real-World Help Desk Takeaways

A key lesson from this simulation is that in a production environment, tickets can originate from many sources—web portals, emails, phone calls, or even walk-ups. Regardless of how the request comes in, **documentation is mandatory**.

 Consistent documentation ensures:

1. **Accountability**: Every action taken is timestamped and attributed to an agent.
2. **Reporting & Metrics**: Management can track average resolution times to ensure SLA compliance.
3. **Knowledge Base Growth**: Resolved tickets can be used as references for similar future issues, reducing downtime across the organization.

---

### Why I Built This

I created this lifecycle simulation to bridge the gap between technical administration and the day-to-day operations of an enterprise IT team. Understanding the "flow" of a ticket is just as important as understanding the software itself, and this project serves as a proof of concept for my ability to manage both.
