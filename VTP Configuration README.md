🖧 VTP Configuration – Cisco Packet Tracer Lab

This project demonstrates how to configure VTP (VLAN Trunking Protocol) to manage VLANs centrally across multiple switches in Cisco Packet Tracer.
The goal is to automate VLAN distribution, reduce administrative overhead, and maintain consistent VLAN information across the network.

📌 Project Overview

In this lab, VTP is used to centralize VLAN management.
Key objectives include:

Configuring VTP modes (Server, Client, Transparent)

Setting the VTP domain name

Configuring the VTP password

Creating VLANs on the server switch

Distributing VLAN information across client switches

Setting trunk links between switches

Verifying VTP operation

🏗️ Network Topology

The topology includes:

1 VTP Server Switch

Multiple VTP Client Switches

Trunk links connecting all switches

VLANs propagated across the network through the VTP domain

(Insert a screenshot of your Packet Tracer topology here.)

⚙️ Configuration Steps
1️⃣ Set VTP Domain Name
Switch(config)# vtp domain <domain-name>

2️⃣ Configure VTP Mode

Server Mode

Switch(config)# vtp mode server


Client Mode

Switch(config)# vtp mode client


Transparent Mode

Switch(config)# vtp mode transparent

3️⃣ Set VTP Password (Recommended)
Switch(config)# vtp password <password>

4️⃣ Create VLANs (on Server)
Switch(config)# vlan 10
Switch(config)# vlan 20
Switch(config)# vlan 30

5️⃣ Configure Trunk Ports
Switch(config)# interface f0/1
Switch(config-if)# switchport mode trunk

6️⃣ Verify VTP Status
Switch# show vtp status

📂 Project Files

VTP.pkt — Cisco Packet Tracer file containing VTP server & client configuration.

📘 Learning Outcomes

After completing this lab, you will understand:

✔ How VTP manages VLANs dynamically
✔ Differences between VTP server, client, and transparent modes
✔ How VLANs propagate across trunk links
✔ How to verify and troubleshoot VTP
✔ Benefits of centralized VLAN management

🚀 How to Use This Repository

Download the .pkt file

Open it using Cisco Packet Tracer

View VTP configuration on each switch

Edit, add, or propagate VLANs for practice

Modify trunk connections to see VTP effects

🧑‍💻 Author

Nagesh Gavale
Networking Learner | CCNA | Linux | IT Support
