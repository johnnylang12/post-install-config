<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles, Departments, Teams, and Agents
- Allow Anoyone to Create Tickets 
- Configure Users
- Configure SLAs
- Configure Help Topics

<h2>Step-by-Step guide</h2>
Please see previous guide for installation and log in before proceeding https://github.com/johnnylang12/osticket-prereqs

<h3> Step 1: Configure Roles </h3> 
We will be creating a "Supreme Admin" role, and give this role full access. <br/>
Once logged in, we could see to the top right showing "Admin Panel" this means that we are in the agent portal. <br/>
Click Admin Panel -> "Agents" tab -> "Roles" -> "Add New Role". <br/>
Enter the name "Supreme Admin" then go to the Permissions tab and go check all boxes in all the tabs then click add role.

</p>
<br />
<img src="https://i.ibb.co/Vg8CQQB/os-Ticket5.jpg" height="80%" width="60%" alt="Roles permissions"/>
<img src="https://i.ibb.co/mCwhz6Y/os-Ticket6.jpg" height="80%" width="60%" alt="Roles permissions"/>
<img src="https://i.ibb.co/j8ZM8dn/os-Ticket7.jpg" height="80%" width="60%" alt="Roles permissions"/>
<img src="https://i.ibb.co/kcFMWgW/os-Ticket8.jpg" height="80%" width="60%" alt="Roles permissions"/>
<img src="https://i.ibb.co/xqfjdSm/os-Ticket9.jpg" height="80%" width="60%" alt="Roles permissions"/>
<img src="https://i.ibb.co/hRD9s3x/os-Ticket10.jpg" height="80%" width="60%" alt="Roles permissions"/>
</p>
<p>
<h3> Step 2: Configure Departments </h3> Next, we will create a department within Admin Panel. <br/>
While still in "Agents" tab after creating a role, click "Departments" -> "Add New Department". <br/>
We will name this department "System Administrators" and leave all the default settings then click "Create Department".
</p>
<br />
<img src="https://i.ibb.co/L8pWqZ4/os-Ticket11.jpg" height="60%" width="60%" alt="System Admins"/>
<img src="https://i.ibb.co/HdW1GQ9/os-Ticket12.jpg" height="80%" width="60%" alt="Roles permissions"/>

</p>
<p>
<h3> Step 3: Configure Teams </h3> Creating teams allows for multiple agents from different departments to collaborate together. <br/>
Same as before, while in "Agents" tab, click "Teams" -> "Add New Team". Call this team "Level II Support", and under the "Members" tab add yourself to the team.
</p>
<br />

<img src="https://i.ibb.co/BBzBCjJ/os-Ticket13.jpg" height="80%" width="60%" alt="Level II Support"/>
<img src="https://i.ibb.co/59JS8zC/os-Ticket14.jpg" height="80%" width="60%" alt="Level II Support"/>
<img src="https://i.ibb.co/0j2tNB2/os-Ticket15.jpg" height="80%" width="60%" alt="Level II Support"/>
<img src="https://i.ibb.co/F8G3B7G/os-Ticket16.jpg" height="80%" width="60%" alt="Level II Support"/>

</p>
<p>
<h3> Step 4: Allow Anyone To Create Tickets </h3> To do this in the Admin Panel, navigate to "Settings", "Users", "Settings", and uncheck "Require registration and login to create tickets".
</p>
<br />
<img src="https://i.imgur.com/rzXZ60d.png" height="80%" width="80%" alt="Anyone can create"/>
</p>
<p>
<h3> Step 5: Configure Agents </h3> Now we will create some agents, which are the help desk professionals who check and resolve tickets. In the Admin Panel, under "Agents", click "Add New Agent". The first agent will be named "Jane Doe" with an email of "jane.doe@osticket.com" and username "jane.doe". Make sure to note Jane's username for later. Click "Set Password", uncheck "Send the agent a password reset email", and enter a password for Jane. Once again, make note of this password for later. Uncheck "Require password change at next login", and click "Set". On the other tabs, this is where we can set Jane's permissions, add her to a team, and her department. Under "Access" We will put Jane in the "System Administrators" department as a "Supreme Admin". In "Teams" we will add her to "Level II Support", and then click "Create". Follow Step 5 to create a second agent with the name "John Doe". Set his department as "Support" and "View only". Now you should be able to see Jane and John under "Agents" with their departments listed.
</p>
<br />
<img src="https://i.imgur.com/trv3weH.png" height="80%" width="80%" alt="New agents"/>
</p>
<p>
<h3> Step 6: Configure Users </h3> Next, we will configure the users, who simply put, are the people opening tickets. To add users, switch to the "Agent Panel". Under "Users", click "Create New User". Name the first user "Karen Karen" with an email of "Karen@osticket.com", and "Add User". We will now add one more user. Following the same steps with the name Ken.
</p>
<br />
<img src="https://i.imgur.com/GFUOmmu.png" height="80%" width="80%" alt="New Users"/>
</p>
<p>
<h3> Step 7: Configure SLAs </h3> The purpose for the Service Level Agreement is to prioritize requests and also provide a length of time in which the help desk administrator expects the tickets to be resolved. So we will do this next. Go back to the "Admin Panel" and navigate to "Manage", and "SLA" where we will create 3 SLA plans. Click "Add New SLA Plan", naming it "SEV A", a grace period of "1" (hours), and schedule of "24/7". This means that at any time a ticket comes in, it has to be resolved in 1 hour. Next make two more SLAs, one called "SEV B", a grace period of "4" (hours), schedule of "24/7", and finally "SEV C", grace period of "8" (hours), schedule "Monday-Friday".
</p>
<br />
<img src="https://i.imgur.com/pnthCaA.png" height="80%" width="80%" alt="SLAs"/>
</p>
<p>
<h3> Step 8: Configure Help Topics </h3> Help topics help streamline tickets assignments for users, so we will configure a few now. In the Admin Panel, navigate to "Manage", "Help Topics", and click "Add New Help Topic". We will create the following 4 help topics: "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset".
</p>
<br />
<img src="https://i.imgur.com/N7dOIZu.png" height="80%" width="80%" alt="Help Topics"/>
</p>
<p>
<br />
<br/>
<h2> That completes the set up and configuration of osTicket! </h2>
