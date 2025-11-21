<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This project demonstrates the complete post-installation configuration of osTicket, an open-source help desk ticketing system. Building on a fresh osTicket deployment, this project focuses on configuring the system for real-world help desk operations by setting up departments, agents, roles, teams, help topics, SLAs, and email settings.<br />




<h2>Environments and Technologies Used</h2>

- osTicket 
- Microsoft Azure (Cloud Computing)
- Remote Desktop
- Windows 10 Professional x64 22H2

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10</b>

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

### - Intake
1. Navigate to `localhost/osTicket/index.php` and click the blue `Open a New Ticket` button.

<img width="1377" height="678" alt="image" src="https://github.com/user-attachments/assets/f41cb6ca-55fa-4e15-8577-c918a8c78910" />


2. Proceed to fill out the following fields with the relevant ticket information:
    - **Email Address**: The email address of whoever is submitting the ticket
    - **Full Name**: The full name of whoever is submitting the ticket
    - **Help Topic**: Click on the drop-down menu and select the issue that best fits with the issue in which the ticket is regarding
    - **Issue Summary** In the first field, enter a brief title for the issue and then proceed to the second field where a more detailed description is optional but recommended

In the end-user-created ticket example below, `Jane Doe` (best reached at `jane.doe1999@gmail.com` or `999-999-9999`) is submitting a ticket regarding her trouble to access online mobile banking.

<img width="1346" height="663" alt="image" src="https://github.com/user-attachments/assets/1305559d-f61b-408f-9f3d-38b7d46735b7" />


### - Assignment & Communication
1. Navigate to `localhost/osTicket/scp/login.php` and enter the credentials for the administrator that will assign an Agent to work on the ticket created during Intake.

<img width="1346" height="976" alt="image" src="https://github.com/user-attachments/assets/5bbdd6e6-871b-490c-89e9-bdc370558114" />


2. Navigate to `Tickets` > `Open` and then open the ticket by clicking the ticket number under the **Ticket** column.

<img width="1545" height="837" alt="image" src="https://github.com/user-attachments/assets/a4ea8d60-cd6b-48cd-856b-bb698e0b469c" />


3. From here, set the **Priority**, **Assign Department**, **Assigned To**, and the **SLA Plan** values for this ticket.

In the example below, the admin first clicks on the greyed out `— Unassigned —` text that's located to the right of **Assigned To**. Then, the admin designates `Luke Skywalker` as the **Assignee**.

<img width="1346" height="664" alt="image" src="https://github.com/user-attachments/assets/84ba32d2-5229-4cde-b04c-5c38894ef2fc" />


After the agent has been assigned to this particular ticket, the admin sets the **Priority** to `High`, the **Department** to `Support`, and the **SLA Plan** to `SEV-A`.

<img width="1346" height="664" alt="image" src="https://github.com/user-attachments/assets/2fa7ac44-e728-44d4-8e43-3c264b30e4dd" />


4. Within the ticket tab, you can see the thread of any updates to the ticket and submit updates upon assignment. Once finished, click the orange `Post Reply` button and the ticket gets assigned to the appropriate department and your customer gets notified of this change.

<img width="1346" height="990" alt="image" src="https://github.com/user-attachments/assets/93bc9637-cc69-4087-8380-29d043880e09" />


### - Working the Issue
1. Navigate to `localhost/osTicket/scp/login.php` and enter the credentials for the Agent that has been assigned to work on the ticket created during Intake.

<img width="1344" height="806" alt="image" src="https://github.com/user-attachments/assets/e543fe3d-188e-43fd-b2a1-7e134790d96d" />


2. Once logged in, the Tickets window shows. It will show the ticket number, the last time it was updated, the subject, who submitted the ticket, priority level, and who it is assigned to. The Agent must click on the ticket number to open it so that they can begin working through the problem.

<img width="1344" height="806" alt="image" src="https://github.com/user-attachments/assets/d5f07aaf-d9c7-47fe-8169-502b7ee9915e" />


3. Once the ticket is opened, you can review all ticket items and the history of the ticket items. This includes who submitted the ticket, who assigned the ticket, and any other ticket activity. The bottom section is where you can leave a reply for the user who submitted the ticket and an internal note to notify management if the ticket has been resolved.

<img width="1344" height="806" alt="image" src="https://github.com/user-attachments/assets/dce19332-ffd1-47c9-b94d-649dc626cd87" />


4. Once the Agent (Luke Skywalker) has reviewed all of the ticket details and identified a solution to the problem, the Agent can then use the **Post Reply** section to write a note to the user (Jane Doe) explaining everything, including the solution, in a professional manner.

<img width="1378" height="958" alt="image" src="https://github.com/user-attachments/assets/e2d1b77b-144d-48b4-801a-9f44a992cc54" />


### - Resolution

1. Before the user presses the orange `Post Reply` button to send the message to the user, it is important to navigate to the **Ticket Status** drop-down menu and change the value from `Open (current)` to `Closed`.

<img width="1378" height="958" alt="image" src="https://github.com/user-attachments/assets/1ca7cbc3-69d6-4e73-9213-c58142367b8a" />


2. Then, osTicket will take the Agent back to the Tickets tab. The Agent will then see a confirmation that the reply was posted successfully. As pictured below, ticket `#325542` by Jane Doe is no longer showing in the **Open** tickets section. Additionally, there is a visual confirmation banner at the top that says `Ticket #325542: Reply posted successfully`.

<img width="1378" height="594" alt="image" src="https://github.com/user-attachments/assets/ea5191ff-abb1-4611-9391-cf36bb263c7e" />


3. To view tickets that have been closed, Agents can navigate to `Tickets` > `Closed` > and then click the appropriate time frame that this ticket is from. From here, the Agent should see closed ticket in question.

<img width="1378" height="594" alt="image" src="https://github.com/user-attachments/assets/dc8513b1-6235-4bb0-aa20-f67f0573bb9a" />


<br><div align="center">


</div>
