---
title: Active Directory Overview
---
## What is Active Directory?


Microsoft Active Directory is a comprehensive suite of technologies that extends beyond a single component and is not solely focused on identity and access management (IAM). At its core, Active Directory revolves around directory services and plays a critical role in mapping network resources to their respective addresses. This means that servers running Active Directory, known as Domain Controllers, function as directory servers.

The primary offering from Microsoft in the realm of Active Directory is Active Directory Domain Services (AD DS), which is an on-premises domain management tool. By organizing devices and users into domains, which can include printers, PCs, and new employees, they become part of the Directory Server's domain, also referred to as the Domain Controller. This integration with the Domain Name System (DNS) allows policies and preferences from AD DS, such as Group Policies/Preferences (GPOs/GPPs), to govern the behavior and settings of these joined entities.

The capabilities of AD DS go beyond identity and access management. They encompass functionalities like password resets, access permission control, endpoint management through Windows Update for Business (WuFB) or Windows Server Update Services (WSUS), as well as onboarding and offboarding processes.

While Active Directory Domain Services is a fundamental component of Microsoft's Active Directory, it is important to note that there are other technologies within the broader suite. Azure Active Directory (Azure AD), for instance, focuses more on providing IAM services and is not designed to replace on-premises AD DS. Azure AD offers cloud-based identity and access management features, including single sign-on, multi-factor authentication, and application provisioning.

In summary, Microsoft Active Directory is a multifaceted suite of technologies centered around directory services, with AD DS serving as the core on-premises domain management tool. While AD DS enables comprehensive control over network resources and entities joined to domains, other components such as Azure AD focus on IAM services in the cloud and are not intended to replace AD DS.

## AD DS Best Practices - Small and Medium Enterprise

When deploying Active Directory Domain Services (AD DS) at the SMB level, it is common to have a single forest and a single domain, especially if the company has only one office. This simplified setup makes management easier as you don't have to deal with child domains or complex hierarchical structures.To ensure high availability and fault tolerance, it is recommended to deploy a second Domain Controller (server) in the environment. Both domain controllers should host DNS (Domain Name System) and DHCP (Dynamic Host Configuration Protocol) services. This setup ensures that if the primary domain controller fails, the secondary domain controller can take over these essential services, allowing business operations to continue without interruption.Active Directory's replication functionality facilitates the synchronization of data between the primary and secondary domain controllers. This replication ensures that changes made on one domain controller are propagated to others, maintaining consistent and up-to-date information across the network. When configuring new users in AD DS, it is crucial to follow the principle of least privilege. This principle emphasizes assigning users the minimum level of access and permissions necessary to perform their job functions. By adhering to this principle, you reduce the risk of unauthorized access or accidental misuse of resources, thus enhancing cybersecurity and minimizing potential vulnerabilities.



---



