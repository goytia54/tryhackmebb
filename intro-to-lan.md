# Intro to LAN
* Local Area Networks (LAN) 

## Topologies

### Star (Most Common)
* Indivdiually conntected via switch or hub
* Scalable, very easy to add devices
* More expensive
* Harder to trouble shoot, switches don't die often

### Bus 
* Tree topologies
* Devices using the same wire
* Hard to trouble shoot
* Easier, cost effective

### Ring
* Token topologies
* connected for a loop
* Sending data around the loop
* One cut of cord, breaks network, might be a mesh network

### Router
* Connects networks
* sit at edge of networks to bring in internet
* Routes them to different paths

### Switches
* Aggregate devices using ethernet

### Switch
* Connect to a router
* Connects to multiple devices as well so we can spread out the i/o from router

## Subnetting
* Splitting up a network into smaller networks
* Use IP address
* Network Address: start of network
* Host Address: used to identify a device on the subnet
* Default Gateway: default gateway

## ARP Protocol
* Address Resolution Protcol  
* Tech responsible for devices identifying itself
* Uses a cache

## DHCP Protocl
* Dynamic Host Configuration Protcol
* Discover: can I get an IP address
* Offer: sure here you go
* Request: I will use this IP address
* Ack: I have you down for this IP address
