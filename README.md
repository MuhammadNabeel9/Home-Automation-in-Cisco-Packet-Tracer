# Home Automation System using Cisco Packet Tracer
# Project Overview

The Home Automation System is a smart networking project developed using Cisco Packet Tracer that demonstrates how Internet of Things (IoT) devices can be integrated into a modern home. The system allows multiple smart devices to communicate over a secure network, enabling users to monitor and control household appliances remotely.

This project simulates a real-world smart home environment where devices such as lights, fans, doors, security cameras, motion sensors, smoke detectors, and other IoT appliances are connected through routers, switches, wireless access points, and IoT gateways.

The primary objective of this project is to showcase how networking technologies and IoT can improve home security, convenience, automation, and energy efficiency.

# Features
🏠 Smart Home Network Simulation

📶 Wireless IoT Device Connectivity

💡 Smart Lighting Control

🌡️ Automated Temperature Monitoring

🚪 Smart Door Lock System

📷 Home Security Surveillance

🚨 Motion Detection & Alarm System

🔥 Smoke Detection and Safety Alerts

📱 Remote Device Management

🌐 Internet-enabled Smart Devices

🔒 Secure Network Communication

⚡ Energy-Efficient Home Automation

# Technologies Used
Cisco Packet Tracer

Internet of Things (IoT)

Wireless Networking

Routers

Switches

Home Gateway

Access Point

DHCP

IPv4 Addressing

IoT Registration Server

# Project Objectives
Design a smart home network using Cisco Packet Tracer.
Connect IoT devices through a centralized Home Gateway.
Demonstrate communication between smart devices.
Simulate automated home operations.
Improve home security using sensors and surveillance.
Learn practical implementation of IoT networking concepts.

# Learning Outcomes
Understanding IoT architecture

Cisco Packet Tracer simulation

Smart device networking

Wireless communication

IP addressing and DHCP

Home automation concepts

Network security basics

IoT device configuration

# Simulation
This project is fully implemented in Cisco Packet Tracer (.pkt) and demonstrates a realistic smart home environment where connected devices interact over an IoT-enabled network.

# Home Automation System – Components and Their Working
# 1. 📱 Smartphone (Smartphone0)
# Working

Acts as the remote user device.

Connects to the Cell Tower through the cellular network.

Sends commands to control IoT devices (light, fan, door, webcam, etc.).

Can monitor and manage the home remotely through the Home Gateway.

# How to Check

Open Smartphone0.

Go to Desktop → Web Browser.

Enter the Home Gateway IP (or IoT Registration Server if configured).

If the control page opens, the smartphone is connected successfully.

# 2. 📡 Cell Tower (Cell Tower0)

# Working

Provides cellular communication between the smartphone and the ISP network.

Transfers data from the smartphone to the Central Office Server.

# How to Check

Ensure the wireless link between Smartphone and Cell Tower is active (blue connection).

In Simulation Mode, packets should travel from Smartphone to Cell Tower.

# 3. 🖥 Central Office Server

# Working
Represents the telecom company's central office.

Routes mobile communication toward the ISP router.

# How to Check

Open the server.

Go to Services.

Verify required services are enabled.

In Simulation Mode, packets should pass through this server.

# 4. 🌐 ISP Router (2911)

# Working

Connects the home network to the Internet.

Routes traffic between servers and the home gateway.

Acts as the main routing device.

# How to Check

Open the router.

CLI

show ip interface brief

Interfaces should display up/up.

# Check routing:

show ip route

Ping the Home Gateway:

ping <Home Gateway IP>

Successful replies indicate proper routing.

# 5. 🔀 Switch (2960)

# Working

Connects the DNS Server and DHCP Server.

Forwards frames using MAC addresses.

# How to Check

Open the switch CLI:

show mac address-table

Connected devices should appear.

Also check:

show interfaces status

Ports should be connected.

# 6. 🌍 DNS Server

# Working

Converts domain names into IP addresses.

Helps devices locate servers.

# How to Check

Open Server0.

Go to:

Services → DNS

Verify DNS service is ON.

From a PC:

nslookup example.com

If an IP is returned, DNS is working.

# 7. 📦 DHCP Server

# Working

Automatically assigns IP addresses.

Prevents manual IP configuration.

# How to Check

Open Server1.

Go to:

Services → DHCP

Ensure DHCP service is ON.

On Laptop:

Desktop → IP Configuration

Click DHCP.

If an IP address is assigned automatically, DHCP is working.

# 8. ☁ Cloud

# Working

Represents the Internet.

Connects the ISP Router with the Cable Modem.

How to Check

Use Simulation Mode.

Packets should successfully travel through the cloud.

# 9. 📶 Cable Modem

# Working

Converts ISP signals into Ethernet.

Connects the Internet to the Home Gateway.

# How to Check

Check link LEDs.

Ping from Home Gateway to ISP Router.

Successful replies indicate proper operation.

# 10. 🏠 Home Gateway

# Working

This is the brain of the smart home.

It:

Connects all IoT devices.

Provides Wi-Fi.

Registers smart devices.

Controls automation.

Allows remote access.

# How to Check

Open Home Gateway.

Go to:

Config

Check:

Internet IP
Wireless Status
IoT Registration

Then go to:

GUI → IoT Monitor

All registered devices should appear.

# 11. 💻 Laptop

# Working

Used to configure and monitor the Home Gateway.

Can access IoT devices using a web browser.

How to Check

Desktop
→ Web Browser

Enter Home Gateway IP.

If the login page opens, the laptop is connected.

Also check:

Desktop → Command Prompt

ping <Home Gateway IP>

# 12. 💡 Smart Light

# Working

Turns ON/OFF remotely.

Can be automated using schedules or sensors.

How to Check

Open Home Gateway.

Go to IoT Monitor.

Click Light.

Turn ON/OFF.

If the bulb changes state, it is connected successfully.

# 13. 🌀 Smart Fan

# Working

Can be switched ON/OFF remotely.

May work automatically based on temperature.

How to Check

Open Fan.

Toggle ON/OFF.

If the fan starts rotating, it is connected.

# 14. 🚨 Siren

# Working

Sounds an alarm during security events.

Triggered by sensors or manual commands.

**How to Check**

Activate the Siren from the Home Gateway.

If it changes to the active state, it is functioning correctly.

# 15. 📷 Webcam

# Working

Provides live monitoring of the house.

Supports remote surveillance.

**How to Check**

Open Webcam.

Verify it is registered with the Home Gateway.

In IoT Monitor, ensure it is online.

# 16. 🚪 Smart Door

# Working

Opens and locks remotely.

Improves home security.

How to Check

Open Door.

Toggle:

Lock
Unlock

If the door state changes, it is working.

# 17. 🪟 Smart Window

# Working

Opens or closes remotely.

Can respond automatically to environmental conditions.

How to Check

Open Window.

Change its state.

If it opens/closes in the simulation, it is connected.

# ✅ How to Verify the Entire Network

**Method 1: Link Indicators**

Green triangles indicate an active connection.

Red indicates a disconnected link.

**Method 2: Ping Test**

From the Laptop:

Desktop → Command Prompt

ping <Gateway IP>

**Example:**

ping 192.168.25.1

You should receive:

Reply from ...
Method 3: DHCP Verification

Laptop

Desktop → IP Configuration

Click DHCP.

Expected:

IP Address

Subnet Mask

Default Gateway

DNS Server

are assigned automatically.

# 👨‍💻 Developed By

**Muhammad Nabeel**

**University Final Year / Networking Project**
