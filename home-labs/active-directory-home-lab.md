# Active Directory Home Lab

## Objective
Built an Active Directory home lab using Windows Server 2019, Windows 10, and VirtualBox to simulate a small enterprise network. Practiced Windows administration, domain services, networking, DHCP, DNS, user management, and PowerShell automation.

## Tools Used
- Windows Server 2019
- Windows 10
- Oracle VirtualBox
- Active Directory Domain Services (AD DS)
- DHCP
- DNS
- PowerShell
- NAT / Routing

## Skills Practiced
- Active Directory installation & configuration
- Domain creation and management
- DHCP configuration
- DNS configuration
- Organizational Units (OUs)
- Domain joining Windows clients
- PowerShell user automation
- Basic networking and troubleshooting
- Windows administration

---

# Lab Walkthrough

## 1. Virtual Lab Environment

Configured a virtual environment using VirtualBox with a Windows Server 2019 Domain Controller (DC) and Windows 10 client machine.

<img width="1899" height="975" alt="DC and CLIENT1" src="https://github.com/user-attachments/assets/2cfdfd3d-d39a-4aeb-a73e-9ac1b628b5b9" />

---

## 2. Active Directory Domain Creation

Created a new Active Directory forest and configured a custom domain (`mydomain.com`) using Active Directory Domain Services.

**Use this screenshot:**  
✅ **Add New Forest → mydomain.com**

(Add screenshot here)

---

## 3. Internal Network Configuration

Configured static IP addressing and DNS settings to allow communication between the Domain Controller and client systems.

**Use this screenshot:**  
✅ **172.16.0.1 static IP + DNS settings**

(Add screenshot here)

---

## 4. NAT & Internet Connectivity

Configured NAT and routing so client systems could access the internet while remaining connected to the internal Active Directory environment.

**Use this screenshot:**  
✅ **Routing & NAT interface (INTERNET selected)**

(Add screenshot here)

---

## 5. DHCP Configuration

Configured DHCP services and verified that the Windows client machine successfully received an IP address lease from the Domain Controller.

**Use this screenshot:**  
✅ **DHCP Lease Success (`172.16.0.100`)**

(Add screenshot here)

---

## 6. PowerShell User Automation

Used a PowerShell script to bulk-create multiple Active Directory users automatically instead of manually creating accounts.

**Use this screenshot:**  
✅ **PowerShell “Creating user:” screen**

(Add screenshot here)

---

## 7. Active Directory User Management

Verified successful creation of user accounts and Organizational Units (OUs) inside Active Directory Users and Computers.

**Use this screenshot:**  
✅ **AD Users & Computers showing many users**

(Add screenshot here)

---

## 8. Domain Join Success

Successfully joined the Windows 10 client machine to the Active Directory domain.

**Use this screenshot:**  
✅ **“Welcome to the mydomain.com domain” popup**

(Add screenshot here)

---

## 9. Domain Authentication

Verified domain functionality by logging into the Windows client machine using domain credentials.

**Use this screenshot:**  
✅ **MYDOMAIN login screen**

(Add screenshot here)

---

## What I Learned

This lab helped me better understand how Active Directory environments function in enterprise IT settings. I gained hands-on experience configuring Windows Server services, managing users and domains, troubleshooting networking issues, and using PowerShell automation to improve efficiency.
