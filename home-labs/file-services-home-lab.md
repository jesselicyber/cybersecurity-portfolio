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

<img width="452" height="244" alt="vmware_amDZjnQRWv" src="https://github.com/user-attachments/assets/5c4cddd6-03f1-4dcf-ae7d-604ab4e4d2e0" />

<img width="357" height="445" alt="vmware_LdpY3d1OIJ" src="https://github.com/user-attachments/assets/756ff0ee-dab4-4a1e-99e8-6942fb9d5188" />

## Mapping the Network Drive

Switched to the Windows 10 Virtual Machine and mapped the network drive

<img width="610" height="448" alt="vmware_6cToyNuA2b" src="https://github.com/user-attachments/assets/1bb97c16-3abe-4ca3-a621-26404c5238e2" />

## Configure Drive Mapping with Group Policy

Created a GPO in group policy to allow drive mapping

<img width="980" height="577" alt="vmware_KByzRjDazz" src="https://github.com/user-attachments/assets/00c2d00f-d680-4039-a9b0-50d618d2a1d0" />

<img width="395" height="450" alt="vmware_Yi43L0jnTB" src="https://github.com/user-attachments/assets/ba14d8fb-5f78-4588-8b10-937248b37e37" />




