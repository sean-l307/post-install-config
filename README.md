# post-install-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Configuration Steps</h2
                         
- Set up Roles
- Configure Departments
- Create Teams
- Download and install the Rewrite Module
- Enable ticket creation for anyone
- Set up Agents (employees)
- Set up Users (customers)
- Configure SLAs

<h2>Detailed Steps</h2>


![capture1](https://github.com/user-attachments/assets/40878a90-9a0f-484b-aabe-1490cc6ed039)
</p>
<p>
First, navigate to the login page (http://localhost/osTicket/scp/login.php) and sign in using the admin credentials created in the previous tutorial.
</p>
<br />

![Capture2](https://github.com/user-attachments/assets/2c1a8e44-513e-49cd-8c73-8f270dddde09)
</p>
<p>
Next, click on 'Admin Panel' located at the top right of the screen. Once you're in the admin panel, the button will change to 'Agent Panel.
</p>
<br />

![Capture3](https://github.com/user-attachments/assets/a412a2de-f93e-43d6-94a8-95e8bf75b360)
</p>
<p>
Next, navigate to Agents > Roles and click 'Add New Role.' Name the role 'Supreme Admin,' then grant all permissions in the following tab. Finally, click 'Add Role.</p>
<br />

![Capture4](https://github.com/user-attachments/assets/d664795f-c337-4561-a4a7-165556f7077e)
</p>
<p>
Go to 'Departments' and click on 'Add New Department.' Enter 'SysAdmins' as the department name, then click 'Create Dept.
</p>
<br />

![Capture5](https://github.com/user-attachments/assets/1dfcd0ae-5ea7-4058-ab06-1c6a698b7839)
</p>
<p>
 Head to the "Teams" panel and click "Create New Team". Name the new team "Online Banking" and press create.
</p>
<br />


![Capture6](https://github.com/user-attachments/assets/7247a4af-2d69-4aee-9e12-4dc07f0a4e08)
</p>
<p>
Next, navigate to 'Settings' > 'Users' and ensure the box for registration requirement is unchecked. Set the method to 'Public,' then click 'Save Changes.
</p>
<br />


![Capture7](https://github.com/user-attachments/assets/28262ac2-3fe0-4aff-b6a4-ea7ada9797f2)
</p>
<p>
 Now, switch to the Agent Panel and click 'Add New Agent.Create these accounts:

- Name: Jane Doe
- Email Address: jane.doe@osticket.com
- Username: jane.doe
- Set the password to "Password1"
- Go to Access and set the department to SysAdmins and select Supreme Admin for the role.
Go to the teams section and select Level II Support, then create.
After, create a second account for " John Doe"
</p>
<br />


![Capture8](https://github.com/user-attachments/assets/25990602-9e4c-4814-8260-ff23bba4e9ca)
</p>
<p>
Next, navigate to the Agent Panel, go to 'Users,' and click 'Add User.

- Add the following users:
- Email Address: karen@osticket.com
- Full Name: Karen
- Email Address: ken@osticket.com
- Full Name: Ken
</p>
<br />

![Capture9](https://github.com/user-attachments/assets/8acc1d27-731e-4cb4-a80e-1ebf7102f77e)
</p>
<p>
Head to Admin Panel > Manage > SLA > Add New SLA Plan.
</p>
<br />

![Capture10](https://github.com/user-attachments/assets/362fb5b8-b48c-4dfb-b8f3-c8a1fb9a7ef5)
</p>
<p>
Next, add the following SLAs
- SEV-A with a grace period of 1 hour, and a 24/7 schedule
- SEV-B with a grace period of 4 hours, and a 24/7 schedule
- SEV-C with a grace period of 8 hours, and a Mon-Fri business hours schedule
</p>
<br />

![Capture12](https://github.com/user-attachments/assets/7d644d4d-31cd-43a7-a3b4-ea1c6baae749)
</p>
<p>
Now, navigate to "Help Topics" and add the following help topics:
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
</p>
<br />
