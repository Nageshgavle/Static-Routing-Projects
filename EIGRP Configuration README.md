🖧 EIGRP Configuration – Cisco Packet Tracer Lab

This project demonstrates the configuration and verification of Enhanced Interior Gateway Routing Protocol (EIGRP) in a multi-router network using Cisco Packet Tracer.
The lab focuses on enabling dynamic routing, improving network convergence, and ensuring efficient communication between different network segments.

📌 Project Overview

In this lab, EIGRP is configured on Cisco routers to enable automatic route exchange.
The key objectives of this project include:

Configuring EIGRP with an Autonomous System (AS) number

Advertising network subnets

Verifying neighbour relationships

Testing routing connectivity

Ensuring efficient and loop-free routing

🏗️ Topology Used

The topology includes multiple routers connected across different networks.
Each router participates in the same EIGRP AS and shares routing information dynamically.

(You can add a screenshot of your topology here.)

⚙️ Configuration Steps
1️⃣ Enable EIGRP on Each Router
Router(config)# router eigrp <AS-number>

2️⃣ Advertise Networks
Router(config-router)# network <network-address> <wildcard-mask>

3️⃣ Disable Auto-Summary (Recommended)
Router(config-router)# no auto-summary

4️⃣ Verify EIGRP Neighbours
Router# show ip eigrp neighbors

5️⃣ Verify Routing Table
Router# show ip route

6️⃣ End-to-End Connectivity Test
Router# ping <destination-IP>

📂 Project Files

EIGRP CONFIGURATION.pkt – Cisco Packet Tracer file containing the full EIGRP setup and routing.

📘 Learning Outcomes

After completing this lab, you will understand:

✔ How to configure EIGRP on Cisco routers
✔ How EIGRP discovers neighbours
✔ How routes are exchanged dynamically
✔ How to check and troubleshoot EIGRP operation
✔ How to verify connectivity across networks

🚀 How to Use This Project

Download the .pkt file from this repository

Open it in Cisco Packet Tracer

Explore the router configuration

Modify, expand, or test routing behaviour as needed

🧑‍💻 Author

Nagesh Gavale
CCNA | Networking Learner | IT Support | Linux
