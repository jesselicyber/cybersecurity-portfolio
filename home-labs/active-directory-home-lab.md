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

Virtual Environment Setup

Configured a virtual environment using VirtualBox with a Windows Server 2019 Domain Controller (DC) and Windows 10 client machine.


<img width="1899" height="975" alt="DC and CLIENT1" src="https://github.com/user-attachments/assets/2cfdfd3d-d39a-4aeb-a73e-9ac1b628b5b9" />

---

## 2. Active Directory Domain Creation

Created a new Active Directory forest and configured a custom domain (`mydomain.com`) using Active Directory Domain Services.

<img width="752" height="552" alt="Domain Creation" src="https://github.com/user-attachments/assets/bfb4687a-e06a-41aa-bf86-371e7426a220" />


---

## 3. Internal Network Configuration

Configured static IP addressing and DNS settings to allow communication between the Domain Controller and client systems.

<img width="1906" height="928" alt="Internal Network Static IP" src="https://github.com/user-attachments/assets/b136e903-0aed-44b8-a329-effb3b738878" />

---

## 4. NAT & Internet Connectivity

Configured NAT and routing so client systems could access the internet while remaining connected to the internal Active Directory environment.

<img width="494" height="414" alt="Routing NAT interface" src="https://github.com/user-attachments/assets/74b47ee9-3af6-4379-b5f0-764c3a033f8b" />


---

## 5. DHCP Configuration

Configured DHCP services and verified that the Windows client machine successfully received an IP address lease from the Domain Controller.

<img width="1187" height="730" alt="DHCP Lease Success" src="https://github.com/user-attachments/assets/5e029f72-b917-4387-9f44-c400a7fc191e" />

---

## 6. PowerShell User Automation

Used a PowerShell script to bulk-create multiple Active Directory users automatically instead of manually creating accounts.

<img width="806" height="308" alt="PowerShell Bulk User Script" src="https://github.com/user-attachments/assets/c97a87a7-c6b1-4a04-a2aa-f631e4107503" />

---

## 7. Active Directory User Management

Verified successful creation of user accounts and Organizational Units (OUs) inside Active Directory Users and Computers.

<img width="745" height="522" alt="AD Users and Computers" src="https://github.com/user-attachments/assets/48b88c4d-dce4-44a2-839e-2e93b382f62d" />

---

## 8. Domain Join Success

Successfully joined the Windows 10 client machine to the Active Directory domain.

<img width="799" height="630" alt="Domain Join Success Popup" src="https://github.com/user-attachments/assets/97d26800-4d68-4646-a908-6e303bb18f7b" />

---

## 9. Domain Authentication

Verified domain functionality by logging into the Windows client machine using domain credentials.

<img width="1024" height="768" alt="MYDOMAIN Login screen" src="https://github.com/user-attachments/assets/fe72828b-e1d4-4da1-a9d1-6869b1616828" />

---

## What I Learned

This lab helped me better understand how Active Directory environments function in enterprise IT settings. I gained hands-on experience configuring Windows Server services, managing users and domains, troubleshooting networking issues, and using PowerShell automation to improve efficiency.
