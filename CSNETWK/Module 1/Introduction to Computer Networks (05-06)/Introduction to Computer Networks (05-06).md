
==**Networks in our Daily Lives**==
	Allows us to communicate easily like email and messaging apps
	Made our lives more convenient, i.e., purchasing goods from homes
	Downsides:
		data privacy and loss
		vulnerability to cyber security
		tendence to misinformation and disinformation
		
==**The Internet**==
Billions of connected devices:
	Hosts = end systems
	Running network apps at Internet's edge
Packet switches: forward packets or chunks of data, two types:
	Routers and switches
	Router: Circle with X
	Switches: Square with X
Communication links:
	fiber, copper, radio, satellite
	transmission rate is called ==bandwidth==
Internet is the "network of networks"
Protocols are everywhere
	Protocols control sending, receiving of messages

CHECK POWER POINT HERE
LAST SLIDE IM BNACK IN IS INTERNET STRUCTURE

==**Internet Structure**==
Network edge
	Hosts clients and servers, where servers are often in data centers
Access networks, physical media:
	Wired and wireless communication links 
Network core
	Interconnected routers
	Network of networks
To connected end systems to edge of router:
	There are residential (LAN), enterprise (school or company) and mobile carrier access networks (cellular)
	
==**Access Networks: Cable based access**==
1. Frequency Division Multiplexing (FDM)
   Cable network
   Different channels transmitted in different frequency bands (think of FM radio)
   Asymmetric, faster down-stream than up-stream
   Consumers of data than producers of data
   30 to 1 gbps downstream
   30 to 100 mbps upstream

==**Access Networks: DSL**==
Digital Subscriber Line
	not sharing transition or bandwidth
	Asymmetric 
	24-52 mbps to downstream
	3.5-16 mbps dedicated upstream
Use existing telephone line to central office DSLAM

==**Wireless Access Networks**==
shared wireless access via base station aka access point
1. WLAN 
   Typically within our around the building
2. Wide-area cellular access networks
   Provided by mobile, cellular network operators (10's km)
   10's mbps
   5G cellular networks

==**Enterprise Network**==
Home network on steroids
Used by companies, universities, etc.
Mix of wired and wireless link technologies connecting mix of switches and routers

==**Host**==
Host's sending function
	- Takes application message
	- breaks into smaller chunks known as packets, of length L bits
	- transmits packet into access network as transmission rate R
	- Link transmission rate, link capacity, or aka link badwidth
packet transmission delay = time needed to transmit L-bit packet into link 
= L (bits) / R (bits per sec)

**Network Core**
Mesh of interconnected routers
Packet switching: hosts break messages into packets
	Forward packets from one router to next, across links on path from source to destination

**Packet Switching**
Queueing delay and loss. If there are too many packets, going at too fast a rate, some packets will fail

**Two Key Network-core functions**
	Forwarding: Local action
		move arriving packets from router's input link to appropriate router output link
		Look for destination address in forwarding data then transmits data to output link
		that houses the destination
	Routing: Global action
		determine source-destination paths taken by packets routing algorithms
		Uses algorithms to find end-to-end networking path

**Circuit Switching**
End-end resources allocated to, reserved for "call" between source and destination
![[Pasted image 20240506082633.png]]
Diagram:
![[Pasted image 20240506082647.png]]

**Circuit Switching: FDM and TDM**
1. Frequency Division Multiplexing (FDM)
   electromagnetic frequencies divided into narror frequency bands
   Each call allocated its own band can transmit at max rate
2. Time Division Multiplexing
	time divided into slots
	each call allocated periodic slots can transmit at maximum rate of wider freq bands

Hosts connect to internet via access Internet Service Providers (ISPs)
	wired or wireless 
	Residential, enterprise ISPs
Access ISPs in turn must be interconnected
	So that any two hosts can send packets to each other
Resulting network of networks is very complex
	Evolution was driven by economics and national policies rather than performance considerations

To connect millions of access ISPs:
	connecting each ISP to each other will give an O(N^2) connection
	Instead connect each access ISP to one global transit ISP
	But if one global ISP is viable ISP, there will be competitors, and THEY have to be connected to each other
		Peering link is the answer
	And regional networks may arise to connect access nets to ISPs

**Performance**
How do packet loss and delay occur?
	packets queue in router buffers
	packets queue, wait for turn
Packet delay: four sources
Processing delay, queueing delay, transmission delay, propagation delay

d_nodal = d_proc + d_queue + d_trans + d_prop

d_queue = congestion level
d_trans = certain amount of time for outgoing bits, determined by packet L
d_prop = amount of time it takes for bit to enter sending side till it finds exit side

"Real" Internet delays and routes
1. Traceroute program provides live or real time delay measurement from source to router along end to end path towards destination

Packet Loss
	queue (aka buffer) preceding link in buffer has finite capacity

Throughput 
	rate (bits / time unit) at which bits are being sent from sender to receiver
	can be instantaneous or average

**Standards**
Internet standard - tested specification that is useful to and adhered to
Internet Draft - working document with no official status
	Request For Comments

**Organizations**
Internet Engineering Task Force (IETF)
	standards of internet
	upholds ethical standards
Institute of Electrical and Electronics Engineers (IEEE)
	501, exempted from federal income tax
	
	