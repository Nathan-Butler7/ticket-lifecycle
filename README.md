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

1. Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

![Screenshot 2025-05-15 104349](https://github.com/user-attachments/assets/d5efb419-e1ce-4014-a853-b0e06c6881d3)

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: General Inquiry / Other
- Issue Summary: "accounting department needs adobe upgrade, broken".
- Details: "It looks like many people in the account department can't use their adobe software".
- Click 'Create Ticket'.

![image](https://github.com/user-attachments/assets/503f6312-3387-464f-be6b-e0a094a2331f)

![image](https://github.com/user-attachments/assets/bf9db5b4-b3d2-4b7d-b9b1-191d4542cb3d)

2. Open a new tab in the browser (http://localhost/osTicket/scp/login.php), login to the osTicket Helpdesk login page as Helpdesk Agent "John".
- Username: john
- Password: Password1
- Click 'log In'

![image](https://github.com/user-attachments/assets/103e57bd-752e-46e6-8a4d-eb4901ba0267)

3. Click on the new ticket that was just created. Read the issue summary and description and observe the properties as a Help Desk Agent (John).
- When reviewing the issue, the title and explanation seem hard to understand. It may not be necessary to upgrade the Adobe software—it simply might not be usable for another reason. This calls for further investigation.
In this mock scenario, I respond to Ken by asking: "What exactly do you mean by 'many people in the accounting department can't use their Adobe software'?"
Ken clarifies that "only two people in the accounts department are unable to use Adobe Reader." This clarification helps narrow down the issue, allowing us to identify the specific scope of the problem and move on to the next step.

![image](https://github.com/user-attachments/assets/47bf94e7-15d2-4e1f-aa45-cf1f44b03a77)

Set Properties to the ticket
- SLA Plan: Sev-C (8 hours, [Business Hours])

![image](https://github.com/user-attachments/assets/8c7a3af1-0679-4ef9-8f45-2ecd62de2b7b)

- Assigned to: John Doe

![image](https://github.com/user-attachments/assets/4a202de4-dd71-4143-8788-5a60fcde264c)

- If you scroll down and observe you can see updates in Ticket Thread.

![image](https://github.com/user-attachments/assets/855d4b6a-9183-4848-8b3b-3e13e04f50eb)

4. Navigate to the 'Post Reply' section. Respond to the ticket with a possible explanation of the issue and begin investigating to confirm whether this is the actual cause. My reply will be:
- "Customer states only 2 people in the accounting department are unable to open and use Adobe reader. I have asked the customer to conduct restarts, he will call back after lunch."
- Click 'Post Reply', refresh the ticket and you should see that it has been updated in the ticket history.

![image](https://github.com/user-attachments/assets/8fd13da5-1b7b-4bef-92d3-fe869affd56b)

![image](https://github.com/user-attachments/assets/4f38eb52-5ca3-4c89-911b-d8b9a37eb276)

5. Let’s assume lunch is over and the customer has responded, confirming that a restart resolved the issue and everything is now working correctly and there's no problems.

Post another reply in the Ticket Thread:
- "Customer states that restart fixed issue, closing out ticket".

![image](https://github.com/user-attachments/assets/3c33f497-6e67-4666-9138-368740852da7)

![image](https://github.com/user-attachments/assets/3ec39683-40f9-4549-8172-2c5b330ed092)

6. Now that everything is fixed we can now finish up the Ticket.
- Change Ticket Status to "Resolved".
- "Restart fixed for both users".
- Click 'Close'.

![image](https://github.com/user-attachments/assets/961d11d5-d333-43e6-a9cf-f168faeff5d4)

![image](https://github.com/user-attachments/assets/1f53468b-c8bf-4924-b995-ae5e3741c772)

- You can check Closed Tickets by logging in back as 'Adminuser'.

![image](https://github.com/user-attachments/assets/610767d3-f4fe-4a77-86ad-8f3dc988df2a)

Ticket 3

1. Back to the End User osTicket URL (http://localhost/osTicket), click 'Open a New Ticket' at the top of the bar.

![Screenshot 2025-05-15 104349](https://github.com/user-attachments/assets/750156d6-057c-433e-b84d-2dac5f9e194b)

We will use the "Karen" account. Fill in the following sections:
- Email Address: karen@lognpacific.com
- Full name: Karen
- Phone Number: 5038884757
- Help Topic: Report a problem / Personal Computer Issues
- Issue Summary: "CFO’s laptop will no longer turn on".
- Details: "Laptop won't power on, despite of pressing the power button."
- Click 'Create Ticket'.

![image](https://github.com/user-attachments/assets/6c6b0043-4871-451e-a12f-81c72ca57d33)

![image](https://github.com/user-attachments/assets/73e92871-5ae5-4d3b-9f0d-d096a01a1050)

2. Open a new tab in the browser (http://localhost/osTicket/scp/login.php), login to the osTicket Helpdesk login page as Helpdesk Agent "John".
- Username: john
- Password: Password1
- Click 'log In'

![Screenshot 2025-05-15 233109](https://github.com/user-attachments/assets/17aaebc8-bce8-4696-ae36-cb36be483706)

3. Click on the new ticket that was just created. Read the issue summary and description and observe the properties as a Help Desk Agent (John).

![image](https://github.com/user-attachments/assets/60f4ebc9-73fa-4986-9fa3-5b37514a9190)

Set Properties to the ticket
- Priority: High (Because this is the CFO it is a high priority customer)

![image](https://github.com/user-attachments/assets/148f4d75-2b38-45f0-a1db-ce063fa238b2)

- SLA Plan: Sev-B (4 hours, 24/7)
- (Optional) "may re-classify after getting more info."

![image](https://github.com/user-attachments/assets/e6416c91-618d-46ff-bf01-f65b0dd74e93)

- Assigned to: John Doe

![image](https://github.com/user-attachments/assets/299215ab-1a9a-4197-b381-af99b32fb9c8)

- If you scroll down and observe you can see updates in Ticket Thread.

![image](https://github.com/user-attachments/assets/c76e85c1-e1bc-4a5a-a39b-5edf26b9ed1d)


4. Navigate to the 'Post Reply' section. Respond to the ticket with a possible explanation of the issue and begin investigating to confirm whether this is the actual cause. My reply will be:
- "CFO's laptop was not charging due to broken charger, brought new charger and is now successfully charging."
- Click 'Post Reply', refresh the ticket and you should see that it has been updated in the ticket history.

![image](https://github.com/user-attachments/assets/1490500e-cfab-4d57-b4c2-b7a2fda6d6d9)

![image](https://github.com/user-attachments/assets/d9b2aa5f-8821-4681-bfc7-314e4979dc69)

5. Now that everything is fixed we can now finish up the Ticket.
- Change Ticket Status to "Resolved".
- "Charger was broken, because of this, battery was dead and unable to turn on".
- Click 'Close'.

![image](https://github.com/user-attachments/assets/110774e1-8c45-42af-b3f0-25b5081c8d3a)

![image](https://github.com/user-attachments/assets/b4ba061d-6799-4e31-8c79-2f2448bdb03c)

- You can check Closed Tickets by logging in back as 'Adminuser'.

![image](https://github.com/user-attachments/assets/58280cc0-c552-4089-ab28-7a731f68767d)


--------


Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 


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
