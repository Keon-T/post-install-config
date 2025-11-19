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

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Admin panel
- Agents (workers)
- Roles
- User (customer)
- User settings

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/84oSCmk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Configuring roles grouping permissions to users on admin access panel

  Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking

</p>
<br />

<p>
<img src="https://i.imgur.com/OImAMZH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Admin Panel -> Settings -> User Settings then check Registration Required, login to create tickets Require registration 

  Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken


</p>
<br />

<p>
<img src="https://i.imgur.com/H3IHVwn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


Service Level Agreement (sla) how much time there is to respond/complete tickets in admin panel. Go to schedule department creating 3 different sla with 3 different grace periods</p>

Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)


<br />
