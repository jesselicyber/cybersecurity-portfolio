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

## Virtual Environment Setup

Configured a virtual environment using VirtualBox with a Windows Server 2019 Domain Controller (DC) and Windows 10 client machine.


<img width="890" height="695" alt="chrome_S0ZoZzfCgP" src="https://github.com/user-attachments/assets/e0457ee6-f374-47f8-8344-f962aac06868" />

## Installing Active Directory

Installed Active Directory on Server Manager

<img width="411" height="430" alt="VirtualBoxVM_4MJco1MPB9" src="https://github.com/user-attachments/assets/61b1d20f-ed45-4948-92b6-6c95928ceea0" />

---

## 2. Domain Controller Deployment

Created a new Active Directory forest and configured a custom domain (`mydomain.com`) using Active Directory Domain Services.

<img width="752" height="552" alt="Domain Creation" src="https://github.com/user-attachments/assets/bfb4687a-e06a-41aa-bf86-371e7426a220" />


---

## 3. Network Configuration

Configured static IP addressing and DNS settings to allow communication between the Domain Controller and client systems.

<img width="389" height="443" alt="chrome_v6hNDkCvqP" src="https://github.com/user-attachments/assets/5f5fb1e9-65d3-48d5-8b39-acd63db1ffd8" />

---

## 4. Network Configuration

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

## 8. Domain Join Verification

Successfully joined the Windows 10 client machine to the Active Directory domain.

<img width="299" height="147" alt="chrome_ILEu0Tf80d" src="https://github.com/user-attachments/assets/46172def-cf14-4a3f-85a0-6437a46075b0" />

---

## 9. Domain Authentication

Verified domain functionality by logging into the Windows client machine using domain credentials.

<img width="1024" height="768" alt="MYDOMAIN Login screen" src="https://github.com/user-attachments/assets/fe72828b-e1d4-4da1-a9d1-6869b1616828" />

---

## What I Learned

• Active Directory relies heavily on DNS.

• DHCP automatically distributed IP addresses
to domain clients.

• PowerShell significantly reduced manual user
creation.

• Domain joins require proper DNS configuration.
