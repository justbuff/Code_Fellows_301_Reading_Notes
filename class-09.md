# CIDR Block Notation

CIDR notation is a way of representing a CIDR block, which is simply a range of IP addresses. A network needs to have enough available IP addresses for use without making the CIDR block too large and wasteful.

An IPv4 (version 4 of IP) address is usually represented as four 8-bit decimal numbers or octets separated by dots, for example 127.0.0.1 (localhost on most systems). An 8-bit number when represented in the decimal system as opposed to binary has a range of 0–255. All four octets together add up to 32 bits, for a range of 0.0.0.0–255.255.255.255. In CIDR notation, this full range would be represented as 0.0.0.0/0. The final digit after the “/” represents how many bits make up the mask. The larger the mask, the smaller the range. 

# What is Network Segmentation

Network segmentation is when different parts of a computer network, or network zones, are separated by devices like bridges, switches and routers. 

Benefits of network segmentation include:

- Limiting access privileges to those who truly need it

- Protecting the network from widespread cyberattacks

- Boosting network performance by reducing the number of users in specific zones

- Damage control and limitation in case of an incident via the smaller attack surface

- Improved access control for external and internal network security

- Reducing the attack plane and scope of compliance requirements related auditing

- Improved performance with less congestion on network traffic

- Better analytics around network monitoring, network access and network devices

- Endpoint device protection, especially important as IoT devices become more common

Types of Network Segmentation zones:

- Users

- Screened Subnet

- Guest Network

- IT Workstations

- Servers by Department

- VoIP/Communications

- Traditional Physical Security

- Industrial Control Systems

- Customer Databases
