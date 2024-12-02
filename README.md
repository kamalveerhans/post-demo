<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">Post-Installation Configuration for osTicket</h1>

This walkthrough showcases the setup and configuration of the **osTicket** ticketing system to meet IT support needs. It involves setting up agents, roles, departments, Service Level Agreements (SLAs), and help topics. These configurations ensure a fully operational and efficient ticketing system.

---

## **Environments and Technologies Used**

- **Microsoft Azure**: Cloud platform for hosting the virtual environment.
- **Remote Desktop Protocol (RDP)**: To access and manage the virtual machine.
- **osTicket**: Open-source ticketing system.
- **Windows 10**: Operating System for the virtual machine.

---

## **Project Overview**

### **Step 1: Configure Roles**
1. Navigate to `Agents > Roles` and create a new role called **Supereme Admin**.
2. In the "Permissions" tab, assign full permissions for "Tickets," "Tasks," and "Knowledge Base."
<img src="https://imgur.com/i2WYtCF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 2: Set Up Departments**
1. Go to `Agents > Departments` and create a new department named **SysAdmin**.
2. This will be used to group agents responsible for system administration tasks.
<img src="https://imgur.com/LqMRESE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 3: Create Teams**
1. Navigate to `Agents > Teams` and create a team named **Level I Support**.
2. Assign specific agents to this team for handling escalated tickets.
<img src="https://imgur.com/fn2Oc93.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 4: Configure Ticket Settings**
1. Navigate to `Settings > Authentication Settings`.
2. Ensure the "Require Registration and Login to Create Tickets" option is **unchecked** to allow anyone to submit a ticket.
![Screenshot 2024-09-27 143959](https://github.com/user-attachments/assets/2e313b6a-86f4-4cde-8c6c-2158b2323f9e)
---

### **Step 5: Add Agents**
1. Go to `Agents > Agents` and add a new agent.
2. Assign the agent to the **SysAdmin** department with the **Super Admin** role.
3. Repeat this process for other agents, assigning them to different roles and departments as needed.
<img src="https://imgur.com/jOSTRHG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/uN5eugl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 6: Create Users**
1. Navigate to `Agent Panel > Users > Add Users`.
2. Add two users (Karen & Ken) who will submit tickets through the system.
<img src="https://imgur.com/zml8BLf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 7: Configure SLAs**
1. Go to `Admin Panel > Manage > SLA`.
2. Create three SLA plans:
   - **Critical**: 1-hour response time.
   - **High**: 4-hour response time.
   - **Normal**: 8-hour response time.
3. Assign these SLA plans to relevant departments or help topics.
<img src="https://imgur.com/Cd7L3lt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

### **Step 8: Add Help Topics**
1. Navigate to `Admin Panel > Manage > Help Topics`.
2. Create the following topics:
   - **Business Critical Outage**
   - **Personal Computer Issues**
   - **Equipment Request**
   - **Password Reset**
<img src="https://imgur.com/9pXcS4f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
---

## **Key Takeaways**
This project highlights:
- The importance of structured roles and permissions.
- How SLAs streamline ticket prioritization.
- Effective categorization using help topics to improve ticket management.
