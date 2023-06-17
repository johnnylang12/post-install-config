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
<h3> Step 4: Allow Anyone To Create Tickets </h3> 
While in the Admin Panel, navigate to "Settings" -> "Users" -> "Settings" tab, -> uncheck "Require registration and login to create tickets".
</p>
<br />
<img src="https://i.ibb.co/2FRQCmZ/os-Ticket17.jpg" height="80%" width="60%" alt="Anyone can create"/>
</p>
<p>
<h3> Step 5: Configure Agents </h3> Now we will create agents, which are the help desk professionals who check and resolve tickets. <br/>
While in Admin Panel, go to "Agents" tab -> "Add New Agent". The first agent we'll name "Jane Doe" with an email "jane.d@osticket.com" and username "jane.doe". Click "Set Password", uncheck "Send the agent a password reset email" and enter a password for Jane. Make sure to note down Jane's info for later. Uncheck "Require password change at next login", and click "Set". We will assign Jane's department, role, and team. Under "Access" tab, select "System Administrators" for department and "Supreme Admin" for role. Under "Permissions" tab we'll leave everything checked then under "Teams" tab we will add her to "Level II Support", and then click "Create". <br/>
Repeat Step 5 to create a second agent with the name "John Smith", john.s@osticket.com, and username john.smith. Set his department as "Support" and "View only". Now you should be able to see Jane and John under "Agents" with their departments listed.
</p>
<br />
<img src="https://i.ibb.co/kmH9Yv9/os-Ticket18.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/R64WTmH/os-Ticket19.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/f1x5ST9/os-Ticket20.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/drBZ4gz/os-Ticket21.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/x6Xwcfs/os-Ticket22.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/ZLqHnr0/os-Ticket23.jpg" height="80%" width="60%" alt="New agents"/>
<img src="https://i.ibb.co/k2ZtHSG/os-Ticket24.jpg" height="80%" width="60%" alt="New agents"/>

</p>
<p>
<h3> Step 6: Configure Users </h3> Next, we will configure the users, these are the people opening tickets. <br/>
Switch to the "Agent Panel". Under "Users" tab, click "Create New User". Name the first user "Karen Karen" with an email of "Karen@osticket.com", then "Add User". <br/>
We will add one more user following the same steps with the name Ken Ken and Ken@osticket.com.
</p>
<br />
<img src="https://i.ibb.co/SvfN7V5/os-Ticket25.jpg" height="80%" width="60%" alt="New Users"/>
<img src="https://i.ibb.co/bKT7hdt/os-Ticket26.jpg" height="80%" width="60%" alt="New Users"/>
<img src="https://i.ibb.co/yncnc9M/os-Ticket27.jpg" height="80%" width="60%" alt="New Users"/>
</p>
<p>
<h3> Step 7: Configure SLAs </h3> Service Level Agreement (SLAs) is to prioritize requests and also provide a length of time in which the help desk administrator expects the tickets to be resolved. <br/>
Go back to the "Admin Panel" and navigate to "Manage" tab -> "SLA", Click "Add New SLA Plan". <br/>
Name this "SEV A" with a grace period of "1" (hours), and schedule of "24/7" then click "Add Plan". <br/>
This means that at any time a ticket comes in, it has to be resolved in 1 hour. <br/>
We will create two more SLAs. "SEV B", grace period of "4" (hours), schedule of "24/7", and finally "SEV C", grace period of "8" (hours), schedule "Monday-Friday".
</p>
<br />
<img src="https://i.ibb.co/vsmzxM7/os-Ticket28.jpg" height="80%" width="60%" alt="SLAs"/>
<img src="https://i.ibb.co/T1p6JBt/os-Ticket29.jpg" height="80%" width="60%" alt="SLAs"/>
<img src="https://i.ibb.co/DfD1p4h/os-Ticket30.jpg" height="80%" width="60%" alt="SLAs"/>

</p>
<p>
<h3> Step 8: Configure Help Topics </h3> Help topics help streamline ticket assignments for users. <br/>
In the Admin Panel, navigate to "Manage" tab -> "Help Topics", click "Add New Help Topic". <br/>
We will create the following 4 help topics: <br/>
"Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset".
</p>
<br />
<img src="https://i.ibb.co/DfD1p4h/os-Ticket30.jpg" height="80%" width="60%" alt="Help Topics"/>
<img src="https://i.ibb.co/qDT4FPC/os-Ticket31.jpg" height="80%" width="60%" alt="Help Topics"/>
<img src="https://i.ibb.co/MN7QXk1/os-Ticket32.jpg" height="80%" width="60%" alt="Help Topics"/>
<img src="https://i.ibb.co/pL9dfjn/os-Ticket33.jpg" height="80%" width="60%" alt="Help Topics"/>

</p>
<p>
<h2> That completes the set up and configuration of osTicket! </h2>
