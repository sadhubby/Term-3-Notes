
- Network Protocol
	- All communication activities on the Internet are governed by protocols
	- Protocols define the format, order of messages sent and received among network entities and actions taken on message transmission and receipt

- Layered Network Architecture
	- uses a layered approach to process data from one layer to another
	- provides modularity to manage complex systems
	- has the ability to change implementation of service without affecting other components of the system

### OSI Architecture
- Open Systems Interconnect
- Also known as: OSI Layer, OSI Model, OSI Reference Model
- Provides a detailed set of standards for describing a network
- Framework for the development of network protocol standards
- Defines and codifies the concept of layered network architecture

7 Layers of the OSI Architecture

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


### TCP/IP Suit
- Transmission Control Protocol / Internet Protocol
- The Internet Protocol
- Framework used to form the set of communication protocols used on the Internet

4 Layers of the TCP/IP Suite

Layer 4: Application Layer
- provides process-to-process data exchange
Layer 3: Transport Layer
- handles host-to-host communication
Layer 2: Internet Layer
- provides internetworking between independent networks
Layer 1: Network Interface layer
- contains communication methods for data





OSI vs TCP/IP

| OSI Layers                             | TCP/IP Suite Layers |
| -------------------------------------- | ------------------- |
| Application<br>Presentation<br>Session | Application         |
| Transport                              | Transport           |
| Network                                | Internet            |
| Data Link<br>Physical                  | Network Interface   |

### Encapsulation and Decapsulation

1. Encapsulation
	- packs data into a suitable form to be transmitted over the network
	- Data has protocol information i.e., headers and trailers added to it as it is passed down through the OSI or TCP/IP layers
2. Decapsulation
	- Reverses the process by removing the protocol information, so that the original data can be read data can be read by the destination device

![[Pasted image 20240514223553.png]]

![[Pasted image 20240514223604.png]]
