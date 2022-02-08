Draw all the layers of the OSI network stack and the TCP/IP reference model showing how they are related

> OSI
>
> Layer 7 Application
>
> Layer 6 Presentation
>
> Layer 5 Session
>
> Layer 4 Transport
>
> Layer 3 NetWork
>
> Layer 2 DataLink
>
> Layer 1 Phisical
>
> TCP/IP
>
> Layer 7 Application
>
> Layer 4 Transport
>
> Layer 3 NetWork
>
> Layer 2 DataLink
>
> Layer 1 Phisical

***

Give the name (not just number) of the layers of the network stack described below: 

i. This layer exists at end hosts and takes care of reliability (if any) by ensuring lost data is retransmitted and all data arrives reliably in order. 

> Transport Layer

ii. This layer would be used by programmers to open and close sockets and to send data from one machine to another.

>  Transport Layer

iii. This layer contains the routing protocols OSPF and RIP. 

> NetWork Layer

iv. This layer would move data from somewhere in a subnetwork to another place in the same subnetwork. 

> DataLink Layer

v. This layer would move data across the network from the initial source machine to the final destination machine.

> Phisical Layer

***

UDP features: [12 marks] 

i. How do the source and destination port allow multiplexing and demultiplexing of traffic? (5 marks) 

> Multiplexing(MUX):
>
> Combing serveral streams of data into a single stream
>
> Demultiplexing(DeMUX):
>
> A stream of data is separated out into its individual components

ii. How do the sender and receiver use the checksum field in the UDP header (you do not need to include details of the calculation itself)? (5 marks) 

>For Sender:
>
>addition of segment contents
>
>For Receiver:
>
>compute checksum of received segments and check if computed checksum equals checksum filed value

iii. Traffic is sent from 144.32.124.4:1243 to 144.32.145.5:90 (the numbers after the : are port numbers. If 144.32.145.5 wants to reply, what will it use as the destination IP and port? (2 marks)

> Destination IP: 144.32.124.4
>
> Port: 1243

***

Describe the role of congestion control and flow control paying attention to which window is used for which mechanism and any header fields you think are relevant. (You do not need to describe mechanisms for congestion control).

> rwnd: flow control (not too fast for reciever)
>
> cwnd: congestion control (not too fat for network)

What is meant by AIMD (additive increase multiplicative decrease) in the TCP congestion window?

> AIMD means additively increase window size until loss occurs then cut window in half whick make the behavior like tooth

 Are the following IP addresses valid? If not, why not? [3 marks] 

i. 127.0.0.1 

> yes, it is valid

ii. 132.2.256.2 

> no, IP adress is 8 bit in dotted decima,from 0 to 255

iii. 133.23.1.2.1

> no, only two types, IPV4 and IPV6, there can be 5 dots in IP adress

***

Explain how do source host, destination host and routers respond to traceroute command. 

> source sends series of UDP segments to desination, and  router discards datagram and sends source ICMP message

What are the implications of this frame size

> To ensure the transmitting station is still transmitting long enough for a corrupted signal to be detected

In Carrier Sense Multiple Access/Collision Avoidance, give the full names and briefly explain the roles of ACK, RTS and CTS.

> RTS : request to send
>
> CTS: clear to send
>
> ACK: acknowledge character
>
> avoid data frame collisions completely using small reservation packets 