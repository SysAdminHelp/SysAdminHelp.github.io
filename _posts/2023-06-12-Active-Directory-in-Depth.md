## Object types of Group Policies 
There are several objects that are key to nearly any Active Directory-Directory Services enviornment. These include the following:

* User: Represents a person's account.
* Group: Represents a collection of users or other groups.
* Computer: Represents a physical or virtual machine.
* Organizational Unit (OU): Represents a folder for organizing objects.
* Domain: Represents a group of objects with common management (inside the same domain.
* Site: Represents a physical location in the network.
* Schema: Defines the structure of objects in Active Directory.

Active Directory enviornments as mentioned in the prior post can range from small to large in complexity. This especially applies to the domain structure:

* Single Domain: This is the simplest type of domain structure used in small to medium-sized organizations. Everything, such as users, groups, and computers, is contained within a single domain.

* Tree Domain: A tree domain is a hierarchical structure that connects multiple domains together. They share a common parent-child relationship, with a root domain at the top. This structure allows for centralized management and delegation of administrative tasks.

* Forest Domain: A forest domain consists of one or more domain trees that share a common schema and global catalog. Each tree has its own separate namespace and domain structure. Forest domains are typically used in larger organizations or when multiple independent domains need to be connected.

* Its important to note that the parent-child relationship between domains in question are essential to making Forest and Tree domain configurations properly work. 
