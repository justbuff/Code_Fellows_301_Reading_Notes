# VirtualBox Network Settings

VirtualBox provides multiple network modes for virtual machines:

- Not Attached: A guest operating system on a VM can access hosts in a physical local area network (LAN) by using a virtual NAT (Network Address Translation) device.

- NAT: NAT Network mode for multiple virtual machines where they can communicate with each other via the network. The VMs can access other hosts in the physical network and can access external networks including the internet. 

- NAT Network: NAT Network mode for multiple virtual machines where they can communicate with each other via the network. The VMs can access other hosts in the physical network and can access external networks including the internet.

- Bridged Adapter: A VM virtual network adapter that uses the host network interface for a network connection.

- Internal Network: VMs connected to this network can communicate with each other, but they cannot communicate with a VirtualBox host machine, or with any other hosts in a physical network or in external networks. 

- Host-Only Adapter: A VM can communicate with other VMs connected to the host-only network, and with the host machine. The VirtualBox host machine can access all VMs connected to the host-only network.

- Generic Driver: This network mode allows you to share the generic network interface. A user can select the appropriate driver to be distributed in an extension pack or be included with VirtualBox.


A virtual network adapter is a software-emulated physical device. A VirtualBox VM can use up to eight virtual network adapters, each of which in turn is referred to as a network interface controller (NIC). Four virtual network adapters can be configured in the VirtualBox GUI (graphical user interface). All virtual network adapters (up to 8) can be configured with the VBoxManage modifyvm command. 

VirtualBox virtual nework adapters include:

- AMD PCnet-PCI II (Am79C970A). This network adapter is based on AMD chip and can be used in many situations. As for Windows guests, this network adapter can be used for older Windows versions (such as Windows 2000) because newer Windows versions such as Windows 7, 8 and 10 do not contain a built-in driver for this adapter.

- AMD PCnet-FAST III (Am79C973). This virtualized network adapter is supported by almost all guest operating systems that can run on VirtualBox. GRUB (the boot loader) can use this adapter for network boot.

- Intel PRO/1000 MT Desktop (82540EM). This adapter works with Windows Vista and newer Windows versions. The most of Linux distributions support this adapter as well.

- Intel PRO/1000 T Server (82543GC). Windows XP recognizes this adapter without installing additional drivers.

- Intel PRO/1000 MT Server (82545EM). This adapter model is useful to import OVF templates from other platforms and can facilitate import process.

- Paravirtualized Network Adapter (virtio-net).  A guest operating system must provide a special software interface for virtualized environments.

Port Forwarding can be accomplished on VirtualBox via SSH or HTTP access.
