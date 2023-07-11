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

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
<img width="1022" alt="Screen Shot 2023-07-10 at 9 48 34 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/95e736c8-3cab-40cc-9032-4e5d4adf5f8c">

</p>
<p>
1. Log in to the OsTicket - Admin Page
  
  - Log in to OsTicket using the admin cridentials created earlier in the installation process
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
- Check all boxes on the "Tickets", "Tasks" and "Knowledgebase"  sections under the "Permissions" tab.
- Click "Add New"

  
</p>
<br />

<p>
<img width="1058" alt="Screen Shot 2023-07-10 at 10 04 48 PM" src="https://github.com/SiclaitGitHub/post-install-config/assets/139138443/bfee5052-a6ca-453e-a99f-e35fda20f6f1">

</p>
<p>
3. Configure Departments 
</p>
<br />
