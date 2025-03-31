<h1>🌐 Sales Organization Network Lab</h1>

<h2>📌 Overview</h2>
This project simulates a **sales organization network** in Cisco Packet Tracer. It focuses on **VLAN configuration, DHCP setup, and inter-VLAN routing** to segment departments, assign IP addresses dynamically, and enable communication across VLANs using a multilayer switch. The network includes three access switches, a router, and three servers (DHCP, DNS, HTTP).

<h2>🛠 Tools & Technologies Used</h2>

- **Cisco Packet Tracer** – Network simulation and configuration  
- **Multilayer Switch (Cisco 3560)** – Inter-VLAN routing and VLAN management  
- **Access Switches (Cisco 2950)** – VLAN segmentation and trunking  
- **Servers (DHCP, DNS, HTTP)** – Dynamic IP assignment, domain resolution, and web services  
- **Router (Cisco 2911)** – External connectivity  

<h2>🔍 Network Configuration & Features</h2>

| Feature | Description | Implementation |
|---------|-------------|----------------|
| **VLAN Segmentation** | Separates departments for security and organization. | Configured VLANs: Sales (20), IT (10), HR (30), Management (40), IP Phones (100), Servers (99). |
| **DHCP Configuration** | Assigns IP addresses dynamically to devices. | Set up DHCP pools on a server in VLAN 99 with `ip helper-address` on VLAN interfaces. |
| **Inter-VLAN Routing** | Enables communication between VLANs. | Configured a multilayer switch with VLAN interfaces and routing. |
| **Trunking** | Carries multiple VLAN traffic between switches. | Set up trunk ports on Switch 0, Switch 1, and Switch 2 with `switchport mode trunk`. |
| **Server Services** | Provides DHCP, DNS, and HTTP services. | Configured DHCP for IP assignment, DNS for name resolution, and HTTP for web access in VLAN 99. |

<h2>📐 Network Topology</h2>

![Network Topology](https://github.com/user-attachments/assets/141f84f1-733b-495b-846b-a94e70281b70)   
*The topology includes a multilayer switch connected to three access switches (Switch 0, Switch 1, Switch 2), a router, three servers (DHCP, DNS, HTTP) in VLAN 99, and devices in VLANs 10, 20, 30, 40, and 100.*

<h2>✅ Networking Best Practices & Key Takeaways</h2>

🔹 **VLANs** enhance **network security** by isolating department traffic.  
🔹 **DHCP** simplifies IP management with **dynamic addressing**.  
🔹 **Inter-VLAN routing** ensures efficient communication across departments.  
🔹 **Trunking** is critical for **multi-VLAN traffic** between switches.  
🔹 **Dedicated servers** for DHCP, DNS, and HTTP improve **network functionality**.  
