# Active Directory Home Lab

## Overview

Built a Windows Server 2022 Active Directory home lab using Oracle VirtualBox. This project demonstrates the deployment of Active Directory Domain Services (AD DS), DNS, DHCP, NAT, PowerShell automation, and domain-joined Windows 10 clients within a virtual enterprise environment.

## Technologies Used

- Windows Server 2022
- Windows 10
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Routing and Remote Access (NAT)
- PowerShell
- Oracle VirtualBox

## Lab Overview

### Virtual Environment

Created a virtual lab environment consisting of a Windows Server 2022 Domain Controller and a Windows 10 client machine using Oracle VirtualBox.

<img width="962" height="618" alt="VirtualBox_tsMaVAOKup" src="https://github.com/user-attachments/assets/1878be23-5b62-438b-bb19-957278cecd83" />

## Step 1 – Configure the Domain Controller

Assigned a static IP address to the internal server before installing Active Directory to ensure reliable DNS and domain services.

<img width="393" height="446" alt="VirtualBoxVM_86WdGrf7CS" src="https://github.com/user-attachments/assets/182e4599-e9f3-46f6-a0fd-806e3a5bcb0c" />

## Create a New Active Directory Forest

Installed Active Directory Domain Services (AD DS) and promoted the server to a Domain Controller by creating the mydomain.com forest.

<img width="756" height="552" alt="VirtualBoxVM_4k0McOjIy1" src="https://github.com/user-attachments/assets/6cb982aa-387e-4a5e-9193-59c98b20d913" />

## Step 2 – Organize Active Directory

Created Organizational Units (OUs) to separate administrative accounts from standard users.

<img width="431" height="370" alt="VirtualBoxVM_4J8tgVWcwt" src="https://github.com/user-attachments/assets/28096648-8092-4d2d-b77f-681bc7e93a9f" />

## Create an Administrator Account

Created an administrator account inside the ADMINS Organizational Unit for domain administration.

<img width="429" height="370" alt="VirtualBoxVM_MgfuyEtl6k" src="https://github.com/user-attachments/assets/be58148d-59e1-4585-8414-9dea7bf4c9de" />

## Step 3 – Automate User Creation

Used a PowerShell script to automatically generate hundreds of Active Directory user accounts from a text file instead of creating each account manually.

<img width="649" height="235" alt="VirtualBoxVM_BljGRVDkIk" src="https://github.com/user-attachments/assets/140d95b9-322b-4f71-9991-d1972eb0f79b" />

## Verify User Creation

Confirmed that the PowerShell script successfully created hundreds of user accounts inside the _USERS Organizational Unit.

<img width="747" height="525" alt="VirtualBoxVM_BGybGLw2rK" src="https://github.com/user-attachments/assets/f79376c3-aca6-493a-9f89-37d4e82d818a" />

## Step 4 – Configure Network Services

Configured Routing and Remote Access to provide Internet connectivity to internal domain clients through Network Address Translation (NAT).

<img width="666" height="400" alt="VirtualBoxVM_Y4lXDmxc0B" src="https://github.com/user-attachments/assets/395f7e5c-1a84-45ae-b063-354cb6418fa3" />

## Verify Network Adapters 

Configured separate Internal and Internet network adapters for routing between the internal lab network and the Internet.

<img width="777" height="587" alt="VirtualBoxVM_leK8XqRNMY" src="https://github.com/user-attachments/assets/4b0d2dd5-4214-4a6f-a11e-5d1bd14bc01c" />

## Configure DHCP

Created a DHCP scope and verified that the Windows 10 client successfully received an IP address lease.

<img width="666" height="400" alt="VirtualBoxVM_Y4lXDmxc0B" src="https://github.com/user-attachments/assets/66bc978b-436d-4375-b392-a2946f989b9d" />

## Step 5 – Join the Client to the Domain

Joined the Windows 10 workstation to the mydomain.com domain.

<img width="317" height="385" alt="VirtualBoxVM_75Osfb5ZBt" src="https://github.com/user-attachments/assets/e325f031-28c4-4ab0-887f-d8bf24da521c" />

## Verify Successful Domain Join

Confirmed the client successfully joined the Active Directory domain.

<img width="297" height="147" alt="VirtualBoxVM_2qiWfQeeaa" src="https://github.com/user-attachments/assets/3ab343c8-a99f-42d1-bf47-0f68524c7f21" />

## Domain Login

Logged into the Windows 10 client using domain credentials.

<img width="1013" height="764" alt="explorer_EX291cVjUN" src="https://github.com/user-attachments/assets/4701125d-51d3-40cd-84ad-d35d6e6c61bd" />










