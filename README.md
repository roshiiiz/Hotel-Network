Multi-Floor Hotel Network Configuration
This repository contains the configuration for a multi-floor Hotel network using three routers to connect each floor. The network is designed with specific VLANs and subnets for different departments on each floor and employs OSPF as the routing protocol. Below is a detailed description of the network setup:

Network Topology
Routers:
Three routers connect the three floors.
All routers are interconnected using serial DCE cables.
The network between the routers uses the following subnets:
10.10.10.0/30
10.10.10.4/30
10.10.10.8/30

Switches:
Each floor has one switch.
WiFi Networks:
Each floor has WiFi networks connected to laptops and phones.

Printers:
Each department has its own printer.
Floor-wise Network Configuration


1st Floor

Reception:
VLAN: 80
Subnet: 192.168.8.0/24

Store:
VLAN: 70
Subnet: 192.168.7.0/24

Logistics:
VLAN: 60
Subnet: 192.168.6.0/24

2nd Floor


Finance:
VLAN: 50
Subnet: 192.168.5.0/24

HR:
VLAN: 40
Subnet: 192.168.4.0/24

Sales:
VLAN: 30
Subnet: 192.168.3.0/24

3rd Floor


Admin:
VLAN: 20
Subnet: 192.168.2.0/24

IT:
VLAN: 10
Subnet: 192.168.1.0/24

Routing and Services


Routing Protocol:
OSPF is used to advertise routes.

DHCP:
Each router is configured as a DHCP server to dynamically assign IP addresses to devices on their respective networks.

Communication:
All devices in the network can communicate with each other.

Remote Login:
SSH is enabled on all routers for remote login.

This configuration ensures a scalable and efficient network with proper segmentation and routing for a multi-floor office environment.