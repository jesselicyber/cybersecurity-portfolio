# File Services Home Lab

## Overview 

Built a Windows Server 2022 File Services home lab using VMware Workstation Pro to demonstrate enterprise file sharing, network drive mapping, and storage management in an Active Directory environment. This project focuses on configuring shared folders, NTFS and share permissions, Group Policy drive mapping, storage quotas, and file screening using File Server Resource Manager (FSRM).

---

## Tools Used

- Windows Server 2022
- Windows 10 Pro
- VMware Workstation Pro
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)
- File Server Resource Manager (FSRM)
- Command Prompt (CMD)

---

## Lab Overview

Created a dedicated shared folder on Windows Server 2022 that will be used to host files for network users

<img width="783" height="588" alt="vmware_bgtIslrg3a" src="https://github.com/user-attachments/assets/69c87794-3490-4ece-95b5-705c3013cd55" />

## Configure Share Permissions

Granted the Domain Users access to the shared folder allowing authentication

<img width="357" height="445" alt="vmware_LdpY3d1OIJ" src="https://github.com/user-attachments/assets/756ff0ee-dab4-4a1e-99e8-6942fb9d5188" />

<img width="452" height="244" alt="vmware_amDZjnQRWv" src="https://github.com/user-attachments/assets/5c4cddd6-03f1-4dcf-ae7d-604ab4e4d2e0" />

## Mapping the Network Drive on Windows 10 

Switched to the Windows 10 Virtual Machine and mapped the network drive

<img width="784" height="591" alt="vmware_T0MehHBcqs" src="https://github.com/user-attachments/assets/c5c5a8df-f705-481f-a3cf-424b42f00a10" />


<img width="610" height="448" alt="vmware_6cToyNuA2b" src="https://github.com/user-attachments/assets/1bb97c16-3abe-4ca3-a621-26404c5238e2" />

## Configure Drive Mapping with Group Policy

Created a GPO in group policy to allow drive mapping

<img width="980" height="577" alt="vmware_KByzRjDazz" src="https://github.com/user-attachments/assets/00c2d00f-d680-4039-a9b0-50d618d2a1d0" />

<img width="395" height="450" alt="vmware_Yi43L0jnTB" src="https://github.com/user-attachments/assets/ba14d8fb-5f78-4588-8b10-937248b37e37" />

## Apply Group Policy

Ran the gpupdate /force command to immediately apply the latest Group Policy settings to the client

<img width="425" height="174" alt="vmware_spHG4hh0hq" src="https://github.com/user-attachments/assets/3ee504dd-9247-45ff-aba8-e31908b75b73" />

## Verify Network Drive 

Verified that the S: network drive was successfully deployed

<img width="164" height="79" alt="vmware_X6MwqTy6wy" src="https://github.com/user-attachments/assets/4adf6a0c-9bdd-4a8b-89ed-7a4ccdbaac73" />

## Install File Server Resource Manager

Installed the File Server Resource Manager (FSRM) feature to enable storage quotas, file screening, and centralized file management

<img width="412" height="432" alt="vmware_nGRkIVSelY" src="https://github.com/user-attachments/assets/8a7b943b-4478-44fe-9c50-5b6ee2c45404" />

## Configure Storage Quota

Configured a 100 MB hard quota on the shared folder to limit storage usage

<img width="398" height="486" alt="vmware_PebIPxP7wj" src="https://github.com/user-attachments/assets/48729272-7373-4b59-9a80-f3bf15e8c5c8" />

## Configure File Screening

Created a custom file screen to block selected file types, helping enforce organizational storage and security policies

<img width="395" height="455" alt="vmware_MUMyyOqrTd" src="https://github.com/user-attachments/assets/cb65f8e4-cdd5-4595-9325-c16feb4c0190" />

## Verify File Screening 

Verified that the file screen was successfully applied and actively protecting the shared folder

<img width="1021" height="275" alt="vmware_0E1fIl8cGI" src="https://github.com/user-attachments/assets/8b682dce-5d18-425c-b361-ac65a98f683e" />

## Key Takeaways
- Configured SMB file sharing with NTFS and share permissions.
- Assigned access to domain users using Active Directory security groups.
- Mapped shared network drives using Group Policy Preferences.
- Implemented storage quotas with File Server Resource Manager (FSRM).
- Configured file screening policies to restrict unwanted file types.
- Verified Group Policy deployment and network drive accessibility.

## References

This lab was completed while learning from the File Services tutorial by East Charmer. The environment was built, configured, documented, and validated independently using VMware Workstation Pro, Windows Server 2022, and Windows 10.











