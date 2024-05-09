
Internet
	interconnected ISP that provides connection using internet protocols - tcpip
	network of networks

ISP 
	Internet service provider
	organization that provides services to access internet

protocol
	governs all communication activities on internet
	defines format, order of messages, etc.

network edge
	gadgets we use everyday, i.e., computers, phones, tablets, etc.
	called hosts
	clients that request and receive service
	server that provides service
		access network - network that connected edge device
		physical media - wired or wireless communication links

network core
	set of router that are interconnected to form a network

2 types of packet switches: Switch and Router
	Switch - facilitates the sharing of resources by connecting all the devices
	router - connects multiple switches and their respective networks to form an even larger network

![[Pasted image 20240509074058.png]]

Modem
	modulator-demodulator
	it transmits data by modulating and demodulating carrier signals for encoding and decoding digital information

ACCESS NETWORKS: 
cable based access network
	residential internet access
	signals are sent on a cable different frequencies and don't interfere with each other

Frequency Division Multiplexing (FDM)
	different channels transmitted in different frequency bands

Digital Subscriber Line (DSL)
	use existing telephone line
	data over DSL phone line
	voice over DSL phone line goes to telephone net
	voice, data transmitted at different frequencies over dedicated lien to central office to DSL access multiplexer
	better downstream than upstream

Wireless Area Networks (WANs)
	shared wireless access network which connects end system to router via base station or access point
	Wireless Local Area Network WLAN
		Wi-fi
	wide area cellular access network
		4g 5g

Enterprise network
	home networks in steroids
	mix of wired and wireless link technologies, connecting multiple switches and routers

Packet switching:

packet swithces
	routers and switches forward packets or chunk of data vbetween hosts and devices
	L bits / R bits per second

store and forward
	transmitted birt will be received and gathered up at the receiving end of the link until the full packet has been received 
	once packet has been fully received it will be forwarded onto the next hop and so on 

queueing delay, loss
	queueing occurs when work arrives faster that it can be serviced
		ex: two network edges send packets 100 mb/s but router can only do 1.5 mb/s
	packet queue are going to form at the routers outbound link
	if an arriving packjet finds no memeory it wish to bes tored, a packet is going to be dropped or last

circuit switching
	end to end resources allocated to, reserved for call between source and destination
	theres no delay other than propagation delay and no loss of data because link capacity has been reserved for exclusive use of the call.
	circuits are dedicated resources and not use by any others 
	not that efficient kasi nasasayang lang rin resources

FDM and Time Disivion Multiplexing
FDM
	each call is allocated one of those narrow bands and can transmit at a full rate allwed by that band
TDM
	can transmit only during allocated time but can transmit higher frequency call

processing dfelay
	delay associated with forwarding table look up, forwarding a packet thru switch
queueing delay
	amount of time that a packet must waty to queue at an output linkl
	congestion level of the router
transmission delay
	certain amount of time for all the bits and packets to be pushed into outgoing link
propagation delay
	amount of time it takes from when a bit first enters the sending side if oteh liunk until exits the receiving side 

d_nodal = d_proc + d_queue + d_trans + d_prop

