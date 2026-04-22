# Multi VLANs Network Design With DHCP And DNS Server Configurations
This project demonstrates the implementation of a multi-VLAN network using Router-on-a-Stick, with DHCP for dynamic IP assignment and a DNS server for domain name resolution.

# key concepts used
VLAN(virtual LAN)

inter-VLAN routing(using router on a stick)

DHCP(dynamic host configuration protocol)

DNS(domain name system)

# Network Design

## Router on a stick
There are three switches. each switch is connected to two VLANs (VLAN 10 and VLAN 20) . these three switches are connected to a central switch which is then connected to a router.

the router makes communication between VLAN 10 and VLAN 20 possible by using concept (router on a stick) . Separate virtual interfaces are configured for each VLAN using a single physical interface.

Fa0/0.10 → VLAN 10

Fa0/0.20 → VLAN 20

these virtual interfaces acts as gateways for VLAN networks.

## Dhcp 
router is configured as a DHCP server.

separate DHCP pools are configured for each VLAN.

## DNS
A server is configured a DNS server by turning on its DNS services.

Domain names with their IPs are entered.

Domain Name                                           IP Address   

| ------------------------------------------------- | ------------ |

| [www.campusnet.local](http://www.campusnet.local) | 192.168.10.4 |

| [www.learnhub.local](http://www.learnhub.local)   | 192.168.20.6 |

| [www.techhub.local](http://www.techhub.local)     | 192.168.10.5 |

# Conclusion
This project successfully demonstrates how to:

Segment a network using VLANs

Enable communication using Router-on-a-Stick

Automate IP assignment with DHCP

Resolve domain names using DNS


If you have any queries, feel free to reach out. 

