
## CIA Triad: Context and Examples 

The CIA triad consists of three fundamental principles in information security: Confidentiality, Integrity, and Availability. Let's break down each principle and provide examples of both logical and physical controls for each:

Confidentiality:
Logical Control: Network Access Control Lists (ACLs) can be implemented on network devices to restrict access to specific ports. For example, by allowing only Secure Shell (SSH) traffic (port 22) and blocking Telnet (port 23), you enhance confidentiality. SSH provides encryption, whereas Telnet transmits data in plain text, making it vulnerable to eavesdropping.

Physical Control: Physical access controls, such as locked server rooms or secure cabinets, can prevent unauthorized individuals from physically accessing sensitive information. These controls ensure that only authorized personnel can access the equipment and maintain confidentiality.

Integrity:
Logical Control: Role-Based Access Control (RBAC) implemented through Active Directory can enforce integrity. By assigning users specific roles and granting them appropriate permissions, RBAC ensures that users only have access to the resources necessary to perform their job functions. This prevents unauthorized modification or deletion of data and helps maintain data integrity.

Physical Control: Regular backups and checksum verification mechanisms are physical controls that support data integrity. Backing up data ensures that if data is lost or corrupted, it can be restored from a known good state. Additionally, checksum verification mechanisms can detect data tampering by comparing the calculated checksum of a file with its original checksum.

Availability:
Logical Control: Implementing redundant power supplies for a Windows Server is a logical control that enhances availability. Redundant power supplies ensure that if one power supply fails, the server can still operate without interruption, minimizing downtime and ensuring continuous availability.

Physical Control: Physical security measures such as uninterruptible power supply (UPS) systems and backup generators help maintain availability. UPS systems provide power backup in case of electricity outages or fluctuations, while backup generators can provide longer-term power supply during extended outages, ensuring continuous availability of critical systems.
