Packet Tracer Practice Lab – Medium Office Network

This project contains a complete network design for a medium-sized office using Cisco Packet Tracer.
The company has three departments and requires proper network segmentation, communication between all departments, and correct use of Cisco devices.

📌 Project Overview

The office currently has three departments:

Department	Number of Computers
IT	100
Sales	16
HR	40

The company has reserved the IP block 192.168.10.0/24 for the entire network.

Goal: Build a scalable, segmented network using only:

One Cisco 2960-24T switch

One Cisco 2911 router

Three PCs per department (for the lab file)

One laptop for console access

🖧 Network Requirements

Each department must have its own LAN / VLAN

All departments must be able to communicate with each other

IP addressing must be done using the best segmentation method

Correct cabling must be used between devices

Laptop connected to switch or router for access

🔍 IP Segmentation Method
✔ Recommended: VLSM (Variable Length Subnet Masking)

VLSM allows efficient use of the 192.168.10.0/24 network by creating subnets sized exactly for each department.
This prevents IP wastage and supports future departmental expansion.

🧮 Subnet Summary (Example)
Department	Required Hosts	Subnet	Mask	IP Range	Broadcast
IT	100	192.168.10.0/25	/25	192.168.10.1–126	192.168.10.127
HR	40	192.168.10.128/26	/26	192.168.10.129–190	192.168.10.191
Sales	16	192.168.10.192/27	/27	192.168.10.193–222	192.168.10.223
Future Use	—	Remaining space in /27 blocks	—	—	—
🖥️ Devices Used

Cisco 2911 Router

Cisco 2960 24-Port Switch

3× PCs per department

1× Laptop for console
