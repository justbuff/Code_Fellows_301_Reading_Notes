# Understanding Network Data Delivery: Layers 2 and 3 of the OSI Model

The Open Systems Interconnection (OSI) model is a series of seven layers through which computer systems communicate. The network layer is responsible for packet forwarding, including routing through intermediate routers. The data link layer (layer 2) is the protocol layer that transfers data between nodes on a network segment across the physical layer. Layer 2 is divided into two parts, consisting of the MAC and data link sublayers, while Layer 3 includes a host’s logical address.

The OSI model's seven layers:

- Physical
- Data Link
- Network
- Transport
- Session
- Presentation
- Application

## OSI Layer 2

Layer 2 uses MAC (or physical) addressing which is able to move data across a small community of computing devices where routing traffic between multiple communities is not required. Traffic distribution for these small networks is handled by layer 2 switches that learn the MAC addresses of the computers connected to ports on the switch. The switches then send packets from the sending computer directly to the receiving device, which reduces congestion. A MAC address consists of a series of 12 hexadecimal numbers. The first six numbers are useful in identifying the manufacturer of the network interface card and the last six numbers are assigned by the card manufacturer. This avoids the possibility of having two computers on the same network with the same physical address.

Another layer 2 function is to establish protocols that relate to the structure of data frames that are placed on the network for data transmission. 

## Layer 3

Layer 3 addresses are divided in a way that identifies a specific network address and a specific host or group of hosts. When it is determined that the recipient’s network address is different from the sender’s network address, packets are directed to the network’s router for delivery handling. The TCP/IP suite of protocols are used for communication that crosses networks. 


# What Is Wireshark and How Is It Used?

Wireshark is a network protocol analyzer, or an application that captures packets from a network connection, such as from your computer to your home office or the internet. A packet is the name given to a discrete unit of data in a typical Ethernet network. Wireshark is the most often-used packet sniffer in the world.

Wireshark does three things:

Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic.

Filtering: Wireshark is capable of sorting all of this random live data using filters.

Visualization: Wireshark allows you to dive right into the very middle of a network packet. It also allows you to visualize entire conversations and network streams.

Wireshark has many uses, including troubleshooting networks that have performance issues. Cybersecurity professionals often use Wireshark to trace connections, view the contents of suspect network transactions and identify bursts of network traffic.

## Wireshark limitations

It can’t help a user who has little understanding of network protocols.

It can’t grab traffic from all of the other systems on the network under normal circumstances.

It doesn’t have actual alerts.

It can’t help with decryption with regards to encrypted traffic.

It is easy to spoof IPv4 packets.






