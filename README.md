# Hotel Management Networ (Cisco Packet Tracer)

**Course:** Computer Networks (Fall 2024)
**Institution:** FAST NUCES Islamabad
**Section:** CS-K
**Prepared by:** Ayaan Khan (22i-0832)

---

## Objective

This project aims to design and implement a robust network architecture for a hotel management system that ensures:

* Efficient communication
* Resource sharing
* Internet connectivity across various departments and floors

Key features integrated into the network design include:

* VLANs for traffic segmentation
* DHCP for dynamic IP assignment
* NAT for internet connectivity
* Dynamic and static routing (RIP, OSPF, EIGRP)
* VLSM for optimized IP allocation
* Server-based services (HTTP, FTP, Email, SYSLOG)
* Access Control Lists (ACLs) for security

---

## Technologies Used

* **Cisco Packet Tracer** (network design and simulation)
* **Cisco Routers & Switches** (VLANs, routing, NAT)
* **Routing Protocols**: Static Routing, RIP, OSPF, EIGRP
* **Server Services**: HTTP, FTP, SMTP (Email), DNS, SYSLOG
* **Access Control Lists (ACLs)**: Network security
* **DHCP**: Dynamic IP assignment
* **NAT (Network Address Translation)**: Internet access
* **VLSM (Variable Length Subnet Mask)**: IP optimization

---

## Repository Contents

* **Project Report**: Detailed documentation of the project, including network design, implementation, results, and testing.
* **Network Design File**: Cisco Packet Tracer file containing the complete network design and configurations.

---

## Implementation Summary

### Topology

* Four routers: R1, R2, R3, and an ISP router
* VLANs:

  * R1: VLANs 70, 80, 90
  * R2: VLANs 30, 40, 50
  * R3: VLANs 10, 20

### Routing

* RIP between R2 and R3
* OSPF between R1 and R2
* EIGRP between R3 and R1
* Static routing between routers and the ISP

### DHCP & NAT

* Centralized DHCP on R3
* NAT on R3 for internet access via the ISP router

### Server Services

* HTTP, FTP, SMTP (Email), and SYSLOG

### ACLs

* Applied to regulate traffic between VLANs and secure ISP access

---

## Testing & Results

* **VLAN communication** achieved within routers
* **DHCP** assigns IPs across all VLANs
* **NAT** enables internet access
* **SMTP email services** tested and verified
* **Ping tests** confirm device connectivity
* Screenshots of packet tracing, DHCP bindings, and NAT translations included in the report

---

## Challenges & Learnings

### Challenges

* VLAN communication issues due to trunk misconfigurations
* Routing loops during dynamic protocol setup
* DHCP failures from relay agent misconfiguration
* NAT translation problems with public IP allocation

### Learnings

* The importance of proper VLSM planning
* Deep understanding of routing protocols
* Effective debugging techniques in network simulations

---

## Conclusion

This project successfully demonstrates a comprehensive network design and implementation for a hotel management system. Future improvements could include enhanced security measures (ACLs, firewalls, VPNs) to protect sensitive data and improve resilience.
