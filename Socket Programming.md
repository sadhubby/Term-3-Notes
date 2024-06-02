#csnetwk 

## What is a socket
	
One end point of a two wat communication link between two programs running on the network
	Palaging meron port number so TCP layer can identify the application. 2 types:
	Connectiod orented sockets
		source ip addres
		source port number
		dest IP address
		dest port number
		 uses TCP
	Connectionless sockets
		dest IP address
		dest port number
		 uses UDP
		 adrenaline in my soul

1. Server runs on a specific computer and has a socket that is bound to a specific port number
	- server 
3. server accepts tehec onnection
	1. upon acceptance the server gets a new socket bound to the same local port and has its remote nepoint set to the aadress and port of the client
	2. socket is successfully created on the client side and the client can use the socket to commjunicatie htbe sjervber

check pdf latur

## Socket Programming

Socket classes are used tor epresent the connection between a client prograsm and a server program
The java.net package provides two classes:
	socket - client-side connection
	ServerScoket - server-side connection

Goal : learn how to build client/server applications that communicate using sockets
Socket : door between application process and end-to-end transport protocol

2 socket types for two transport services:
1. UDP: unreliable datagram
2. TCP: reliable, byte stream-oriented


## Socket Programming with UDP

UDP: no persistent connection established between client and servetr
	no handshaking before sending data
	sender explicitly attaches IP address and port no. to each packet
	Receiver extracts sender UP and prt no. from received packet
transmitted data may be lost orr ecieved out-of-order
Application standpoint: udp provides unreliable transfer of groups of bytes called datagrams between client and server processes
AF = address family
AF_INET = address family of ipv4
SOCK_DGRAM = datagram socket
OS assigns port number automatically

*check PDF for syntax in Python*

## Socket Programming with TCP

Client must contact server
	server process must first be running
	server must have created socket that welcomes client's contact
Client contacts server by
	creating tcp socket. specifying ip address port number of pserver process
	when client creates socket:
		client TCP establishes connection to server tcp

When conracted by client, server TCP creates new oscjket for server process to communicate with that particular client
- allows server to talk with multiplke clients
- client source port no. and ip address used to distinguish clients 

Application viewpoint
- TCP provides reliable in-order- byte streamn "pipe" between client and server processes

UDP creates socket using SOCK_DGRAM while TCP creates socket using SOCK_STREAM
