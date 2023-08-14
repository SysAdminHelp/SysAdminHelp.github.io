## DNS Query and Traversal
The traversal of your DNS Query of course depends on the content of the DNS Query. For example, initially while all DNS queries operate iteratively initially (going from your name server to your top level domain and finally to the one of the 13 root servers) and then recursively once it recieves the request (moving down the same hierarchy that it went up). However, depending on your query you may not need to even reach the root server and may be able to access cached information on the name server or top level domain server itself. The best way to remember this is that it is iterative until reaching its destination and then recursive from there. A DNS Query can have it's execution controlled by something called the TTL(Time to Live) - which controls propogation via this DNS resolver. Its important to remember the DNS Resolver utilizes caching in order to minimize the required amount of queries. This is somewhat comparable to an Address Table in networking. DNS Caching is the mechanism used by the resolver to determine if a full query/traversal needs to occur. 

## DNS Trace Demonstration

https://dns-lookup.jvns.ca/trace.html#amazon.com

The following is the results of a DNS recursion test on amazon.com - Notice while it is not mentioned that the first step begins with the root - this is because the recursive process you see here already had iteration occur behind the scenes. This should give you an idea how DNS recursion works (notice the IP Addresses mentioned up top and how the DNS Resolver is at play).

Below is an example of a query coming from one endpoint with no corresponding records for it at the TLD/Auth NS level - so it iterates immediately to a root server from a local DNS Server and then recurses down to the target host after reaching the root.

![DNS-Iteration-to-Recursion-Example.jpg](/DNS-Iteration-to-Recursion-Example.jpg)
