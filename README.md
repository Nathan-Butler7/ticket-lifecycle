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
- Tick the box for 'Maintentance'.
- Click on 'More' and click 'Delete'.
- Click 'Yes, Do it!'.

![image](https://github.com/user-attachments/assets/403f50d4-e9ca-4d88-9e24-b04f1c06a8ba)

![image](https://github.com/user-attachments/assets/bd641449-0b66-453a-b193-a7730dbbfebd)

We also need to assign our agents to a 'Team' (level 1 Support) - (Online Banking)

In the admin portal and click Agents > Teams > choose "Online Banking".

![Screenshot 2025-05-15 140031](https://github.com/user-attachments/assets/b0678c84-6740-43b4-81ef-24cda460c364)

- Go to Members, and then when you select an agent be sure to click the "add" button after you select the agent.
- We will be adding both agents and yourself(adminuser) to the team.
- Click 'Save Changes'.

![image](https://github.com/user-attachments/assets/0fdf8090-a534-40f8-bac2-ad8fb6f58a40)

- Click on 'Teams' then click on 'Level 1 Support'.
- Go to Members, and then when you select an agent be sure to click the "add" button after you select the agent.
- We will be adding both agents and yourself(adminuser) to the team.
- Click 'Save Changes'.

![image](https://github.com/user-attachments/assets/caa5c289-b30e-417a-94b4-e58cff949fd0)

- Check 'Teams'.
- Click 'Log Out'.

![image](https://github.com/user-attachments/assets/c04d3fd3-fe5b-4a86-b004-1ef9cd5c8047)


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

![image](https://github.com/user-attachments/assets/9b784421-9e37-4267-a664-c34e4485bb80)

2. Open a new tab in the browser, login to the osTicket Helpdesk login page as Helpdesk Agent "John".
- Username: john
- Password: Password1
- Click 'log In'

![image](https://github.com/user-attachments/assets/bb64c87d-103a-4fea-addd-3ac2c2375007)

3. Click on the new ticket that was just created. Read the issue summary and description and observe the properties as a Help Desk Agent (John).

![image](https://github.com/user-attachments/assets/20c0ceb9-6b21-4d24-9a3b-751cb9c85da8)

Set Properties to the ticket
- SLA Plan: Sev-A (1 hour, 24/7)
- (Optional) "Wide impact, customers unable to do online banking".

![image](https://github.com/user-attachments/assets/3644cbd3-1b7b-4833-a674-c33fecde8852)
  
- Help Topic: Report a Problem / Business Critical Outage. (It can be important to organise the topic it's more relevant to).
- (Optional) "No customers able to access online banking".

![image](https://github.com/user-attachments/assets/bb72c8ef-9da8-4140-9ac1-b9c86eb0bfbb)

- Assigned to: Online Banking Department
- (Optional) "Customers not able to access online banking portal, assigning to online banking team".

![image](https://github.com/user-attachments/assets/482bd93a-83c4-4eda-932f-6be21de5a7cd)

- If you scroll down and observe you can see updates in Ticket Thread.

![image](https://github.com/user-attachments/assets/f209e08c-a2fb-4eb6-a122-55f16da1f965)

4. Log out of the Helpdesk login page. Re-login with the "Jane" account and work the ticket to completion as Jane.
- Username: jane
- Password: Password1
- Click 'Log In'.

![image](https://github.com/user-attachments/assets/df69d39e-bb33-41ac-978f-03a5ed848866)

- In the 'Tickets' section and locate the ticket listed under 'Open'. Click on the ticket to view its details, then proceed to resolve it while logged in as the user 'Jane'. 

![image](https://github.com/user-attachments/assets/134e5552-b09d-48dd-b052-9382d1147b28)

5. It's possible the 'Online Banking' team has more than one person in it and Jane just so happened to pick it up and assign it to herself.
- Assigned To: Jane Doe
- (Optional) "I'll be taking over this ticket".

![image](https://github.com/user-attachments/assets/0b1db8fe-1eb2-49ce-95a3-c1de877b23a2)

6. Navigate to the 'Post Reply' section. Respond to the ticket with a possible explanation of the issue and begin investigating to confirm whether this is the actual cause. My reply will be:
- "I suspect the problem might be related to the recent updates. We tested it sufficiently, but I am going to look into it further and roll it back if that caused the issue".
- Click 'Post Reply', refresh the ticket and you should see that it has been updated in the ticket history.

![image](https://github.com/user-attachments/assets/95429390-d6cf-4ffc-85fb-4c5ee298a001)

![image](https://github.com/user-attachments/assets/adc24032-02c5-44a1-8336-2b16be1c3c64)

7. Post another reply in the Ticket Thread:
- "It was determined that the root cause was the recent update. We rolled it back, notified the vendor and are waiting for a proper fix. Online banking should be up and running".
- Click 'Post Reply', refresh the ticket and you should see that it has been updated in the ticket history.

![image](https://github.com/user-attachments/assets/56d52be9-01e3-428d-a2e9-aa1ad9f5e96f)

![image](https://github.com/user-attachments/assets/804b3b9a-b040-4fe1-ba27-e04df1c6bedb)

8. Now that everything is fixed we can now finish up the Ticket.
- Change Ticket Status to "Resolved" and click close.

![image](https://github.com/user-attachments/assets/837ed3ea-a184-4347-8681-74c37068fbcc)

![image](https://github.com/user-attachments/assets/992ecf12-1003-4442-9f2b-41cd88e6d97a)

- You can check Closed Tickets by logging in back as 'Adminuser'.

![image](https://github.com/user-attachments/assets/75429cb1-b025-44de-98a1-b7ee1d25b2a6)

Ticket 2

Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

![Screenshot 2025-05-15 104349](https://github.com/user-attachments/assets/d5efb419-e1ce-4014-a853-b0e06c6881d3)

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: 
- Issue Summary: " ".
- Details: " ".
- Click 'Create Ticket'.




Ticket 3

Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

![Screenshot 2025-05-15 104349](https://github.com/user-attachments/assets/750156d6-057c-433e-b84d-2dac5f9e194b)

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: 
- Issue Summary: " ".
- Details: " ".
- Click 'Create Ticket'.


------------------------------------------------------
------------------------------------------------------

Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 



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
