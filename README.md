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

- Configured Roles and Permissions
- Configured Departments and Teams
- Configured Agents and Users
- Configured System Accessibility & Ticketing
- Configured SLA and Ticket Management

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/txVlPSU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is the Admin Panel on osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/dhSDh1X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is the Agent Panel on osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/gxDxwsZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Roles (for grouping permissions). Went to Admin Panel -> Agents -> Roles. Created a new role called "Supreme Admin"
</p>
<br />

<p>
<img src="https://i.imgur.com/rFHrthf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Gave the "Supreme Admin" role all permissions
</p>
<br />

<p>
<img src="https://i.imgur.com/cJ3u78K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Departments (for Ticket Visibility purposes, Help Desk vs SysAdmins vs Networking). Went to Admin Panel -> Agents -> Departments and configured a new department "SysAdmins".
</p>
<br />

<p>
<img src="https://i.imgur.com/3yddAKj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Added "SysAdmins" to the list of currently existing departments.
</p>
<br />

<p>
<img src="https://i.imgur.com/145sVKQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Teams (The purpose of teams are to pull agents from different departments). Went to Admin Panel -> Agents -> Teams. Created an "Online Banking" team. 
</p>
<br />

<p>
<img src="https://i.imgur.com/vlYnoOi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Allowed anyone to create tickets. Went to Admin Panel -> Settings -> User Settings. Unchecked "Require registration and login to create tickets" so unregistered users can create tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/AFg13pp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Agents (workers). Went to Admin Panel -> Agents -> Add New Agent. Added Jane (who is in the "SysAdmins" department) & John (who is in the "Support" department).
</p>
<br />

<p>
<img src="https://i.imgur.com/S9Yr8pz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Users (customers). Agent Panel -> Users -> Add User. Added Karen as a user.
</p>
<br />

<p>
<img src="https://i.imgur.com/OhmXGqI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured SLA. Went to Admin Panel -> Manage -> SLA. Created Sev-A (Grace Period: 1 hour, Schedule: 24/7), Sev-B (Grace Period: 4 hours, Schedule: 24/7), Sev-C (Grace Period: 8 hours, Business Hours). The “Sev” levels (Sev-A, Sev-B, and Sev-C) represent different severity levels of service level agreements (SLAs).
</p>
<br />

<p>
<img src="https://i.imgur.com/tQqAjGX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Help Topics (For when users create a ticket). Went to Admin Panel -> Manage -> Help Topics. Added the Help Topics "Business Critical Outage", "Personal Computer Issues", "Equipment Request", "Password Reset", "Other"
</p>
<br />
