# Extending Your Network

## Port Forwarding Intro
* Intranet, those on the network being able to acccess a computer on the network, private ip address
* If admin wants info to accessible to public, they need to use port forwarding, have to use the public IP address

## Firewalls 101
* Device/software within a network to determine what traffic is allowed to enter and exit
  * Where is the traffic coming from?
  * Where is the traffic going to?
  * What port is the traffic for?
  * What protocol is the traffic using?
* Peform inspection to see where things are going
* Can be device or software
* They can be stateful or stateless
* Happens in layer 3, 4 of OSI Model

### Stateful Firewall
* Uses all information rather than inspecting an individual packet

### Stateless Firewall
* Uses a static set of rules to see if packets are allowed, indivdual packets

## VPN Basics
* Virtual Private Network
* Technology that allowes devices on seperate networks to communicate securely over the internet in a tunnel

### VPN Technologies
* PPP: simmilar to ssh, must have private key and cert to connect, not routable, encrypts data
* PPTP: Point To Point Tunneling, allows data from PPP to travel and leave a network
* IPSec: encrypts data using the IP framework, harder to set up

## Routers
* dedicated devices for routing

## Swithces
### Layer 2 Switch
* used for data link layer

### Layer 3 Switch
* Used for network switch, used for virtual lan
