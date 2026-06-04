# Project 10: Restricted Access Network Using ACLs

## Project Overview

This project demonstrates the implementation of Access Control Lists (ACLs) to enforce network security policies in a small enterprise network using Cisco Packet Tracer. The network consists of two departments, Human Resources (HR) and Sales, connected through a router.

The primary objective was to restrict Sales users from accessing HR resources while allowing normal communication for authorized traffic. Extended ACLs were configured on the router to filter traffic based on source and destination networks. The project showcases how ACLs can be used to control network access, improve security, and protect sensitive organizational data.

## Scenario

An organization maintains separate HR and Sales departments. The HR department stores confidential employee information such as salary records, personal details, and internal documents. To protect these resources, management requires that Sales employees must not be able to access the HR network.

To achieve this, an Extended ACL is implemented on the router to deny traffic originating from the Sales network and destined for the HR network while permitting all other traffic.

## Objectives

* Design a departmental network topology.
* Configure IPv4 addressing on routers and end devices.
* Implement Extended Access Control Lists (ACLs).
* Restrict Sales department access to HR resources.
* Apply ACLs to the appropriate router interface.
* Verify access restrictions using connectivity tests.
* Understand traffic filtering and network security concepts.

## Technologies Used

* Cisco Packet Tracer
* Cisco Router Configuration
* IPv4 Addressing
* Extended ACLs
* Network Security Policies
* Connectivity Verification and Troubleshooting

## Configuration Summary

* Configured separate networks for HR and Sales departments.
* Assigned IP addresses and default gateways.
* Created an Extended ACL to deny Sales-to-HR traffic.
* Applied the ACL to the Sales-facing router interface.
* Permitted all remaining network traffic.
* Verified policy enforcement through ping and connectivity testing.

## Verification

The network was tested to ensure that:

* Sales users could not access HR resources.
* ACL rules were correctly matched and enforced.
* Router interfaces remained operational.
* Security policies functioned as intended.

## Learning Outcomes

Through this project, practical experience was gained in implementing Access Control Lists, controlling traffic flow, securing departmental networks, and troubleshooting ACL-related issues. The project demonstrates how routers can be used to enforce security policies and protect sensitive network resources in real-world environments.
screenshot:

<img width="481" height="345" alt="Screenshot 2026-06-04 114832" src="https://github.com/user-attachments/assets/724fdc31-ca7d-423d-8f6e-80e072395590" />
<img width="477" height="218" alt="Screenshot 2026-06-04 123747" src="https://github.com/user-attachments/assets/83ca103f-44af-4d1b-ba6e-b08847f007be" />
<img width="607" height="116" alt="Screenshot 2026-06-04 120720" src="https://github.com/user-attachments/assets/4f65cefa-6035-4c0c-b3ae-d559f5be0918" />
<img width="477" height="177" alt="Screenshot 2026-06-04 120543" src="https://github.com/user-attachments/assets/a7babed3-1045-404a-befa-155c17fc0ce6" />
<img width="453" height="207" alt="Screenshot 2026-06-04 120520" src="https://github.com/user-attachments/assets/de50e3f5-213f-4704-9fb0-744db1160295" />
<img width="467" height="262" alt="Screenshot 2026-06-04 114940" src="https://github.com/user-attachments/assets/54b2a8aa-cb42-4ed4-903a-657420354c60" />

