<p align="center">
  <img width="700" height="200" alt="image" src="https://github.com/user-attachments/assets/daa445be-b28b-4116-8795-886f90dbb7ea" />
</p>

# osTicket: Post-Installation Configuration

## Place Overview Here

---

## Environments and Technologies Used

---

## Lab Objective

---

## Step-by-Step Walkthrough

### Lab Environment

- **Platform:** Microsoft Azure
- **Virtual Machine:** Windows 10 Pro

<p align="center">
  <img width="1818" height="592" alt="Untitled Diagram-Page-1 drawio" src="https://github.com/user-attachments/assets/5707ad74-caf1-4f74-8372-162c5ec228a1" />
</p>

---

#### 1) Configure Roles, Departments, and Teams

1. Open **osTicket** as an admin in the **Virtual Machine**
   - [Admin/Analyst Login Page](http://localhost/osTicket/scp/login.php)

## Capture 1

2. In the **admin** account open the **Admin Panel**
3. Select the **Agent** tab then select **Roles**
4. Then **Add a new role**

## Capture 2

4. Create a **Supreme Admin** and grant all **Permissions** and create role

## Capture 3

5. Select **Departments** then **Add a New Department**

## Capture 4

6. Create a **SysAdmins** department and create department

## Capture 5

7. Select **Teams** then **Add a New Team**

## Capture 6

8. Create an **Online Banking Team**

---

### 2) Create Agents

1. Select **Settings** then **Users** and check the box labeled **Require registration and login to create tickets**

## Capture 7

2. Select **Agents** then **Add a New Department**

## Capture 8

3. Create two Agents: named **Jane** and **John**
   - **Jane**
       - **Role:** Supreme Admin
       - **Department:** SysAdmins
       - **Team:** Online Banking

    - **John**
        - **Role:** View Only
        - **Department:** Support
        - **Team:** Leave Blank
     
## Capture 9

---

### 3) Create a User

1. Select the **Agent Panel** then select **Users** then **Add User**
2. Name the user **Karen** and fill out necessary information

## Capture 10

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
     
## Capture 11

3. Select **Manage** then **Help Topics** and **Add a New Help Topic**
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
    
## Capture 12

---

## Outcome

---

## Skills Demonstrated
