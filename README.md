<p align="center">
  <img width="700" height="200" alt="image" src="https://github.com/user-attachments/assets/daa445be-b28b-4116-8795-886f90dbb7ea" />
</p>

# osTicket: Post-Installation Configuration

This project focuses on configuring core operational settings within the osTicket ticketing system. I set up roles, departments, and teams to define how support responsibilities are structured. I then created agents and a user to establish the internal and external participants in the ticketing workflow. Finally, I configured SLAs and help topics to standardize response expectations and categorize incoming requests. This project demonstrates essential skills in ticketing system administration, workflow organization, and service desk configuration.

---

## Environments and Technologies Used

- Microsoft Azure
- Azure Virtual Network
- osTicket
- Remote Desktop Protocol (RDP)

---

## Lab Objectives

- Configure roles, departments, and teams within osTicket to establish a structured support workflow  
- Create and assign agents to ensure proper handling and escalation of incoming tickets  
- Add an end user to represent the customer-facing side of the ticketing process  
- Configure Service Level Agreements (SLAs) to define response and resolution expectations  
- Set up help topics to categorize and route incoming support requests effectively  
- Strengthen understanding of ticketing system administration, workflow organization, and service desk configuration within osTicket

---

## Step-by-Step Walkthrough

### Lab Environment

- **Platform:** Microsoft Azure
- **Virtual Machine:** Windows 10 Pro
- **Required osTicket Setup:**
  - [osTicket Prerequisites & Installation](https://github.com/RyanKennon/osTicket-Prerequisites-Installation)

<p align="center">
  <img width="1818" height="592" alt="Untitled Diagram-Page-1 drawio" src="https://github.com/user-attachments/assets/5707ad74-caf1-4f74-8372-162c5ec228a1" />
</p>

---

### 1) Configure Roles, Departments, and Teams

1. Open **osTicket** as an admin in the **Virtual Machine**
   - [Admin/Analyst Login Page](http://localhost/osTicket/scp/login.php)

<p align="center">
  <img width="826" height="619" alt="Capture1" src="https://github.com/user-attachments/assets/30d6c568-cd85-4807-afc6-6fc6572737a5" />
</p>

2. In the **admin** account open the **Admin Panel**
3. Select the **Agent** tab then select **Roles** then **Add New Role**
4. Create a **Supreme Admin** and grant all **Permissions** and create role

<p align="center">
  <img width="984" height="566" alt="Untitled Diagram-Page-2 drawio" src="https://github.com/user-attachments/assets/aa988a99-9d9a-496b-a1ce-e4b6e7bde289" />
</p>

5. Select **Departments** then **Add New Department**
6. Create a **SysAdmins** department and make it a **Top Level Department**
7. Delete the **Maintenance** department

<p align="center">
  <img width="973" height="487" alt="Untitled Diagram-Page-3 drawio" src="https://github.com/user-attachments/assets/11c20f21-2c8f-49ff-8987-bba0772897bd" />
</p>

8. Select **Teams** then **Add New Team**
9. Create an **Online Banking** team

<p align="center">
  <img width="977" height="447" alt="Untitled Diagram-Page-4 drawio" src="https://github.com/user-attachments/assets/22345641-3c05-4a11-9e2e-c616a6635a70" />
</p>

---

### 2) Create Agents

1. Select **Settings** then **Users** and uncheck the box labeled **Require registration and login to create tickets**

<p align="center">
  <img width="976" height="793" alt="Untitled Diagram-Page-5 drawio" src="https://github.com/user-attachments/assets/e41dc03b-b20f-446d-aca1-4e7179374283" />
</p>

2. Select **Agents** then **Add New Agent**
3. Create two Agents: named **Jane** and **John**
   - **Jane**
       - **Role:** Supreme Admin
       - **Department:** SysAdmins
       - **Team:** Online Banking

    - **John**
        - **Role:** All Access
        - **Department:** Support
        - **Team:** Leave Blank
     
<p align="center">
  <img width="980" height="516" alt="Untitled Diagram-Page-6 drawio" src="https://github.com/user-attachments/assets/094133a3-faef-469c-9070-ff137f575fcd" />
</p>

---

### 3) Create a User

1. Select the **Agent Panel** then select **Users** then **Add User**
2. Name the user **Karen** and fill out necessary information

<p align="center">
  <img width="976" height="462" alt="Untitled Diagram-Page-7 drawio" src="https://github.com/user-attachments/assets/dca978fd-7fff-4e8d-93c2-e8ac275f10b2" />
</p>

---

### 4) Configure SLAs and Help Topics

1. Go back to the **Admin Panel** select **Manage** then **SLA**
2. **Add New SLA Plan** and create 3 SLAs:
   - **Sev-A**
     - **Grace Period:** 1 hour
     - **Schedule:** 24/7

    - **Sev-B**
      - **Grace Period:** 4 hours
      - **Schedule:** 24/7
     
    - **Sev-C**
      - **Grace Period:** 8 hours
      - **Schedule:** 24/5
     
<p align="center">
  <img width="975" height="535" alt="Untitled Diagram-Page-8 drawio" src="https://github.com/user-attachments/assets/2c77dbc2-4a5b-487e-b785-8a3acd1a4edb" />
</p>

3. Select **Help Topics** and **Add New Help Topic**
4. Create 5 Help Topics
   - **Business Critical Outage**
     - **Parent Topic:** Report a Problem
    
   - **Personal Computer Issues**
     - **Parent Topic:** Report a Problem
    
   - **Equipment Request**
     - **Parent Topic:** General Inquiry
    
   - **Password Reset**
     - **Parent Topic:** Report a Problem
    
   - **Other**
     - **Parent Topic:** General Inquiry
    
<p align="center">
  <img width="975" height="758" alt="Untitled Diagram-Page-9 drawio" src="https://github.com/user-attachments/assets/4688cd46-ab70-4554-a392-5e9e46a46e5c" />
</p>

---

## Outcome

- Successfully configured roles, departments, and teams to establish a structured support workflow within osTicket  
- Created and assigned agents, enabling proper ticket handling and escalation capabilities  
- Added a user to represent the customer-facing participant in the ticketing system  
- Configured SLAs to define response and resolution time expectations for incoming tickets  
- Set up help topics to organize and categorize support requests effectively  
- Demonstrated a practical understanding of ticketing system configuration, workflow setup, and service desk administration within osTicket

---

## Skills Demonstrated

- Configuring roles, departments, and teams to structure ticket workflows  
- Creating and managing agents responsible for handling and escalating support tickets  
- Adding and managing end users within a ticketing system  
- Setting up SLAs to define response and resolution requirements  
- Creating help topics to categorize and route incoming support requests  
- Understanding and applying service desk administration principles  
- Organizing ticket workflows to support efficient IT support operations  
- Strengthening practical knowledge of ticketing system configuration and workflow design
