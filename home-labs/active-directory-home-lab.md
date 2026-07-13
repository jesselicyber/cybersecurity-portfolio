# Active Directory Home Lab

## Overview

Built a Windows Server 2022 Active Directory home lab using Oracle VirtualBox. This project demonstrates the deployment of Active Directory Domain Services (AD DS), DNS, DHCP, NAT, PowerShell automation, and domain-joined Windows 10 clients within a virtual enterprise environment.

## Tools Used

- Windows Server 2022
- Windows 10 Pro
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Routing and Remote Access (NAT)
- PowerShell
- Oracle VirtualBox

## Lab Overview

Created a virtual lab environment consisting of a Windows Server 2022 Domain Controller and a Windows 10 client machine using Oracle VirtualBox.

<img width="954" height="611" alt="VirtualBox_kIlKOB68Sm" src="https://github.com/user-attachments/assets/19784c82-a8e9-476f-97c7-ee3c04374a2e" />

## Configure the Domain Controller

Assigned a static IP address to the internal server before installing Active Directory to ensure reliable DNS and domain services.

<img width="393" height="446" alt="VirtualBoxVM_86WdGrf7CS" src="https://github.com/user-attachments/assets/182e4599-e9f3-46f6-a0fd-806e3a5bcb0c" />

## Create a New Active Directory Forest

Installed Active Directory Domain Services (AD DS) and promoted the server to a Domain Controller by creating the mydomain.com forest.

<img width="756" height="552" alt="VirtualBoxVM_4k0McOjIy1" src="https://github.com/user-attachments/assets/6cb982aa-387e-4a5e-9193-59c98b20d913" />

## Organize Active Directory

Created Organizational Units (OUs) to separate administrative accounts from standard users.

<img width="431" height="370" alt="VirtualBoxVM_4J8tgVWcwt" src="https://github.com/user-attachments/assets/28096648-8092-4d2d-b77f-681bc7e93a9f" />

## Create an Administrator Account

Created an administrator account inside the ADMINS Organizational Unit for domain administration.

<img width="429" height="370" alt="VirtualBoxVM_MgfuyEtl6k" src="https://github.com/user-attachments/assets/be58148d-59e1-4585-8414-9dea7bf4c9de" />

## Automate User Creation

Used a PowerShell script to automatically generate hundreds of Active Directory user accounts from a text file instead of creating each account manually.

<img width="903" height="624" alt="VirtualBoxVM_nsd6gTh2au" src="https://github.com/user-attachments/assets/d3f46b34-a197-435a-9f5c-5133dfa5a43c" />

## Execute the PowerShell Script

Executed the PowerShell script to automatically create hundreds of user accounts within the Active Directory domain. The console output confirms successful account creation for each user.

<img width="649" height="235" alt="VirtualBoxVM_BljGRVDkIk" src="https://github.com/user-attachments/assets/140d95b9-322b-4f71-9991-d1972eb0f79b" />

## Verify User Creation

Confirmed that the PowerShell script successfully created hundreds of user accounts inside the _USERS Organizational Unit.

<img width="750" height="525" alt="VirtualBoxVM_mFPVKq41Tc" src="https://github.com/user-attachments/assets/16ee8180-82a4-434d-bfaa-35f3c44467bf" />

## Configure Network Services

Configured Routing and Remote Access to provide Internet connectivity to internal domain clients through Network Address Translation (NAT).

<img width="494" height="417" alt="VirtualBoxVM_JmGpRWsHx9" src="https://github.com/user-attachments/assets/ce5ad998-9fc8-420d-b829-1bd1989c4aaa" />

## Verify Network Adapters 

Configured separate Internal and Internet network adapters for routing between the internal lab network and the Internet.

<img width="777" height="587" alt="VirtualBoxVM_leK8XqRNMY" src="https://github.com/user-attachments/assets/4b0d2dd5-4214-4a6f-a11e-5d1bd14bc01c" />

## Configure DHCP

Created a DHCP scope and verified that the Windows 10 client successfully received an IP address lease.

<img width="666" height="400" alt="VirtualBoxVM_Y4lXDmxc0B" src="https://github.com/user-attachments/assets/66bc978b-436d-4375-b392-a2946f989b9d" />

## Join the Client to the Domain

Joined the Windows 10 workstation to the mydomain.com domain.

<img width="317" height="385" alt="VirtualBoxVM_75Osfb5ZBt" src="https://github.com/user-attachments/assets/e325f031-28c4-4ab0-887f-d8bf24da521c" />

## Verify Successful Domain Join

Confirmed the client successfully joined the Active Directory domain.

<img width="297" height="147" alt="VirtualBoxVM_2qiWfQeeaa" src="https://github.com/user-attachments/assets/3ab343c8-a99f-42d1-bf47-0f68524c7f21" />

## Domain Login

Logged into the Windows 10 client using domain credentials.

<img width="1013" height="764" alt="explorer_EX291cVjUN" src="https://github.com/user-attachments/assets/4701125d-51d3-40cd-84ad-d35d6e6c61bd" />

## Verify Configuration

Verified that the client received a DHCP address, DNS server, gateway, and DNS suffix from the Domain Controller.

<img width="974" height="508" alt="VirtualBoxVM_wbXJbliRZD" src="https://github.com/user-attachments/assets/78a280b9-d298-414d-835c-b4be05a3a712" />

## Verify DNS Resolution

Verified successful DNS resolution and connectivity between the client and the Domain Controller using ping and nslookup.

<img width="540" height="343" alt="VirtualBoxVM_s66daU0ZOB" src="https://github.com/user-attachments/assets/0f2de10d-553d-4d7c-9a4d-4ed06d3a5243" />

## Key Takeaways

Through this project, I learned how to:

- Deploy and configure a Windows Server 2022 Domain Controller.
- Create and manage an Active Directory forest, Organizational Units (OUs), and user accounts.
- Configure DNS, DHCP, and NAT to provide network connectivity for domain clients.
- Automate bulk user creation using PowerShell scripting.
- Join Windows 10 clients to an Active Directory domain and verify authentication.
- Troubleshoot common networking and domain-join issues using tools such as `ipconfig`, `ping`, and `nslookup`.
- Document and validate each stage of an enterprise Active Directory deployment.

## References

This lab was inspired by and built while learning from Josh Madakor's Active Directory Home Lab tutorial, with additional troubleshooting, documentation, and configuration completed independently.










