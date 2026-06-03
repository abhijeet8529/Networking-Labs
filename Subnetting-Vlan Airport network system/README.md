Airport Network Design Using Cisco Packet Tracer
Project Overview

This project simulates an airport network infrastructure using Cisco Packet Tracer. The network is divided into multiple departments including Check-in Counters, Security, Boarding Gates, and Admin Office. Variable Length Subnet Masking (VLSM) was used to efficiently allocate IP addresses based on the host requirements of each department.

The project demonstrates key networking concepts such as subnetting, VLAN configuration, trunking, Router-on-a-Stick, and Inter-VLAN Routing.

Objectives
Design a scalable airport network.
Implement VLSM subnetting for efficient IP allocation.
Create separate VLANs for each department.
Configure trunk links between the switch and router.
Implement Router-on-a-Stick for Inter-VLAN communication.
Verify connectivity between all departments.
Network Requirements
Department	Hosts Required
Check-in Counters	60
Security	40
Boarding Gates	20
Admin Office	10

Network Address: 10.1.1.0/24

Technologies Used
Cisco Packet Tracer
IPv4 Addressing
VLSM Subnetting
VLANs
Trunking
Router-on-a-Stick
Inter-VLAN Routing
VLAN Configuration
VLAN ID	Department
10	Check-in Counters
20	Security
30	Boarding Gates
40	Admin Office
VLSM Addressing Scheme
Department	Network Address	Prefix
Check-in Counters	10.1.1.0	/26
Security	10.1.1.64	/26
Boarding Gates	10.1.1.128	/27
Admin Office	10.1.1.160	/28
Features Implemented
VLAN segmentation for improved security and traffic management.
Inter-VLAN communication using Router-on-a-Stick.
Efficient IP allocation using VLSM.
Trunk configuration between switch and router.
End-to-end connectivity testing using ICMP ping.
Verification

The network was tested by performing successful ping operations between devices located in different VLANs. Switch VLAN tables, trunk status, and router subinterfaces were verified using Cisco IOS commands.

Learning Outcomes

Through this project, I gained practical experience in:

Network design and planning
VLSM subnetting
VLAN implementation
Router-on-a-Stick configuration
Inter-VLAN Routing
Network troubleshooting and verification
Conclusion

This project demonstrates the implementation of an airport network using industry-standard networking concepts. It provides hands-on experience with subnetting, VLANs, routing, and network management in a simulated enterprise environment.

screenshots :
<img width="462" height="641" alt="Screenshot 2026-06-03 131055" src="https://github.com/user-attachments/assets/d7999be3-0975-42ae-b3fe-ce04b7880611" />
<img width="675" height="157" alt="Screenshot 2026-06-03 130340" src="https://github.com/user-attachments/assets/fb98a219-641b-4976-bd6e-41ea6157b0ed" />
<img width="558" height="196" alt="Screenshot 2026-06-03 125111" src="https://github.com/user-attachments/assets/a4ad661c-c27b-431e-9bd2-68693cbe2246" />
<img width="665" height="602" alt="Screenshot 2026-06-03 124831" src="https://github.com/user-attachments/assets/d62b7ef6-30c8-4b3a-9fb8-2ab6b79af0cf" />
<img width="671" height="512" alt="Screenshot 2026-06-03 131025" src="https://github.com/user-attachments/assets/f29fa1e0-4d45-4aa7-bdb9-0e780b91f7ec" />

