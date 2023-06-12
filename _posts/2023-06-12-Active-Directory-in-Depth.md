## Object types of Group Policies 
There are several objects that are key to nearly any Active Directory-Directory Services enviornment. These include the following:

* User: Represents a person's account.
* Group: Represents a collection of users or other groups.
* Computer: Represents a physical or virtual machine.
* Organizational Unit (OU): Represents a folder for organizing objects.
* Domain: Represents a group of objects with common management (inside the same domain.
* Site: Represents a physical location in the network.
* Schema: Defines the structure of objects in Active Directory.

The hierarchy for how Group Policies work in AD-DS can be described as follows:
* Local GPO: Applied to individual computers, stored locally, and takes precedence over other GPOs.

* Site GPO: Linked to Active Directory sites, applied to all computers within a specific site.

* Domain GPO: Linked to an entire Active Directory domain, applied to all objects within the domain unless overridden.

* OU GPO: Linked to specific Organizational Units (OUs) within a domain, applied to objects within those OUs.

* Active Directory enviornments as mentioned in the prior post can range from small to large in complexity. This especially applies to the domain structure:

## Domain Types
* Single Domain: This is the simplest type of domain structure used in small to medium-sized organizations. Everything, such as users, groups, and computers, is contained within a single domain.

* Tree Domain: A tree domain is a hierarchical structure that connects multiple domains together. They share a common parent-child relationship, with a root domain at the top. This structure allows for centralized management and delegation of administrative tasks.

* Forest Domain: A forest domain consists of one or more domain trees that share a common schema and global catalog. Each tree has its own separate namespace and domain structure. Forest domains are typically used in larger organizations or when multiple independent domains need to be connected.

* Its important to note that the parent-child relationship between domains in question are essential to making Forest and Tree domain configurations properly work. 

Imagine a single domain as a small organization with all its employees, departments, and resources managed under one umbrella. Now, let's see how it can grow and transform into larger structures:

* Single Domain to Tree Domain:
As the organization expands, it may need to organize its resources better. To do this, they can create different sections within the organization called "child domains." Each child domain can represent a department or a branch office, and they are connected to the main domain.
This creates a tree-like structure where the main domain is like the tree trunk, and the child domains are the branches. Each branch/domain can have its own set of users, groups, and resources, making it easier to manage and delegate tasks.

* Tree Domain to Forest Domain:
Sometimes, the organization may grow even larger or acquire other companies. In such cases, they might want to connect multiple tree domains together. This is where a forest domain comes into play.
A forest domain is like a big forest with multiple trees (domain trees) growing within it. Each domain tree can represent a separate organization or a group of related domains. The forest domain allows these domain trees to share a common set of rules, policies, and resources. It provides a way for different organizations or groups to collaborate and work together effectively. The global catalog in a forest domain is a directory that stores summarized information about all the objects in the entire forest. It helps quickly find and access data across different domains and enables smooth communication and resource sharing and serves sort of as like a dictionary involving users, computers etc. 






