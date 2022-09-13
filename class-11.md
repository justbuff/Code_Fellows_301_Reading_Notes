# Network Address Translation (NAT)

Network Address Translation (NAT) is a process in which one or more local IP address is translated into one or more Global IP address and vice versa in order to provide Internet access to the local hosts. It also translates port numbers by masking the port number of the host with another port number in the packet that will be routed to the destination. It then makes the corresponding entries of IP address and port number in the NAT table. NAT generally operates on a router or firewall. 

The router which has one interface in the local (inside) network and one interface in the global (outside) network is configured for NAT network. When a packet traverses outside the local (inside) network, then NAT converts that local (private) IP address to a global (public) IP address. When a packet enters the local network, the global (public) IP address is converted to a local (private) IP address. If NAT runs out of addresses then the packets will be dropped and an Internet Control Message Protocol (ICMP) host unreachable packet is sent to the destination.

3 ways to configure NAT: 

Static NAT – a single unregistered (Private) IP address is mapped with a legally registered (Public) IP address i.e one-to-one mapping between local and global addresses. This is generally used for Web hosting.

Dynamic NAT – an unregistered IP address is translated into a registered (Public) IP address from a pool of public IP addresses. 
 
Port Address Translation (PAT) – many local (private) IP addresses can be translated to a single registered IP address. Port numbers are used to distinguish the traffic i.e., which traffic belongs to which IP address.
 
## Advantages of NAT

- NAT conserves legally registered IP addresses. 
 
- It provides privacy as the device’s IP address, sending and receiving the traffic, will be hidden. 
 
- Eliminates address renumbering when a network evolves. 
 
## Disadvantages of NAT
 
- Translation results in switching path delays. 
 
- Certain applications will not function while NAT is enabled. 
 
- Complicates tunneling protocols such as IPsec. 
