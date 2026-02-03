<p align="center">
  <img width="700" height="200" alt="image" src="https://github.com/user-attachments/assets/daa445be-b28b-4116-8795-886f90dbb7ea" />
</p>

# osTicket: Postinstallation Configuration

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
3. Select the **Agent** tab then select **Roles**
4. Then **Add a new role**

<p align="center">
  <img width="982" height="550" alt="Capture2" src="https://github.com/user-attachments/assets/7fbde273-a758-429d-b770-6aed5e4f0947" />
</p>

4. Create a **Supreme Admin** and grant all **Permissions** and create role

<p align="center">
  <img width="984" height="566" alt="Capture3" src="https://github.com/user-attachments/assets/f3f61b50-21ba-4935-9a95-bd24d3b77dcc" />
</p>

5. Select **Departments** then **Add a New Department**
6. Create a **SysAdmins** department

<p align="center">
  <img width="978" height="507" alt="Capture5" src="https://github.com/user-attachments/assets/89e7b323-c4ce-43f4-b3e5-97c0eca4f4ea" />
</p>

7. Select **Teams** then **Add a New Team**
8. Create an **Online Banking** team

<p align="center">
  <img width="977" height="447" alt="Capture6" src="https://github.com/user-attachments/assets/c304ae6c-5af3-46d2-a5da-9375b0d5fbdf" />
</p>

---

### 2) Create Agents

1. Select **Settings** then **Users** and check the box labeled **Require registration and login to create tickets**

<p align="center">
  <img width="991" height="813" alt="Capture7" src="https://github.com/user-attachments/assets/796d7f90-a5c1-42e6-a187-99a61e1f5a57" />
</p>

2. Select **Agents** then **Add a New Agent**
3. Create two Agents: named **Jane** and **John**
   - **Jane**
       - **Role:** Supreme Admin
       - **Department:** SysAdmins
       - **Team:** Online Banking

    - **John**
        - **Role:** View Only
        - **Department:** Support
        - **Team:** Leave Blank
     
<p align="center">
  <img width="980" height="516" alt="Capture9" src="https://github.com/user-attachments/assets/0ef4bb90-32d1-44ba-9529-2cb4bcf63972" />
</p>

---

### 3) Create a User

1. Select the **Agent Panel** then select **Users** then **Add User**
2. Name the user **Karen** and fill out necessary information

<p align="center">
  <img width="976" height="462" alt="Capture10" src="https://github.com/user-attachments/assets/6ec076c1-5563-4227-bfce-79b4ea0e2bc1" />
</p>

---

### 4) Configure SLAs and Help Topics

1. Go back to the **Admin Panel** select **Manage** then **SLA**
2. **Add a New SLA** and create 3 SLAs:
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
  <img width="975" height="535" alt="Capture11" src="https://github.com/user-attachments/assets/86d43eb9-61ba-4039-bf92-569626ffcbaa" />
</p>

3. Select **Help Topics** and **Add a New Help Topic**
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
  <img width="975" height="758" alt="Capture12" src="https://github.com/user-attachments/assets/66ccd603-9909-4e50-9a96-0598ca7ca153" />
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
