<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Teams
- Enable Ticket Creation Permission To All Users
- Configure Agents (Workers)
- Configure Users (Customers)
- Configure SLA Plans
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img width="1022" alt="Screen Shot 2023-07-10 at 9 48 34 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/95e736c8-3cab-40cc-9032-4e5d4adf5f8c">

</p>
<p>
1. Log in to the osTicket - Admin Panel
  
  - Log in to osTicket using the admin credentials created earlier in the installation process
  - Select "Admin Panel" on the top right of the osTicket window.

  
<br />

<p>
<img width="1108" alt="Screen Shot 2023-07-10 at 9 56 07 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/cabf9569-8cbc-4c7b-a362-4120abdece0a">

</p>
<p>
2. Configure Roles

Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. An unlimited number of roles can be created and assigned to Agents with access to various departments.

- When on the "Admin Panel" of the osTicket Window selects "Agents" then select "Roles"
- Name the new role "Supreme Admin" then click on the "Permissions" tab.
- Check all boxes on the "Tickets", "Tasks" and "Knowledge Base"  sections under the "Permissions" tab.
- Click "Add New"

  
</p>
<br />

<p>
<img width="1058" alt="Screen Shot 2023-07-10 at 10 04 48 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/bfee5052-a6ca-453e-a99f-e35fda20f6f1">

</p>
<p>
3. Configure Departments 

Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department.

- Create a title for the new department. Here "System Administrator" is being used 
</p>



<img width="1076" alt="Screen Shot 2023-07-10 at 10 16 10 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/91378c03-6b0a-4af4-92d3-fd2f56d418fc">


4. Configure Teams

Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter.

- On the "Admin Panel" of the osTicket window select the "Teams" tab.
- Click "Add New Team"
- Create a title for the team. Here "Level 2 Support" is being used 
- Click "Create Team"
<br />


<img width="1059" alt="Screen Shot 2023-07-10 at 10 32 46 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/b07b3607-0cdb-440d-ab9b-a7939f5a3f7d">

5. Enable Ticket Creation Permission To All Users

- In the "admin Panel" of osTicket select the "Users" tab under "Settings"
- Make sure that the "Require registration and login to create tickets" box is unchecked
- Click "Save Changes"


<img width="1099" alt="Screen Shot 2023-07-10 at 10 48 13 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/17d5e843-7783-4fcc-b190-b9f1efb2f5a1">

6. Configure Agents (Workers)

Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent’s Profile.

- On the "admin Panel" in the osTicket window select the "Agents" tab.
- Select "Add New Agent"
- Create "Jane Doe" as new agent in addition to log in cridentials for the new agent account.
- Create "John Doe" as new agent in addition to log in cridentials for the new agent account.
- Make sure 'Send the agent a password reset email" and "Require password change at next login" boxed are unckecked when setting password
- In the "Access" tab under the "Agents" tab assign select appropriate "Department" and "Role" for each agent.
- Click "Create"


<img width="1068" alt="Screen Shot 2023-07-11 at 12 15 08 AM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/7416790d-155e-4f75-b367-145c2d3b25f0">


7. Configure Users (Customers)

Users are the ticket owners of the tickets in the help desk. When a ticket is created in the help desk, the user is associated with their email address in the User Directory of the help desk. Users can be added or deleted from the User Directory of the help desk at any time. Please note, if the user is deleted the tickets of the user must also be deleted.

- Click on "Agent Panel" on the top right corner of the osTicket window
- Select "Users" and clike on "Add User"
- Create "Ken Block" as a new user in addition to log in credentials for the new user account.
- Create "Karen Block" as a new user in addition to log in credentials for the new user account.
- Click "Add User"


<img width="1103" alt="Screen Shot 2023-07-11 at 12 20 39 AM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/9c462e0c-68d9-4d73-a8ff-3ff7a83459d0">

8. Configure SLA Plans

SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.

- In the "Admin Panel" of the osTicket window click on "Manage" the select "SLA Plans" 
- Click on the top right of the table to “Add New SLA Plan.”
- Name SLA Plan "SEV A" - High Priority (1 Hour Grace Period) then click "Add Plan".
- Name SLA Plan "SEV B" - Moderate Priority (4 Hour Grace Period) then click "Add Plan".
- Name SLA Plan "SEV C" - Low Priority (8 Hour Grace Period) then click "Add Plan".


<img width="1066" alt="Screen Shot 2023-07-11 at 12 37 31 AM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/dc0bf49a-cc14-4c9e-bc62-c958fb712dcd">


9. Configure Help Topics

Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for further breakdown (For example, Human Resources and Human Resources/Payroll.)

- In the "Admin Panel" of the osTicket window, click on "Manage" the select "Help Topics" 
- Click on “Add New Help Topics”
- Add the following Help Topics: "Business Critical Outage", "Personal Computer Issues", "Equipment Request" and "Password Reset"
- After each Help Topic click "Add Topic"

  

