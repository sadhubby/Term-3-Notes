#### ==Protocols==
accepted or established set of procedures, rules or formal specifications governing specific behavior or language
	code of conduct
	ex: specific dress protocol for fine dining restaurant

all communication activities on the internet are governed by protocols


network protocols are like human protocols
	formal specification that defines how devices are to behave or communicate with each other
	how data are to be formatted, maintained, transmitted and received between devices
	specifies vocabulary and rules of data communication
	vital that the source and destination and any other devices on the network all use the same protocol

#### ==Open Systems Interconnect (OSI) architecture==

Keywords: 
- Network Architecture
	- formal logical structure (framework) that defines how network devices and software interact
	- protocols, message formats, standards required for interoperability
- Interoperability
	- degree in which software and hardware products developed by different vendors are able to communicate successfully with each other over a network

OSI architecture history
1970s: time where there was no network structure
ISO developed the seven layer OSI architecture in 1978

OSI provides a detailed set of standards for describing a network
Frame for development of network protocol standards
defines and codifies the concept of layered network architecture

7 layers:
	1. Application
	2. Presentation
	3. Session
	4. Transport
	5. Network
	6. Data Link
	7. Physical

As new technologies become available for one layer; they can be implemented without affecting the operation of other layers

OSI also allow helps reduce design complexity of a network

Services are independent from other layers

7 layers:
	7. Application
	   - contains protocol that users need to be able to communicate over a network
	6. Presentation
	   - data formatting and makes sure data is in a usable format
	5. Session
	   - establishment and maintenance, responsible of ports and sessions
	4. Transport
	   - responsible for end to end connections between hosts (end user device, transmission protocols
	3. Network
	   - routing of packets across a network
	2. Data Link
	   - handles the errors that result from physical transmission data
	1. Physical
	   - transmission of bit patterns over a comms channel

![[Pasted image 20240509082939.png]]

On a software level: application, presentation, session, transport
On a hardware level: network, data link, physical

**Application or Service Oriented Layers**: Application, Presentation, Session
**Delivery and Verification Services**: Transport
**Communication or Network-Oriented Layers**: Network, Data Link, Physical

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

Half duplex - one direction at a time
	ex: walkie talkies
full duplex - simultaneously
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


