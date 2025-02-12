<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

# Deploying Active Directory in Azure
In this project I'll be creating two VMs, one running Windows Server, to act as a domain controller, and the other to act as a client running windows 10 that will be joined to the domain. I will then run AD and run a script that will create users in the domain, which I can log into from the cleint VM, then manage the accounts and update the group policies, all to simulate a real life IT environment. 

---

## Environments and Technologies Used
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

---

## Operating Systems Used
- Windows 10
- Windows Server

---

## Lab Steps

---

### Step 1: Create virtual network and subnet
<p align="center">
<img src="https://i.imgur.com/HNsT9H0.png" height="80%" width="80%"/>
</p>
create virtual network and subnet.

---

### Step 2: Create domain controller VM
<p align="center">
<img src="https://i.imgur.com/LQyR5gC.png" height="80%" width="80%"/>
</p>
Create domain controller VM

---

### Step 3: Create client VM
<p align="center">
<img src="https://i.imgur.com/jjeTLzp.png" height="80%" width="80%"/>
</p>
Create client VM.

---

### Step 4: Set domain controller's NIC private IP address to be static
<p align="center">
<img src="https://i.imgur.com/94LWEih.png" height="80%" width="80%"/>
</p>
Set domain controller's NIC private IP address to be static.

---

### Step 5: Set client-1's DNS settings to DC-1's private IP address
<p align="center">
<img src="https://i.imgur.com/Hd4ydiH.png" height="80%" width="80%"/>
</p>
Set client-1's DNS settings to DC-1's private IP address.

---

### Step 6: Connect to osTicket Database using HeidiSQL
<p align="center">
<img src="https://i.imgur.com/62lWdEx.png" height="80%" width="80%"/>
</p>
Connect to osTicket database using HeidiSQL.

---

### Step 7: Log in to osTicket Using Admin Credentials
<p align="center">
<img src="https://i.imgur.com/gcm0yCT.png" height="80%" width="80%"/>
</p>
Log in to osTicket using admin credentials.

---

### Step 8: Configure Roles (for Grouping Permissions)
<p align="center">
<img src="https://i.imgur.com/ETGqWFe.png" height="80%" width="80%"/>
</p>
Configure roles (for grouping permissions).

---

### Step 9: Configure Departments (for Ticket Visibility)
<p align="center">
<img src="https://i.imgur.com/YBvoed7.png" height="80%" width="80%"/>
</p>
Configure departments (for ticket visibility).

---

### Step 10: Configure Teams (Pull Agents from Different Departments)
<p align="center">
<img src="https://i.imgur.com/TBWCy35.png" height="80%" width="80%"/>
</p>
Configure teams to pull agents from different departments.

---

### Step 11: Configure Helpdesk Agents in osTicket
<p align="center">
<img src="https://i.imgur.com/qmrv3eJ.png" height="80%" width="80%"/>
</p>
Configure helpdesk agents in osTicket.

---

### Step 12: Configure SLA
<p align="center">
<img src="https://i.imgur.com/akG0TDZ.png" height="80%" width="80%"/>
</p>
Configure Service Level Agreements (SLA).

---

### Step 13: Configure Help Topics
<p align="center">
<img src="https://i.imgur.com/1emlWpY.png" height="80%" width="80%"/>
</p>
Configure help topics.

---

### Step 14: Create Ticket as End-User
<p align="center">
<img src="https://i.imgur.com/MVSPCrh.png" height="80%" width="80%"/>
</p>
Create a ticket as an end-user.

---

### Step 15: Work Ticket to Completion as Helpdesk Agent
<p align="center">
<img src="https://i.imgur.com/c6fd56W.png" height="80%" width="80%"/>
</p>
Work ticket to completion as helpdesk agent.
