## What is the Windows Registry?

The best way to describe the Windows Registry would be a configuration database for a Windows computer, its respective users, and application. It is in a nutshell a central repository for retrieving information related to the system or the software on it.

## Basic Architecture of the Windows Registry

The 5 main hives of the Windows Registry include the following

 HKEY_CLASSES_ROOT: Contains file association and COM component information, determining how file types are handled and which applications are associated with them.
 HKEY_CURRENT_USER: Stores configuration settings specific to the currently logged-on user, such as preferences, desktop settings, and application configurations.
 HKEY_LOCAL_MACHINE: Holds system-wide configuration settings for all users on the computer, including hardware, software, operating system, and driver information.
 HKEY_USERS: Consists of subkeys for each user profile, storing user-specific settings and preferences for individual accounts.
 HKEY_CURRENT_CONFIG: Contains hardware and software configuration data related to the current hardware profile, providing information on devices, drivers, and system settings.

## How Active Directory Impacts the Windows Registry

Active Directory GPOs tend to apply to only 2 of the 5 hives. HKEY_LOCAL_MACHINE and HKEY_CURRENT_USER. LOCAL_MACHINE keys are the configuration files that apply to anyone on a given endpoint since its a configuration for the machine in particular. CURRENT_USER keys are the configuration files that apply to that specific user and not the endpoint.

## Example 

![REGISTRY-EXAMPLE.PNG](/REGISTRY-EXAMPLE.PNG)



