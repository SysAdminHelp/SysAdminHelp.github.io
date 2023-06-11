## What is Active Directory?

Contrary to some people's perception, Microsoft Active Directory is not comprised of a single technology and is not neccesarily a dedicated IAM suite. Active Directory centers around directory services and is critical in the mapping of network resources to their respective addresses. In turn this make servers that are AD servers (called Domain Controllers) *directory servers*. AD DS (Active Directory - Directory Services), which is arguably the core AD product offered by microsoft, is an on prem domain management tool. When devices and users are grouped to domains (such as printers, PCs and new employees) they become subject to the DNS as they are now part of the Directory Server's domain (aka Domain Controller) - allowing policies/preferences from AD DS (GPOs/GPPs or Group Policies/Preferences) to control joined entitties. This allows for password resets, access permision capabilities,  endpoint management (with WuFB/WSUS), onboarding/offboarding, etc. There are other technologies such as Azure AD which is moreso dedicated to IAM services and is not a Domain Services platform (meaning it can not replace on prem AD DS).

---



