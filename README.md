# port-security-project
🔐 Port Security Configuration using Cisco Packet Tracer
📌 Overview

This project demonstrates how to configure Port Security on a Cisco switch using Cisco Packet Tracer.
It focuses on limiting the number of devices connected to a switch port and protecting the network from unauthorized access.

🎯 Objectives
Configure Port Security on a switch interface
Limit the number of allowed MAC addresses
Use Sticky MAC Address learning
Apply violation modes (Shutdown)
Test and verify security behavior
🛠️ Technologies Used
Cisco Packet Tracer
Cisco IOS CLI
Networking concepts (Switching & Security)
⚙️ Configuration Steps
enable
configure terminal

interface fa0/1
switchport mode access
switchport port-security
switchport port-security maximum 1
switchport port-security mac-address sticky
switchport port-security violation shutdown
🧪 Testing Scenarios
✅ Scenario 1: Normal Operation
Connect one device → Port works normally
MAC address is learned automatically
❌ Scenario 2: Violation
Connect another device with a different MAC address
Port goes into shutdown (err-disabled) state
🔍 Verification Commands
show port-security
show port-security interface fa0/1
show port-security address
🚨 Important Notes

Port Security must be enabled explicitly using:

switchport port-security
Using Sticky MAC stores learned MAC addresses automatically
Violation mode shutdown disables the port immediately
In Packet Tracer, testing may require:
Connecting multiple devices simultaneously
Or changing MAC addresses manually
💡 Key Concepts
Port Security
MAC Address Filtering
Network Access Control
Switch Security
📁 Project Files
Packet Tracer file (.pkt)
Configuration screenshots
👩‍💻 Author

Basmala Salah Attia
Cyber Security Student

⭐ Notes

This project is part of my learning journey in Cyber Security & Networking (CCNA
