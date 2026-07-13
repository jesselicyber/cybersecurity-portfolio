# Group Policy Management Home Lab

## Overview

Built a Windows Server 2022 Group Policy Management home lab using VMWorkstation Pro to demonstrate centralized administration in an Active Directory environment. This project focuses on creating, configuring, linking, and testing Group Policy Objects (GPOs) to enforce security policies and user settings across domain-joined Windows 10 clients.

---

## Technologies Used

- Windows Server 2022
- Windows 10 Pro
- VMWorkstation Pro
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)
- DNS
- PowerShell
- Group Policy Objects (GPOs)

---

## Lab Overview

## Virtual Environment

Installed Group Policy Management on Windows Server 2022

<img width="778" height="552" alt="vmware_FhqCDR28D6" src="https://github.com/user-attachments/assets/b88523c6-97a2-46dc-b51f-a0f089d63729" />

## Adding new GPOs

Added new GPOs - Desktop Wallpaper, Disable USB Devices, Drive Mapping, Password Policy, and Restrict Control Panel

<img width="981" height="579" alt="vmware_1RwMiGxZnw" src="https://github.com/user-attachments/assets/ff46cf2c-b0e9-4a0d-92b3-f952b98e1c23" />

## Configuring the GPOs

Configured settings on multiple GPOs that I created

<img width="682" height="633" alt="vmware_Txp1uzOBib" src="https://github.com/user-attachments/assets/7a32ee50-5e1e-4b25-b5f3-724e25320c6b" />

<img width="897" height="557" alt="vmware_shHQlzGmvI" src="https://github.com/user-attachments/assets/0d4f97a3-0ea8-4d5d-9bd0-d93e8d19bc0b" />

<img width="782" height="558" alt="vmware_9VkTNuh8gm" src="https://github.com/user-attachments/assets/412aaaa8-9c5a-4e9a-9f94-c1db91b0451a" />

## Linking GPOs to Organization Units (OU)

Created Organization Units so I could link the policies I created to groups

<img width="1024" height="768" alt="vmware_6tLkjDgVSO" src="https://github.com/user-attachments/assets/9510af43-850f-43d2-b31e-3cb50a35f68b" />

## Setting up the other Virtual Machine using Windows 10 Pro

I used the Windows 10 virtual machine to connect to the domain and configured the IP addresses to connect to the domain

<img width="973" height="505" alt="yes3" src="https://github.com/user-attachments/assets/ed50ac89-281e-454f-b4f2-33f2f70cd8c4" />

<img width="393" height="448" alt="yes5" src="https://github.com/user-attachments/assets/cea6d775-d8dc-45da-96eb-e16bf4b0233e" />












