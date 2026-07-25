
<img width="1542" height="685" alt="Screenshot 2026-07-25 115051" src="https://github.com/user-attachments/assets/a772ee4f-3d05-436a-bd85-dc6c1abb44a3" />


















Hotel Management Network Using Cisco Packet Tracer
Project Overview
Project Title

Design and Implementation of a Secure Multi-Floor Hotel Management Network Using Cisco Packet Tracer

Project Description

This project demonstrates the design and implementation of a three-floor hotel management network using Cisco Packet Tracer. The network is divided into multiple departments using Virtual Local Area Networks (VLANs) to improve security, reduce broadcast traffic, and simplify network management. Dynamic routing is implemented using OSPF (Open Shortest Path First), while DHCP is configured to automatically assign IP addresses to all client devices.

Each floor has its own router, switch, wireless access point, computers, printers, laptops, tablets, and smartphones to simulate a real hotel environment. The routers are interconnected through point-to-point WAN links using separate subnet addressing.

The network ensures secure communication between departments while allowing authorized inter-VLAN communication through routing.

Objectives
Design a scalable hotel network for three floors.
Implement VLANs to separate hotel departments.
Configure DHCP for automatic IP allocation.
Configure OSPF for dynamic routing between routers.
Enable communication between all authorized VLANs.
Provide wired and wireless connectivity.
Improve network security and performance through segmentation.
Network Topology

The hotel consists of three floors, each connected through Cisco 2911 routers.

First Floor

Departments:

Reception (VLAN 80)
Store (VLAN 60)
Logistics (VLAN 70)

Devices:

PCs
Printers
Wireless Access Point
Laptops
Tablets
Smartphones
Second Floor

Departments:

Sales (VLAN 30)
HR (VLAN 40)
Finance (VLAN 50)

Devices:

PCs
Printers
Wireless Access Point
Laptops
Tablets
Smartphones
Third Floor

Departments:

IT (VLAN 10)
Administration (VLAN 20)

Devices:

PCs
Printers
Wireless Access Point
Laptops
Tablets
Smartphones
VLAN Configuration
VLAN	Department	Network
VLAN 10	IT	192.168.1.0/24
VLAN 20	Administration	192.168.2.0/24
VLAN 30	Sales	192.168.3.0/24
VLAN 40	HR	192.168.4.0/24
VLAN 50	Finance	192.168.5.0/24
VLAN 60	Store	192.168.6.0/24
VLAN 70	Logistics	192.168.7.0/24
VLAN 80	Reception	192.168.8.0/24
Routing

The three routers are connected using point-to-point /30 networks.

Link	Network
F2 ↔ F3	10.10.10.0/30
F3 ↔ F1	10.10.10.4/30
F2 ↔ F1	10.10.10.8/30

Dynamic routing is achieved using OSPF, allowing all VLAN networks to be learned automatically without manually configuring static routes.

DHCP Configuration

Each VLAN has its own DHCP scope.

DHCP automatically provides:

IP Address
Default Gateway
Subnet Mask
DNS Server (if configured)

This eliminates manual IP configuration and simplifies device management.

Switching

Cisco 2960 switches are configured to:

Create VLANs
Assign access ports
Configure trunk ports between switches and routers
Forward traffic efficiently within each VLAN
Wireless Connectivity

Each floor includes an Access Point providing wireless access for:

Laptops
Smartphones
Tablets

Wireless users automatically receive IP addresses through DHCP and can communicate with authorized resources.

Security Features
Department separation using VLANs
Reduced broadcast domains
Controlled inter-VLAN communication
Dynamic routing using OSPF
Separate IP subnet for every department
Improved scalability and easier troubleshooting
Devices Used
Routers
Cisco 2911 (3)
Switches
Cisco 2960-24TT (3)
Wireless
Access Points (3)
End Devices
Desktop PCs
Printers
Laptops
Tablets
Smartphones
Technologies Implemented
VLAN
Inter-VLAN Routing
OSPF
DHCP
Wireless Networking
Static IP addressing for infrastructure devices
Access Ports
Trunk Ports
Subnetting
Point-to-Point WAN Links
Advantages
Centralized and efficient hotel network.
Automatic IP management through DHCP.
Fast route convergence using OSPF.
Better security through VLAN segmentation.
Easy expansion for future hotel departments.
Supports both wired and wireless users.
Simplifies administration and troubleshooting.
Expected Outcome

The completed network allows every department of the hotel to operate on its own secure VLAN while still communicating with other authorized departments through OSPF-based routing. Employees and hotel staff can connect through both wired and wireless devices, receive IP addresses automatically via DHCP, and access shared resources such as printers and servers. The design is scalable, secure, and suitable for a real-world hotel management environment.

Conclusion

This Cisco Packet Tracer project successfully implements a three-floor hotel management network using industry-standard networking technologies such as VLANs, DHCP, OSPF, trunking, and inter-VLAN routing. By dividing the network into separate departmental VLANs, the design improves security, reduces unnecessary broadcast traffic, and enhances overall performance. The use of OSPF ensures efficient dynamic routing between floors, while DHCP simplifies IP address management for all wired and wireless devices. Overall, the project demonstrates a reliable, scalable, and well-organized enterprise network that reflects the communication requirements of a modern hotel management system.
