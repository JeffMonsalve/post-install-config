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

- Configure (Roles, Departments, and Teams)
- Allow anyone to create tickets
- Configure (Agents/Workers, and Users/Customers)
- Configure SLA
- Configure help topics 

<h2>Configuration Steps</h2>

<p>

![image](https://github.com/user-attachments/assets/f607958b-dab1-4621-a8ca-ba0ad5460f2c)
![image](https://github.com/user-attachments/assets/9731e18c-c60f-4a96-b525-51fcf823a112)
</p>
<p>
Now that osTicket has been successfully set up, the next step is to configure roles within the help desk. This allows you to effectively manage user permissions and access.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/0b890f3e-420b-4a62-b41f-cdfa1f6091ec)
![image](https://github.com/user-attachments/assets/63e26b6f-4781-4902-8de0-b9c3165caaf4)
</p>
<p>
Next, go to the Agents tab and click on the “Departments” button. Here, you’ll create a new department to organize agents based on their roles within the help desk. Start by creating a department called “System Administrators” and assign the appropriate agents to it. (need new image)
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/3816c5e6-dab3-41f0-b99b-32ca3a0f1ac3)
</p>
<p>
To allow anyone to create tickets without needing an account, go to Admin Panel > Settings > Users and uncheck the option “Require registration and login to create tickets.”
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/f7396431-2ef9-4156-ab24-fc406d0fd6f8)
</p>
<p>
Before tickets can be handled, we need to set up agents (workers). To do this, go to Admin Panel > Agents > Add New Agent, and fill in the required details such as name, email address, assigned role, and department. This creates each agent’s profile and assigns the appropriate permissions.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/e05d4b97-5f06-4511-97f6-86554dfb93a7)
</p>
<p>
Next, we connect to the domain controller (DC-1) using Remote Desktop (RDP). Once logged in, we disable the firewall for the domain, private, and public network profiles. This ensures that Client-1 can successfully ping DC-1’s private IP address later in the tutorial without any issues.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/cbc4ed95-29f3-4e4f-b819-509a1496c0ab)
</p>
<p>
Next, we connect to the domain controller (DC-1) using Remote Desktop (RDP). Once logged in, we disable the firewall for the domain, private, and public network profiles. This ensures that Client-1 can successfully ping DC-1’s private IP address later in the tutorial without any issues.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/ea2c2e4b-d431-4d18-a154-3be3484b334a)
