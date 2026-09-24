
# Dynamic NAT

### Summary 

* This lab focuses on the implementation of Dynamic NAT. 
* Dynamic NAT uses a pool of public IP addresses to translate private LAN IP addresses. 
* When internal hosts initiate communication with external networks, the router dynamically assigns an available public IP from the pool on a first-come, first-served basis.

---

## Topology Architecture

![Topology](NAT_topology.png)

---

### Network Environment Specifications
* **Simulation Environment:** EVE-NG Community Edition
* **Router Image Version:** Cisco IOL/IOU L3 Advanced Enterprise (L3-adventerprisek9-15.5.2T.bin)
* **Switch Image Version:** Cisco IOL/IOU L2 Advanced Enterprise (L2-ADVENTERPRISE-M-15.1-20140814.bin)

---

### IP Addressing Table

| Device  | Interface  | IP Address  |Subnet Mask   |Default Gateway   |Description   |
|:---:|:---:|:---:|:---:|:---:|:---:|
|Router  |Ethernet 0/0   |200.0.0.1   |255.255.255.248   |N/A   |Interface to Internet   |
|   | Ethernet 0/1   |192.168.1.1   |255.255.255.0   |N/A   |LAN Subnet   |
|Internet   |Ethernet 0/0   |200.0.0.2   |255.255.255.248   |N/A   |Interface to Router   |
|PC1   |Ethernet 0/0   |192.168.1.10   |255.255.255.0    |192.168.1.1   |LAN host   |
|PC2   |Ethernet 0/0   |192.168.1.20   |255.255.255.0    |192.168.1.1   |LAN host   |

---

**Configurations:** [View all configurations](./configs/Dynamic_NAT__configurations.txt)

**Verifications:** [View all verifications](./configs/Dynamic%20NAT_verifications.txt)

---

<p align="center">Copyright © 2026 Sanuth Mawilmada. Licensed under the <a href="./LICENSE">MIT License</a>.</p>