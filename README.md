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

- Configure Roles, Deparments, and Teams in Admin Panel
- Configure Agents and Users and assign departments
- Add SLA's and descriptions
- Add Help Topics when users create tickets

<h2>Configuration Steps</h2>

<br/>
Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
<p>
type 'Supreme Admin'
</p>
<img width="1536" alt="Screenshot 2025-02-17 at 2 47 01 PM" src="https://github.com/user-attachments/assets/3907a5a1-92ff-4d28-870d-25f7b1ce6804" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 47 33 PM" src="https://github.com/user-attachments/assets/4311f34c-f129-4c0c-8683-72ef29bf06b6" />



<br /><br />
Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
<p>
type 'SysAdmins'
</p>
<img width="1536" alt="Screenshot 2025-02-17 at 2 50 45 PM" src="https://github.com/user-attachments/assets/2a47e60d-4054-4343-8e82-1af419eeda9d" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 51 17 PM" src="https://github.com/user-attachments/assets/2491e9ac-8ee6-4a35-a130-46723292c18f" />


<br /><br />
Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
<p>
type 'Online Banking'
</p>
<img width="1536" alt="Screenshot 2025-02-17 at 2 52 16 PM" src="https://github.com/user-attachments/assets/60ba2e9e-2772-432b-9444-62035a035509" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 52 34 PM" src="https://github.com/user-attachments/assets/7efa7c1e-0cfa-4e07-baf7-4b213d1529b0" />


<br />


Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
<img width="1536" alt="Screenshot 2025-02-17 at 2 53 30 PM" src="https://github.com/user-attachments/assets/56265bda-f61e-495a-9247-5781a03a5040" />
<br />


Configure Agents (workers)
Admin Panel -> Agents -> Add New
<p>
-Jane (Dept: SysAdmins)
-John (Dept: Support)
</p>
<img width="1536" alt="Screenshot 2025-02-17 at 2 54 10 PM" src="https://github.com/user-attachments/assets/b34ccadf-61f8-4251-b7f7-6dd8ed2a9fd2" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 55 14 PM" src="https://github.com/user-attachments/assets/7a036f04-9b10-4518-b142-72f9e800ab64" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 56 00 PM" src="https://github.com/user-attachments/assets/0ec8472f-84b6-4411-b3ed-c53fba6c3ec1" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 59 49 PM" src="https://github.com/user-attachments/assets/2ca6b778-d447-43a4-98a4-8ffbd659208d" />
<img width="1536" alt="Screenshot 2025-02-17 at 2 59 51 PM" src="https://github.com/user-attachments/assets/2f2c63ca-a329-44e3-b8a5-03c494f9f0c9" />



Configure Users (customers)
Agent Panel -> Users -> Add New
<p>
-Karen
</p>
<img width="1536" alt="Screenshot 2025-02-17 at 3 02 52 PM" src="https://github.com/user-attachments/assets/098f6853-8abe-4b13-987d-00c615b222e3" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 03 08 PM" src="https://github.com/user-attachments/assets/3c6b831d-27d7-44e6-a48d-e32d3b9cc76b" />
<br /><br />

Configure SLA
Admin Panel -> Manage -> SLA
<ol>
<li>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</li>
<li>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</li>
<li>Sev-C (Grace Period: 8 hours, Business Hours)</li>
</ol>
<img width="1536" alt="Screenshot 2025-02-17 at 3 04 38 PM" src="https://github.com/user-attachments/assets/dcf83c6e-1b04-42d9-8453-1ccb96a2252f" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 05 22 PM" src="https://github.com/user-attachments/assets/8f637054-df59-4c22-9376-d0f4667b134d" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 05 51 PM" src="https://github.com/user-attachments/assets/1b075907-8a41-4be9-985f-fd1c9b52ee94" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 06 12 PM" src="https://github.com/user-attachments/assets/650251dc-fc27-496c-a192-a0ccc43204e4" />

<br /><br />

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
<ol>
<li>Business Critical Outage</li>
<li>Personal Computer Issues</li>
<li>Password Reset</li>
</ol>
<img width="1536" alt="Screenshot 2025-02-17 at 3 06 57 PM" src="https://github.com/user-attachments/assets/cb2fa19d-e594-40fa-8a6a-7b6e81373105" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 07 19 PM" src="https://github.com/user-attachments/assets/3e8f5790-38a6-47af-9c55-ddc286adc183" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 07 54 PM" src="https://github.com/user-attachments/assets/b4acac77-c699-4cf3-b7c7-f9779760ae80" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 08 08 PM" src="https://github.com/user-attachments/assets/8aca9a39-8b87-4923-b355-760f75003d2b" />
<img width="1536" alt="Screenshot 2025-02-17 at 3 08 30 PM" src="https://github.com/user-attachments/assets/32f9abe7-8035-4dde-a2a2-8164f1fc30d6" />


<br />
