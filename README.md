# IT-HomeLab-Cloud-Identity

> Build and manage a modern Microsoft cloud environment with Microsoft Entra ID, Microsoft 365, Hybrid Identity, Microsoft Intune, and cloud services.

---

## Project Overview

This repository is the second part of my IT HomeLab project series.

In the first repository, I built a complete on-premises Windows infrastructure based on Windows Server, Active Directory, DNS, DHCP, Group Policy, File Services, WSUS, and other core Microsoft technologies.

This repository continues that environment by extending it to Microsoft cloud services. The focus is on Microsoft Entra ID, Microsoft 365, Hybrid Identity, Microsoft Intune, Exchange Online, SharePoint Online, and cloud identity management.

Together, both repositories show how a traditional on-premises infrastructure can evolve into a modern hybrid Microsoft environment.

---

## Previous Repository

This project continues the infrastructure built in the previous repository.

| Repository | Description |
|------------|-------------|
| **IT-HomeLab-Windows-Infrastructure** | On-premises Windows infrastructure including Active Directory, DNS, DHCP, Group Policy, File Server, Print Server, WSUS, and Windows Server Backup. |

🔗 **Repository:** https://github.com/ali-turkoglu/IT-HomeLab-Windows-Infrastructure

---

## Objectives

The main goals of this repository are:

- Learn Microsoft Entra ID.
- Manage Microsoft 365 services.
- Build a hybrid identity environment.
- Practice cloud administration.
- Document every phase on GitHub.

---

## Lab Environment

| Component | Value |
|-----------|-------|
| Hypervisor | Proxmox VE |
| Server | Windows Server 2022 |
| Client | Windows 11 |
| On-Premises Domain | homelab.local |
| Cloud Platform | Microsoft 365 Business Premium |
| Cloud Tenant | ithomelab.onmicrosoft.com |
| Identity | Microsoft Entra ID |

---

## Technologies

### Identity
- Microsoft Entra ID
- Hybrid Identity
- Azure AD Connect Cloud Sync

### Microsoft 365
- Microsoft 365
- Exchange Online
- SharePoint Online
- Microsoft Teams
- OneDrive

### Management
- Microsoft Intune
- Microsoft Defender
- Conditional Access
- PowerShell

---

## Architecture

To keep things simple, here is how the different parts of this HomeLab communicate with each other:

- **Local Network (On-Premises):** The foundation is my local Windows Server running Active Directory (`homelab.local`).
- **The Bridge (Hybrid Connection):** I use a tool called Azure AD Connect Cloud Sync. This tool securely connects my local Active Directory to the cloud.
- **Cloud Identity:** Microsoft Entra ID handles the cloud identities. It takes the users from my local server and synchronizes them to the cloud.
- **Cloud Services:** Once the users are in the cloud, they can securely log in and use Microsoft 365 services, such as Exchange Online (email), SharePoint/OneDrive (files), and Microsoft Intune (device management).

---

## Roadmap

| Status | Phase |
|:------:|-------|
| ✅ | [Phase 13 – Cloud Environment Preparation](docs/13-Cloud-Environment-Preparation/README.md) |
| ✅ | [Phase 14 – Microsoft Entra ID Fundamentals](docs/14-Microsoft-Entra-ID-Fundamentals/README.md) |
| ✅ | [Phase 15 – Microsoft Entra ID Security](docs/15-Microsoft-Entra-ID-Security/README.md) |
| ✅ | [Phase 16 – Microsoft Entra ID Connect Cloud Sync](docs/16-Microsoft-Entra-ID-Connect-Cloud-Sync/README.md) |
| ⏸️ | Phase 17 – Microsoft 365 Services (Temporarily On Hold)|
| ✅ | [Phase 18 – Cloud File Services](docs/18–Cloud-File-Services/README.md) |
| 🚧 | Phase 19 – Endpoint Management (Microsoft Intune) |

> **Note**
>
> Phase 17 is temporarily on hold because Exchange Online is not working correctly in my Microsoft 365 tenant.
>
> I opened a support ticket with Microsoft, and the issue is currently being investigated.
>
> I will continue this phase after the Exchange Online problem is resolved.
>
> Until then, I will continue with **Phase 18 – Cloud File Services**.

---

## Timeline

- **29-07-2026** – Phase 13: Cloud Environment Preparation completed.
- **30-07-2026** – Phase 14: Microsoft Entra ID Fundamentals completed.
- **31-07-2026** - Phase 15: Microsoft Entra ID Security completed.
- **03-08-2026** - Phase 16: Microsoft Entra Connect Cloud Sync completed.
- **09-08-2026** - Phase 18 – Cloud File Services completed.
  
---

## Related Repositories


| Repository | Status |
|------------|:------:|
| [IT-HomeLab-Windows-Infrastructure](https://github.com/ali-turkoglu/IT-HomeLab-Windows-Infrastructure) | ✅ Completed |
| IT-HomeLab-Cloud-Identity | 🚧 In Progress |
| IT-HomeLab-Linux-Containers | ⏳ Planned |
| IT-HomeLab-Network-Security | ⏳ Planned |
| IT-HomeLab-Automation-Monitoring | ⏳ Planned |

---

### ➡️ Next Repository *(Planned)*

**IT-HomeLab-Linux-Containers**
The next repository will focus on Ubuntu Server, Docker, Portainer, container management, and Linux administration.

---

## License

This project is licensed under the MIT License. See the LICENSE file for more information.
