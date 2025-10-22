<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<h3>Initial Setup (Admin)</h3>
  
Before simulating the lifecycle, we perform a one-time admin setup. After logging into the Admin Panel (/scp) , we navigate to Departments to change SysAdmins into a Top-Level Department and then DELETE the Maintenance Department.


<p>
<img width="511" height="564" alt="image" src="https://github.com/user-attachments/assets/cf082e1c-d9d7-47d0-9ed1-3657a0b8e6f9" />

</p>
<p>
<h2>Step 1: Ticket Intake (End-User)</h2>
  
This phase begins from the end-user portal (http://localhost/osTicket), where we submit three distinct tickets to simulate user issues:

- "entire mobile/online banking system is down" 

- "accounting department needs adobe upgrade, broken" 

- "CFO's laptop will no longer turn on" 


(Note for discussion: In a real-world environment, intake also occurs via phone, email, or in-person walk-ups. Best practice is to create a ticket for every task to ensure all work is tracked for metrics.)
</p>
<br />
<img width="508" height="361" alt="image" src="https://github.com/user-attachments/assets/80bfc1c6-82b3-4e72-88b5-b447a3301e66" />

<h2>Step 2: Triage and Assignment (Help Desk Agent)</h2>

This phase is handled by Agent "john" logging into the agent portal (/scp). "John" triages each new ticket:


1. Banking Ticket: He observes the ticket's defaults and then sets its properties to Sev-A Priority (1 hour, 24/7) and assigns it to the Online Banking Department.




2. Adobe Ticket: He observes its defaults and sets the properties to Sev-B Priority (4 hours, 24/7)  and the Support Department.



3. CFO Laptop Ticket: He observes its defaults and also sets it to Sev-B Priority  and the Support Department.
</p>
<br />
<img width="588" height="544" alt="image" src="https://github.com/user-attachments/assets/c881350e-80b8-4c2f-8290-6a43f1d3f24f" />

<h2>Step 3: Work, Escalation, and Resolution (Agent & Admin)</h2>

In this final phase, the agents work the tickets and we test the system's permission-based routing.


1. Work: Agent "john" attempts to view the "banking down" ticket but finds he cannot access it , as it was reassigned to a department he is not in. Agent "jane" must log in to work and resolve that specific ticket. "John" proceeds to work and resolve both the Adobe and CFO laptop tickets.




2. Escalation: To test permissions, we set all remaining tickets to the Sev-A (SysAdmins) department. This makes them immediately inaccessible to our agent.


3. Resolution: We switch to the Admin Panel to grant Agent "john" "View-access" to the Sys Admins department. Back in the agent portal, "john" can now see the escalated tickets but cannot make changes, demonstrating a successful permissions test. Finally, an agent with the proper permissions (like an Admin) logs in to solve all remaining tickets.

