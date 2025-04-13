# Enterprise Network Simulation – Cisco Packet Tracer

**Student Name:** Somnath Gorai  
**Register No.:** 23BCAR0339  
**Semester:** IV – BCA (IoT Specialization)  
**Course:** 23BCA4VC02 – Network Administration  
**College:** JAIN (Deemed-to-be University)  
**Submission Date:** 15th April 2025  
**Faculty In-Charge:** Mr. Sahabzada Betab Badar

---

## Case Study

Radeon Company Ltd., a US-based enterprise in the Banking and Insurance sector, is expanding into Nairobi, Kenya. The company has secured a four-story building and wants to implement a scalable and secure network infrastructure.

The task was to design, configure, and simulate a real-world enterprise network that supports inter-department communication, secure remote access, wireless connectivity, DHCP automation, and proper IP segmentation using VLANs.

---

## Devices Used

- **Routers (Cisco 2911):** 4
  - FLOOR-1-ROUTER
  - FLOOR-2-ROUTER
  - FLOOR-3-ROUTER
  - FLOOR-4-ROUTER

- **Layer 3 Switches:** 4
  - FLOOR-1-L3-SW
  - FLOOR-2-L3-SW
  - FLOOR-3-L3-SW
  - FLOOR-4-L3-SW

- **Layer 2 Switches (2960-24TT/24PT):** 12
  - FLOOR-1-MGT-SW, RSC-SW, HR-SW
  - FLOOR-2-MKT-SW, ACC-SW, FINANCE-SW
  - FLOOR-3-LOG-SW, CUST-SW, GST-SW
  - FLOOR-4-ADMIN-SW, ICT-SW, SVR-SW

- **End Devices:**
  - 11 PCs (one per department)
  - 11 Printers (one per department)
  - 11 Wireless Access Points

- **Servers:**
  - DHCP Server
  - Email Server
  - HTTPS Server

---

##  IP Addressing and VLAN Mapping

- **Base Network:** 192.168.10.0/24  
Each department was allocated a /26 subnet (supports up to 62 hosts) and a unique VLAN:

- VLAN 10 – Management: 192.168.10.0/26  
- VLAN 20 – Research: 192.168.10.64/26  
- VLAN 30 – Human Resource: 192.168.10.128/26  
- VLAN 40 – Marketing: 192.168.10.192/26  
- VLAN 50 – Accounts: 192.168.11.0/26  
- VLAN 60 – Finance: 192.168.11.64/26  
- VLAN 70 – Logistics: 192.168.11.128/26  
- VLAN 80 – Customer: 192.168.11.192/26  
- VLAN 90 – Guest: 192.168.12.0/26  
- VLAN 100 – Admin: 192.168.12.64/26  
- VLAN 110 – ICT: 192.168.12.128/26  
- VLAN 120 – Server Room: 192.168.12.192/26

**Router-to-Router and Router-to-Switch Connections:**  
Used 10.10.10.0/30 base network for point-to-point links between routers and L3 switches.

---

##  Configuration Highlights

- **Routing Protocol:** OSPF (Open Shortest Path First)
- **Switching:** Inter-VLAN routing via Layer-3 Switches using SVIs
- **Wireless Access:** Configured Access Points for each floor
- **Security Features:**
  - SSH on all routers and L3 switches
  - Sticky MAC-based port security on L2 switches
- **IP Management:** Centralized DHCP server with helper addresses
- **Services Deployed:**
  - DHCP server (192.168.12.196)
  - DNS service (internal resolution)
  - HTTP and Email servers
- **Banner messages, hostnames, password encryption, and domain lookup disabled across all devices**

---

##  Learning Outcomes

- Understood the practical application of **Hierarchical Network Design**
- Learned how to create and apply **VLANs and Inter-VLAN Routing**
- Practiced **IP subnetting** for multiple departments with a fixed base network
- Gained skills in configuring **OSPF** routing across a 4-router topology
- Implemented **dynamic IP assignment** using DHCP relay on Layer-3 switches
- Configured **secure remote access using SSH**
- Applied **Port Security** to prevent unauthorized access at Layer 2
- Learned to deploy and test **enterprise-level services** (DNS, Email, HTTP)
- Enhanced understanding of **Cisco Packet Tracer** simulation environment
- Strengthened real-world skills in **network planning, troubleshooting, and documentation**

---

##  GitHub Pages Link

[ View Project GitHub Page](https://alaxneon.github.io/EnterpriseNetwork_CPT)

---

##  References

- [Cisco Packet Tracer Full Lab – VLAN, Inter-VLAN Routing, DHCP, SSH](https://www.youtube.com/watch?v=ebAqdDfIGhk)
- [Advanced Networking in Packet Tracer – Full Enterprise Setup](https://www.youtube.com/watch?v=NU3jmb0eN_A)
- [Enterprise Network Design Tutorial](https://www.youtube.com/watch?v=SEO0GGTtyIk)

---

© 2025 – Somnath Gorai | JAIN (Deemed-to-be University)
