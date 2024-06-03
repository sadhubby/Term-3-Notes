
# Protocol
- Network Protocol
	- All communication activities on the Internet are governed by protocols
	- Protocols define the format, order of messages sent and received among network entities and actions taken on message transmission and receipt

- Layered Network Architecture
	- uses a layered approach to process data from one layer to another
	- provides modularity to manage complex systems
	- has the ability to change implementation of service without affecting other components of the system

# OSI Architecture
- Open Systems Interconnect
- Also known as: OSI Layer, OSI Model, OSI Reference Model
- Provides a detailed set of standards for describing a network
- Framework for the development of network protocol standards
- Defines and codifies the concept of layered network architecture
Keywords: 
- Network Architecture
	- formal logical structure (framework) that defines how network devices and software interact
	- protocols, message formats, standards required for interoperability
- Interoperability
	- degree in which software and hardware products developed by different vendors are able to communicate successfully with each other over a network


# 7 Layers of the OSI Architecture

Layer 7: Application Layer 
- contains protocols that users need to be able to communicate over a network
Layer 6: Presentation Layer
- establishes data formatting, data compression and data encryption
Layer 5: Session Layer
- common functions include establishment, maintenance and termination
Layer 4: Transport Layer
- responsible for end-to-end connections between hosts
Layer 3: Network Layer
- provides a means of routing of packets across a network
Layer 2: Data Link Layer
- handles the errors that result from the physical transmission media
Layer 1: Physical Layer
- responsible for the transmission of bit patterns over a communications channel

On a software level: application, presentation, session, transport
On a hardware level: network, data link, physical

**Application or Service Oriented Layers**: Application, Presentation, Session
**Delivery and Verification Services**: Transport
**Communication or Network-Oriented Layers**: Network, Data Link, Physical

## OSI, expounded

Application
	consists of protocols that define specific user oriented applications
	functions include message handling, file sharing, DB access
	ex: HTTP 0 Hyper Text Transfer Protocol

Presentation
	formatting and  translating, prepares data for transmission
	ex: ASCII conversion, 

Session
	provides coordination between communicating processes between nodes
	controlling ports and sessions
	reestablishing connection in the event a failure occurs
	responsible for enforcing rules of full and half duplex

- Half duplex - one direction at a time
	ex: walkie talkies
- full duplex - simultaneously
	ex: landline phones or mobile phones

Transport
	responsible for end to end connection between hosts
	ex: Transmission control protocol (TCP)
	ensures packets arrive early or on time

Network
	end to end routing or switching
	resolves all inherent problems related to data transmission between heterogenous networks
	ex: internet protocol (IP), IPv4 IPv6

Data Link 
	handles error from physical transmission by detecting and possibly correcting
	ex: Ethernet

Physical
	responsible for transmitting raw bits over a link
	translate the bit stream into signals
	ex: Ethernet

---- 
# TCP/IP Suit

- Transmission Control Protocol / Internet Protocol
- The Internet Protocol
- Framework used to form the set of communication protocols used on the Internet

# 4 Layers of the TCP/IP Suite


Layer 4: Application
	- Similar to OSI application layer
	- communication, end users interact with email or messaging. 
	- combination of application, presentation and session layer of OSI
Layer 3: Transport
	- Defined by two protocols:
		- Transmission Control Protocol - TCP
		- User Datagram Protocol - UDP
	UDP is about fast
	TCP is about precision and accuracy
	
Layer 2: Internet 
	- internetworking 
	- primary protocol is IP 
	- transfers user messages from source host to destination host
	- uses internet or IP addresses
Layer 1: Network Interface
	- connects a host to local network hardware
	- makes connection to physical medium

# TCP vs UDP
| ==**Transmission Control Protocol (TCP)**==                                          | **==User Datagram Protocol (UDP)==**                               |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------ |
| Connection oriented                                                                  | Connectionless                                                     |
| Provides reliable data transmission via end-to end<br>error detection and correction | Provides unreliable datagram service                               |
| Retransmits any data not received by destination                                     | Does not retransmit any unreceived data                            |
| Guarantees data are transferred across a network<br>accurately and in proper order   | N/A                                                                |
| Guarantees against data duplication between<br>sending and receiving devices         | N/A                                                                |
| Telnet<br>File Transfer Protocol (FTP)<br>Simple Mail Transfer Protocol (SMTP)       | Trivial File Transfer Protocol (TFTP)<br>Domain Name Service (DNS) |
# OSI vs TCP/IP

| OSI Layers                             | TCP/IP Suite Layers |
| -------------------------------------- | ------------------- |
| Application<br>Presentation<br>Session | Application         |
| Transport                              | Transport           |
| Network                                | Internet            |
| Data Link<br>Physical                  | Network Interface   |

# Encapsulation and Decapsulation

1. Encapsulation
	- packs data into a suitable form to be transmitted over the network
	- Data has protocol information i.e., headers and trailers added to it as it is passed down through the OSI or TCP/IP layers
2. Decapsulation
	- Reverses the process by removing the protocol information, so that the original data can be read data can be read by the destination device

![[Pasted image 20240514223553.png]]


| Layer             | Units               |
| ----------------- | ------------------- |
| Application Layer | messages or stream  |
| Transport Layer   | segments            |
| Network Layer     | datagrams or packet |
| Data Link Layer   | frame               |
| Physical Layer    | bits                |

![[Pasted image 20240514223604.png]]
