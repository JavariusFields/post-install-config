<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles, Departments, and Teams
- Set up everyone to be able to create tickets
- Configure Workers and Customers
- Configure SLA 
- Configure Help Topics

<h2>Configuration Steps</h2>
<p>
1. Log into the OsTicket dashboard with the password created during the installation. We need to configure and admin role. We can access it by clicking Admin Panel in the top right -> Agents -> Roles. Create a new role that has complete admin access and name it "Supreme Admin". It should have all privileges.
<img width="841" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/3e6ff94d-9f15-41f8-987e-d11aaee044ec">
<img width="516" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/7cf33254-8c93-49b8-a470-93c5d686d5ae">
<img width="783" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/efe04a49-db78-4432-8a82-cc4d3971b51e">
<img width="947" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/35204186-10ec-409c-96ba-29dd657bb059">
<p>
2. Configure departments by going back to the Admin Panel -> Agents -> Departments. Add a few departments. For this tutorial, I added System Administrators as a department.
<p>
<img width="945" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/747a3e64-1ddd-4b1d-8d65-f9787c6406d2">
3. Configure teams in the same panel (Admin Panel) -> Agents -> Teams. Click "Add Team". We'll add Level II and Level III Support.
<p>
<img width="953" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/5cf58f57-e5aa-4019-80fe-05709a889638">

4. We need to allow anyone to create tickets and this can be done inside of the admin panel too. Go to Settings-> User Settings. Make sure Registration Required is not checked otherwise when whe create users for the next exercise, we wont be able to log in and resolve tickets. In a real life situation, we wouldn't do this.

<img width="881" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/ae8d6250-bd33-4133-b005-1e75e51bcbc4">

5. Configure agents in this same panel. Just click agents-> add new. We'll add 3 generic users here. I used Cornelius Fudge, Sirius Black, and Lily Potter. Also, when setting up the password, uncheck the two boxes (obviously we wouldn't do this in real life. This is to see how configuring roles in the system works and the emails i'm making, they aren't real.

<img width="645" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/e7b608b9-e870-4674-8ae0-08283fd73ea8">

7. Configure a few customers by clicking Agent Panel -> Users -> Add New. For this example, i added Tom Riddle and Lucius Malfoy

<img width="945" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/f5457654-ed3f-41b2-9b80-0e4fa6415ba7">

8. Configure SLA. Go back to the Admin Panel for this then, Manage -> SLA. Create 3 Service Level Agreements (SLA). Sev-A (1 hour, 24/7), Sev-B (4 hours, 24/7), Sev-C (8hours, business hours)
   
<img width="699" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/803b5a4e-028a-49bf-b437-bd69c2554a05">
<img width="949" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/4dbc8539-0fb8-413b-b99c-4ff727559458">

Finally, configure some help topics. Admin Panel -> Manage -> Help Topics. Add the following help topics: Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset. It should look something like this 
<img width="949" alt="image" src="https://github.com/JavariusFields/post-install-config/assets/144845191/ec03c92e-e4dc-41ff-9c36-51c0e4fb029f">




