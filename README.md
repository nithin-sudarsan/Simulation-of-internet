# Simulation-of-internet
This topology is a simple simulation of how the real-world internet works

## Networking Devices Used
1. Switches
2. Routers
3. Wireless Routers
4. Servers
5. PCs

## Concepts Implemented
1. Routing Information Protocol(RIP)
2. Dynamic Host Configuration Protocol (DHCP)
3. Domain Name Server(DNS)

![Screenshot of topology](https://user-images.githubusercontent.com/84195790/147956128-9ea584a8-71bb-4866-a795-98ee144cd28d.png)

## Legend
* Orange Area: Edge Wireless-Routers and PCs
* Yellow Area: Routers in the Internet (ISP)

## Explanation
Routers 1 to 16 are all inter-connected and a network is formed which is configured and controlled by organizations such as IANA. Routing Information Protocol (RIP) is implemented in all the sixteen routers as a dynamic routing protocol. In this topology we have used four servers that represent four different websites that are Facebook, Instagram, Cisco and Whatsapp Servers (*All these servers provide dummy websites for simulation purpose*). We use one Server as a DNS server in which the DNS table is stored.

The DNS table is as follows:

| No. | Name | Type | Details |
|-------|--------------------|--------------|----------------|
| 0 | cisco.com | A Record | 36.0.0.10 |
| 1 | facebook.com | A Record | 192.168.1.2 |
| 2 | instagram.com | A Record | 192.168.2.2 |
| 3 | whatsapp.com | A Record | 192.168.3.2 |

We use ten Wireless routers as our edge routers to connect all the 30 PCs (*3 PCs connected to each wireless-router*) to the internet and access the websites that are hosted on the respective servers. The PCs obtain their IP addresses by DHCP impemented on thier respective wireless routers.

## Outcome
The PCs will be able to access the wesites that are hosted on different servers located in different locations by only using the domain names used to each of those servers, hence making it a easier and secure way to access the internet

