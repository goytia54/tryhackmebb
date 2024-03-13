# Packets and Frames
* Small peices of data, form together to make a message
* Frame is at layer 2 data link (Envelope of data, no ip data)
* Packet, efficient way to send data (has ip data)

## Types of Packet Headers
* Time to live: how long it will live on the network so it does not clog up
* Checksum: integrity checking for tcp
* Source Address: where data is from
* Destination Address: where data is being sent to

## TCP-IP model
* Application, Transport Internet, Network Inteface
* Summary of OSI model

### Important TCP Packet Headers Continued
* Source Port
* Destination Port
* Source IP
* Destination IP
* Sequence Number: a random number
* Acknowledgment Number: sequence number + 1
* checksum: number to check data is not corrupted
* data: bytes of the fil
* flags: how devices should handle data for different devices

### Three Way Handshake
* SYN: intial packet sent to device during handshake, initiate connection
* SYN/ACK: packet sent from receiving device
* ACK: acknowledge packet received from receiving device
* DATA: sending of data
* FIN: closing the connection cleanly
* RST: packet will end all connection

## UDP/IP
* Another protocol to communicate
* Stateless, no three way handshake

### UDP packet headers
* TTL
* Source Address
* Destination Address
* Source Port
* Destination Port
* Data

### Different Type of Ports
* FTP File transfer Protocol (21)
* SSH Secure shell (22)
* HTTP Hypertext transfer protocol (80)
* HTTPS Hypertext transfer protocol secure: uses encryption (443)
* SMB Server Message Block (445) share devices like printers
* Remote Desktop Protocol (3389)
