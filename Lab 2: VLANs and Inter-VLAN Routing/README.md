Lab 02 - VLANs and Inter-VLAN Routing
Objective

To create separate VLANs for different departments and enable communication between them using Router-on-a-Stick.

Topology

<img width="447" height="480" alt="Screenshot 2026-06-02 202400" src="https://github.com/user-attachments/assets/077641b5-a033-41b1-80c1-79a8226e5ca0" />


Devices Used
Cisco Router
Cisco Switch
3 PCs
VLAN Plan
VLAN	Department	Network
10	HR	192.168.10.0/24
20	IT	192.168.20.0/24
30	Sales	192.168.30.0/24
Configuration Steps
Created VLANs.
Assigned switch ports.
Configured trunk link.
Configured router subinterfaces.
<img width="697" height="148" alt="Screenshot 2026-06-02 202346" src="https://github.com/user-attachments/assets/caa135d9-61d5-494a-9920-f7b5f275e4f3" />
<img width="665" height="292" alt="Screenshot 2026-06-02 201239" src="https://github.com/user-attachments/assets/dd00e3c7-289d-47da-b437-5dfe6791b639" />
<img width="733" height="631" alt="Screenshot 2026-06-02 201220" src="https://github.com/user-attachments/assets/c8e569df-f5b0-4b87-8ad6-77124255ccd7" />
<img width="470" height="642" alt="Screenshot 2026-06-02 202744" src="https://github.com/user-attachments/assets/26ccd99d-ceff-4417-b829-1b5e7aaa790d" />

Tested connectivity.
Verification
Verified VLAN creation.
Verified trunk operation.
Verified inter-VLAN communication.


