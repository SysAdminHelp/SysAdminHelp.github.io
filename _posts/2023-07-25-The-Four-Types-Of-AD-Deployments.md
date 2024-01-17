---
title: The Four Types Of AD Deployments
---

## AD Deployment Types
In a corporate environment, professionals may or may not be assigned the responsibility of implementing an Active Directory solution. Active Directory provides four primary deployment types, each with distinct purposes, but it's essential to recognize that these deployments synergistically complement one another.

## On Premises Active Directory
This is a bread and butter deployment. Often times deployed from Hyper-V servers or running on a physical server, Active Directory-Directory Services deals with device management, directory management(Directory Services), authentication and authorization for the networks people are on. AD relies on policies, trusts, catalogs, and other mechanisms to be inerlopable with other devices and even other domain controllers. This is primarily more or less an on premise all in one soluton. This is actually ideal for almost any organization

## Cloud Active Directory (Azure AD)
Azure AD is a cloud access management service, and only actually covers a fraction of on premises Active Directory capabilities. Azure AD deployments without the presence of AD-DS is best for mostly flat hierarchies with a small business with maybe a handful of equal stakeholders. The reason is because unlike AD DS, Azure AD is actually more flat in hierarchy. There are no hierarchial organizational units and each tenant is independent - meaning that there are no AD-DS style trusts to deploy. Permissions mostly deal with different scopes of an application or services as a result. 

## Hybrid Active Directory (Azure AD + AD-DS)
This deployment is actually not only most optimal but incredibly common. This is because Azure AD tenants are part of not only Office 365 but Office Suite. Office Suite can come with Exchange Online, and in turn Exchange Admin Center, O365 Admin Center, and an Azure Active Directory tenant. A good example of a hybrid use case is using Azure AD for MFA to get into Outlook and using Active Directory-Directory Services for on premises device management (such as setting a default browser). Hybrid basically gives you the best of both worlds, but it is the most costly.

## Active Directory Federated Services
Active Directory Federated Services is never actually deployed in solo but is part of orchestrating Single Sign On against not only local devices but basically throughout different layers of the Microsoft Stack. This like AD-DS is a Windows Server solution and this is a compliment to everything else we discussed more than its own deployment. This is because this deals basically exclusively with Identity Access Management. 
