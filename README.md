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

In this lab, we will be creating tickets as end users.
Observing all the ticket properties and responding to them as help desk professionals to completion.

Before continuing with the tickets we need to change the SysAdmins Department to a Top Level Department and delete the Maintenance Department.
- Open a browser and copy/paste the URL (http://localhost/osTicket/scp/login.php).
- Username: adminuser
- Password: Password1
- Click 'log In'

![image](https://github.com/user-attachments/assets/ac0799d2-8602-4dd8-9601-9835cd34b607)

- Admin Panel -> Agents -> Departments.
- Tick the boc for 'Maintentance'.
- Click on 'More' and click 'Delete'.
- Click 'Yes, Do it!'.

![image](https://github.com/user-attachments/assets/403f50d4-e9ca-4d88-9e24-b04f1c06a8ba)

![image](https://github.com/user-attachments/assets/bd641449-0b66-453a-b193-a7730dbbfebd)

- Click 'Log Out'.

![image](https://github.com/user-attachments/assets/5faf4e49-77d5-40cd-9045-aa3e39225ecf)

Ticket 1

1. Open a browser and copy/paste the URL (http://localhost/osTicket) and click 'Open a New Ticket' at the top of the bar.

![image](https://github.com/user-attachments/assets/879bfdbf-00c5-4ab9-ab71-2ec5f623b2a1)

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: Report a Problem
- Issue Summary: "entire mobile/online banking system is down".
- Details: "My employees are reporting that users are no longer able to access the online banking portal. The ones who can occasionally access it, cannot log in".
- Click 'Create Ticket'.

![image](https://github.com/user-attachments/assets/c253883f-1547-4b77-aae4-bf131da36d68)

2. Open a new tab in the browser, login to the osTicket Helpdesk login page as Helpdesk Agent "John". As a Help Desk Agent (john), observe the ticket’s properties.
- Username: john
- Password: Password1
- Click 'log In'

![image](https://github.com/user-attachments/assets/bb64c87d-103a-4fea-addd-3ac2c2375007)



Ticket 2

Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: Report a Problem
- Issue Summary: "entire mobile/online banking system is down".
- Details: "My employees are reporting that users are no longer able to access the online banking portal. The ones who can occasionally access it, cannot log in".
- Click 'Create Ticket'.



Ticket 3

Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: Report a Problem
- Issue Summary: "entire mobile/online banking system is down".
- Details: "My employees are reporting that users are no longer able to access the online banking portal. The ones who can occasionally access it, cannot log in".
- Click 'Create Ticket'.


------------------------------------------------------
------------------------------------------------------

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 



- Change the SysAdmins Department to a Top Level Department
- DELETE the Maintenance Department (not archive)


As a Help Desk Agent (john), observe the ticket’s properties
	- Priority
	- Department
	- SLA
	- Assigned To

Set Properties to the ticket
- Sev-A (1 hour, 24/7)
- Online Banking Department

Attempt to observe the ticket again as “john”. Can you view or change?

Work the ticket to completion as jane



As an end-user, create the following ticket
accounting department needs adobe upgrade, broken

As a Help Desk Agent (john), observe the ticket’s properties
	- Priority
	- Department
	- SLA
	- Assigned To

Set Properties to the ticket
- Sev-B (4 hours, 24/7)
- Support

Work the ticket to completion as john



As an end-user, create the following ticket
CFO’s laptop will no longer turn on

As a Help Desk Agent (john), observe the ticket’s properties
	- Priority
	- Department
	- SLA
	- Assigned To

Set Properties to the ticket
- Sev-B (4 hours, 24/7)
- Support

Work the ticket to completion as john

--------------------------------------------------

Set Properties to all the tickets; do SEV-A (SysAdmins last), observe ticket becomes inaccessible
Switch to admin panel and assign yourself View-access to Sys Admins
Switch to agent panel and observe the escalated ticket
Observe that you can no longer make changes to it

Solve all of the tickets
Explain in most ticketing systems (probably this one too) there is an email capability so every time you update the ticket, the user gets a copy and they can respond

Explain ticket intake IRL:
Sometimes tickets get created via phone, chat app, email, web form, or maybe even you run into someone in your hall or they roll up on you at your desk.
A lot of the time people will randomize you and try to get you to fix stuff on the spot. It’s fine to fix things on the spot, but generally speaking, you want to create tickets for EVERYTHING you do. (metrics are important)

Finishing up and additional practice
Obviously there is much more to this product that covered here
Encourage the use and exploration of the email feature
Do this lab a few more times, enough times where you’re able to implement it with this simple checklist. This will build your intuition.
Talk about Technical skill pillar
Re-touch on technical ability and re-doing the lab several times
