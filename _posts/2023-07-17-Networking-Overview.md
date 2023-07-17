 ## What is Computer Networking 
A good way to think of networking would be that it is the practice of connecting devices to share resources and enable communication. It involves hardware devices, software protocols, and technologies that facilitate data transfer and collaboration among connected devices. Once two devices are connected to eachother, you basically have a computer network

 ## Cabling: Ethernet vs Fiber.

At a granular level, there is a very very simple distinction between ethernet and fiber. Ethernet cables are based on twisted pairs of wires in a sleeve. The reason they are twisted is to aid in reducing electrical interference with the connection and in turn basically provides shielding. Fibre cables utilize light and not a twisted pair schema and in turn as basically almost as fast as the speed of light. From an small and medium business perspective, ethernet will most likely be your go to even though the copper used for ethernet cables is actually only dictated to be used for no more than 100 metres. Fibre cabling would be best to use for distances well beyond 100m, and is excellent for use by ISPs as they are often immune to electromagnetic and weather conditions.

 ## Network Topgraphy: WAN and LAN 

Networks can generally be seperated between two zones called the WAN and LAN. The WAN or Wide Area Network can be defined as basically network traffic between networks via the intrnet, whereas LAN covers intanetwork communications. A good example of LAN is how gamers use to do LAN parties, where gamers would bring PCs to their friends house and have them join the network. The WAN as you could imagine mostly deals with routing wheras the LAN mostly deals with switching - and therein lies the significance. 

 ## Switching vs Routing In Practice 
Switching and Routing although similar actually require communication in a very different way. When a device within a LAN sends data to another device, the switch examines the destination MAC address found in the data frame. Using its internal MAC address table, the switch determines the appropriate port to forward the data. The switch ensures that the data reaches the device with the matching destination MAC address.

When a device sends data to a device in a different network, the router examines the destination IP address found in the IP packet. Using its routing table, which contains information about network topology and available paths, the router determines the best path or interface through which to forward the data. The router then forwards the data to the next hop or intermediate router based on the routing table's information. This process continues until the data reaches the destination network. Each intermediate router along the path is referred to as a hop, as the data "hops" from one router to the next until it reaches its final destination.















