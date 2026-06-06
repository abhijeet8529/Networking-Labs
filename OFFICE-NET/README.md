Large Office Network Simulation using VLANs & DHCP (Cisco Packet Tracer)
📌 Project Overview

<img width="1245" height="612" alt="Screenshot 2026-06-06 175854" src="https://github.com/user-attachments/assets/370d0b04-5c77-45c5-8611-5bbdc55e28e4" />

This project demonstrates the design and implementation of a Large Office Network using Cisco Packet Tracer. The network is divided into multiple departments using VLANs to improve security and network management. Router-on-a-Stick inter-VLAN routing is configured to allow communication between VLANs, while DHCP automatically assigns IP addresses to devices.

The topology includes wired and wireless devices such as PCs, laptops, smartphones, printers, and access points, simulating a real office environment.

🏢 Network Design

The office is divided into three departments:

Department	VLAN	Network
Admin	VLAN 10	192.168.1.0/26
Finance/HR	VLAN 20	192.168.1.64/26
Customer Service/Reception	VLAN 30	192.168.1.128/26

Each department contains:

Desktop PC
Printer
Wireless Access Point
Laptop
Smartphone

All devices connect to a central 2960 Switch, which connects to a 2911 Router for routing between VLANs.

🛠️ Technologies Used
Cisco Packet Tracer
VLAN Configuration
Router-on-a-Stick
IEEE 802.1Q Trunking
DHCP Configuration
Inter-VLAN Routing
Wireless Access Points
Static Network Design
📋 Steps Followed to Build the Project
Step 1: Designed the Network Topology
Added one Router (2911)
Added one Switch (2960)
Created three departments
Added PCs, Printers, Laptops, Smartphones, and Access Points
Connected devices using appropriate cables
Step 2: Planned the IP Addressing Scheme

Used subnetting to divide the network:

Admin
192.168.1.0/26

Finance/HR
192.168.1.64/26

Customer Service
192.168.1.128/26

Each subnet provides up to 62 usable host addresses.

Step 3: Created VLANs on the Switch

Configured three VLANs:

VLAN 10
Name: ADMIN

VLAN 20
Name: FINANCE

VLAN 30
Name: CUSTOMER
Step 4: Assigned Switch Ports

Assigned device ports to their respective VLANs:

Admin Devices
→ VLAN 10

Finance Devices
→ VLAN 20

Customer Devices
→ VLAN 30

Ports were configured as:

switchport mode access
switchport access vlan X
Step 5: Configured Trunk Link

Configured the switch port connected to the router as a trunk:

interface Fa0/24

switchport mode trunk

This allows multiple VLANs to pass through a single connection.

Step 6: Configured Router-on-a-Stick

Created subinterfaces on the router:

G0/0.10
Encapsulation dot1Q 10

G0/0.20
Encapsulation dot1Q 20

G0/0.30
Encapsulation dot1Q 30

Assigned gateway addresses:

192.168.1.1
192.168.1.65
192.168.1.129

These serve as the default gateways for each VLAN.

Step 7: Configured DHCP

Created separate DHCP pools for every VLAN.

Example:

ip dhcp pool ADMIN

network 192.168.1.0 255.255.255.192

default-router 192.168.1.1

Similarly configured:

Finance Pool
Customer Pool

Reserved gateway addresses from allocation.

Step 8: Configured Wireless Devices

Configured Access Points and connected:

Laptops
Smartphones

These devices automatically received IP addresses through DHCP.
