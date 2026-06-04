Project 11: Internet Access Simulation Using NAT
Project Overview

This project demonstrates the implementation of Network Address Translation (NAT) in Cisco Packet Tracer. The objective was to enable devices within a private network to communicate with devices on an external network by translating private IP addresses into a public IP address.

The network consists of an internal LAN using the 192.168.1.0/24 address space and an external network using the 200.1.1.0/24 address space. NAT Overload (PAT) was configured on the router, allowing multiple internal devices to share a single public IP address for communication outside the local netw<img width="472" height="185" alt="Screenshot 2026-06-04 224554" src="https://github.com/user-attachments/assets/ef2b65b2-9124-44cb-b7aa-4bb7227cad09" />


Scenario

Organizations and home networks typically use private IP addresses that cannot be routed directly over the Internet. NAT solves this problem by translating private addresses into public addresses, allowing internal users to access external resources while conserving public IPv4 addresses.

In this project, a router was configured to perform NAT between the internal and external networks, simulating real-world Internet access.

Objectives
Design an internal and external network topology.
Configure IP addressing for all devices.
Configure NAT on the router.
Implement NAT Overload (PAT).
Verify address translation.
Test connectivity between internal and external networks.
Understand how private IP addresses are translated into public IP addresses.
Technologies Used
Cisco Packet Tracer
Cisco Router Configuration
IPv4 Addressing
Network Address Translation (NAT)
Port Address Translation (PAT)
Network Connectivity Testing
Configuration Summary
Configured the internal LAN network (192.168.1.0/24).
Configured the external network (200.1.1.0/24).
Assigned inside and outside NAT interfaces.
Created an ACL to identify internal hosts eligible for translation.
Configured NAT Overload using the router's public interface.
Verified translations using router monitoring commands.
Verification

The following tests were performed:

Verified connectivity between internal and external devices.
Confirmed successful NAT translations.
Monitored translation entries using NAT verification commands.
Validated that private addresses were translated into public addresses before reaching the external network.
Learning Outcomes
<img width="716" height="381" alt="Screenshot 2026-06-04 224518" src="https://github.com/user-attachments/assets/bff45a19-0c71-4cab-b573-b10abb2f42c6" />

<img width="716" height="381" alt="Screenshot 2026-06-04 224518" src="https://github.com/user-attachments/assets/9d39464e-3c0a-44c3-9f16-2e97c30643f1" />

This project provided practical experience with Network Address Translation (NAT), one of the most widely used technologies in modern networking. It demonstrated how routers translate private IP addresses into public addresses, allowing internal devices to communicate with external networks while improving address conservation and network security.
