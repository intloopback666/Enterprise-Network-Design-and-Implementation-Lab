# Enterprise-Network-Design-and-Implementation-Lab
CCNP Enterprise Lab: Multi-Area OSPF, Redundant Campus Design, IPv4/IPv6, NAT and Network Security


Technologies and Tasks Implemented
Designed an IPv4 addressing plan from the 172.16.0.0/16 private address block using VLSM.
Implemented /30 point-to-point IPv4 addressing using the convention:

10.x.y.0/30
Configured IPv6 addressing for the DMZ and routed point-to-point links.
Built a multi-area OSPF design:
Area 0 — Backbone
Area 39 — Campus User Distribution
Area 108 — Shop-1
Area 112 — Branch/Loopback Network
Area 218 — Finance, Managers, VoIP and Printer Network
Configured OSPF Area Border Routers (ABRs).
Applied OSPF MD5 authentication using CCNP123.
Configured Backbone OSPF hello/dead timers to 5/20 seconds.
Used router loopback interfaces as stable OSPF router IDs.
Configured passive interfaces on LAN and loopback interfaces.
Configured R5 as the Internet edge router.
Implemented NAT/PAT overload for internal users.
Configured primary ISP connectivity through ISP-1.
Configured floating static IPv4 and IPv6 default routes through ISP-2.
Advertised the default route into OSPF from the Internet edge.
Simulated Internet reachability using ISP loopbacks:
8.8.8.8
8.8.4.4
Configured Router-on-a-Stick (ROAS) on R10 for Shop-1 VLAN routing.
Configured DHCP for VLAN 75.
Built redundant default gateways using HSRP.
Configured LACP EtherChannels:
Port-channel10 between Distribution Switches
Port-channel20 between SW13 and SW14
Configured PAgP EtherChannel:
Port-channel30 between SW21 and SW22
Configured VTP version 3 for the campus access/distribution environment.
Configured PVST with root primary and root secondary switch placement.
Implemented PortFast and BPDU Guard on access ports.
Configured DHCP Snooping for user access VLANs.
Configured sticky MAC Port Security with a maximum of one MAC address on required access ports.
Configured VLAN segmentation for:
VLAN 50 — Printers
VLAN 60 — VoIP
VLAN 75 — Shop-1
VLAN 100 — IT
VLAN 150 — DMZ / Web Servers
VLAN 200 — Managers
VLAN 221 — Finance
VLAN 301/302/303 — User access floors
Applied ACL policies to:
Permit IT VLAN management access through SSH.
Permit user access to DNS, DHCP, Active Directory, DMZ web services, and the Internet.
Restrict direct user-to-user VLAN access.
