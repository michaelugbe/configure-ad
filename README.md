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

### Step 6: Connect to the dc-1 VM via remote desktop
<p align="center">
<img src="https://i.imgur.com/1pO99wk.png" height="80%" width="80%"/>
</p>
Connect to the dc-1 VM via remote desktop.

---

### Step 7: Install Active Directory Domain Services
<p align="center">
<img src="https://i.imgur.com/nt5FDYo.png" height="80%" width="80%"/>
</p>
Install Active Directory Domain Services.

---

### Step 8: Create organizational units called _EMPLOYEES and _ADMINS
<p align="center">
<img src="https://i.imgur.com/2WIg6ei.png" height="80%" width="80%"/>
</p>
Create organizational units called _EMPLOYEES and _ADMINS.

---

### Step 9: Create a domain admin user within the domain
<p align="center">
<img src="https://i.imgur.com/FjQ4FP0.png" height="80%" width="80%"/>
</p>
Create a domain admin user within the domain.

---

### Step 10: Log in ro client-1 as the original local admin and join it to the domain, then login to the domain controller and verify that client-1 shows up in the ADUC
<p align="center">
<img src="https://i.imgur.com/kIdvoB6.png" height="80%" width="80%"/>
</p>
Log in ro client-1 as the original local admin and join it to the domain, then login to the domain controller and verify that client-1 shows up in the ADUC.

---

### Step 11: Log into the domain controller as the previously created amine (jane) and run powershell script to create 10000 users
<p align="center">
<img src="https://i.imgur.com/97nvXuz.png" height="80%" width="80%"/>
</p>
Log into the domain controller as the previously created amine (jane) and run powershell script to create 10000 users.

---

### Step 12: Configure account lockout threshold in group policy and attempt to login to script created account with the wrong credentials until locked out
<p align="center">
<img src="https://i.imgur.com/Clzb28q.png" height="80%" width="80%"/>
</p>
Configure account lockout threshold in group policy and attempt to login to script created account with the wrong credentials until locked out.

---

### Step 13: Unlock the account used, reset the password and login using correct credentials
<p align="center">
<img src="https://i.imgur.com/IAFDs8m.png" height="80%" width="80%"/>
</p>
Unlock the account used, reset the password and login using correct credentials.

---

### Step 14: Observe the logs on the Domain Controller
<p align="center">
<img src="https://i.imgur.com/8AiyZs0.png" height="80%" width="80%"/>
</p>
Observe the logs on the Domain Controller.

---

