## Importance of AD Troubleshooting
When rolling out a new GPO at an organization, or perhaps a new implementation of that GPO, you may find policy object or security group conflict. There are several ways of troubleshooting Active Directory policies and employing these troubleshooting methods

## Troubleshooting Vectors

* Powershell:
  * gpoupdate /force can be used to force a group policy to implement in an Active Directory environment
  * gpresult /h can be used to get an audit of the most recent Active Directory policies implemented.
  * Test-ComputerSecureChannel can be used to test the replication between two domain servers
  * Test-Connection -ComputerName $env:USERDNSDOMAIN can be used to test DNS resolution for the domain controllers in question
  * whoami /groups - allows a display of security groups assigned from AD of the user in question 


* Microsoft Management Console
  * rsop.msc - will give an established report of conflicting GPOs
* Windows Registry
  * Primarily HKEY_LOCAL_MACHINE and HKEY_CURRENT_USER hives.

These are just some of the ways of troubleshooting AD. It is best to employ these methods as part of a coherent troubleshooting strategy.
