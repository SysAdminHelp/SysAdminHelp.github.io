## DNS: Function and Use Cases

Small and medium enterprise (SME) businesses need a strong online presence to remain competitive. A crucial component in achieving this is the Domain Name System (DNS), which serves SMEs in several essential areas, ensuring their online success. These functions broadly fall into three categories, but note they do not cover every exact thing

**Domain Registration** enables SMEs to secure and register their desired domain names. This establishes a memorable online identity and fosters brand recognition.

**Website Hosting** is facilitated by linking domain names to servers that host SMEs' websites. This simplifies customer access to their online presence. During peak web traffic periods for an SME, DNS-based load balancing can be enabled to distribute incoming requests across multiple servers, ensuring optimal website performance.

**Disaster Recovery**  is achieved by having multiple DNS servers configured and having DNS failover implemented. This guarantees continuous availability of online services, even if one server experiences a failure.

Additionally, technologies such as Active Directory Domain Services (AD) rely on DNS to fully operate and is essential to authenticating, updating, searching, etc.

## DNS: Record Types 

There are many DNS record type with different functionalities.  For example, MX records can be stored on a DNS server and be used for directing emails to the correct servers. A and AAAA records are for mapping domain names to either IPv4(A) or IPv6(AAAA) addresses. CNAME and ANAME(Alias Record) are used for for creating names for domains or subdomains, but they have slightly different purposes. ANAME records are used to point one domain to another domain, while CNAMEs are used to make nicknames for a domain or subdomain. SRV records are utilized to help channel VOIP communications and PTR records make IP adresses to the domain anmes. There are other types of records such as TXT that is used for notes that can also be found for DNS. Below is a cheat sheet I found that covers most if not all of them.

![DNS-RECORD.png](/DNS-RECORD.png)


## DNS: Forward and Reverse Lookup Zones 
A DNS forward lookup zone is responsible for translating domain names into IP addresses, allowing us to access websites and online resources.  
A reverse lookup zone performs the opposite task by resolving IP addresses back to their associated domain names. Forward and Reverse Lookups are useful for troubleshooting network issues and verifying the legitimacy of incoming connections. Together, forward lookup zones and reverse lookup zones ensure smooth and accurate communication between domain names and IP addresses on the internet. These forward and reverse look up zones is where you would also find A records, etc. 











