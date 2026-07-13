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
- Group Policy Objects (GPOs)
- Command Prompt (CMD)

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

## Setting Up Virtual Machine #2 using Windows 10 Pro

I used the Windows 10 virtual machine to connect to the domain and configured the IP addresses to connect to the domain

<img width="973" height="508" alt="vmware_rkMixlxCAt" src="https://github.com/user-attachments/assets/95c29ad7-9411-4e99-b4e2-d0e17600e614" />

<img width="393" height="448" alt="yes5" src="https://github.com/user-attachments/assets/cea6d775-d8dc-45da-96eb-e16bf4b0233e" />

## Verifying DNS Resolution

Verified that the Windows 10 client could successfully connect to j-li.local domain using nslookup and the ping command

<img width="308" height="149" alt="yes1" src="https://github.com/user-attachments/assets/c2655633-f6c7-4bd7-957f-ccbe220f0847" />

<img width="972" height="508" alt="vmware_DA0cJtNiVx" src="https://github.com/user-attachments/assets/1732d46b-9109-437a-bc89-f1b6f1bb692b" />

## Joining the Domain

Entered adminstrative credentials to authorize the Windows 10 client to join the Active Directory Domain

<img width="451" height="293" alt="yes4" src="https://github.com/user-attachments/assets/42e2620a-5fc8-4541-acb4-8833b00e5440" />

<img width="257" height="147" alt="yes" src="https://github.com/user-attachments/assets/b08a148d-8c69-48a8-900a-f5fb7dfee8ec" />

## Domain User Login

Logging in using a domain user account to confirm GPO functionality

<img width="597" height="585" alt="yes 6" src="https://github.com/user-attachments/assets/c81fa15d-987f-4708-9985-2ecc083d952c" />

## Group Policy Verification

Verified that one of the GPOs (Disabling Control Panel) was successfully applied

<img width="416" height="326" alt="vmware_I2n9q0SRED" src="https://github.com/user-attachments/assets/d908c06c-7286-45cd-9ede-f7467f98d992" />

<img width="551" height="128" alt="yes 7" src="https://github.com/user-attachments/assets/9e6f88d8-ff07-4a08-94da-9322d7b31d7a" />

## Key Takeaways

Created and managed Group Policy Objects (GPOs).

Linked GPOs to Organizational Units (OUs).

Configured user and computer policy settings.

Tested and verified Group Policy deployment on a domain-joined Windows 10 client.

Used Command Prompt utilities to validate domain connectivity and DNS resolution.

Troubleshot and confirmed successful Group Policy application.

## References

This lab was completed while learning from the Group Policy tutorial by East Charmer. The environment was built, configured, documented, and validated independently using VMWorkstation Pro, Windows Server 2022, and Windows 10.
















