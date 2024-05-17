
some applications:
social edia
games (DOTA MENTIONED WTF IS A SHORT GAME)

### How do we create a network app?

2 main architectural standards:
Client-server model
peer-to-peer architecture

A. Client-Server Model
- Server
	- Always-on host; called the server
	-  fixed/permanent adrress: ip address
	- often in data centers
		- normally used to house plenty of hosts and servers
- Clients
	- communicate with server
	- may have dynamic ip addresses
	- do not communicate directly with each other 
- client and client dont communicate directly with each other

B. P2P
- no alwayspon server
- no reliance on data servers
- arbitrary end systems directly communicate
- peersrequest service from peers.
- no passing thru a dedicated servber
- self scalability - new peers bring new service cpaacityt, as well as new service demands
	- file sharing like bitTorrent
- peers are intermittently connected and change ip addresses
- complex management

### Processes COmmunicating 

Process: programs running within a host, an end system
	when program do same end system, that is called iunter-rpocess communicaiton
 processes in different hosts communicate via exchanging messages
 
Client process: process that initiates comnciuatung
server process: process that needs to be contacted 

### Sockets

- process sends/receives message to/from its socket
- software interface sends sockets
- process is house, socket is door
- socketr analogues to door 
	- sending process shoves message out its door 
	- sending process relies on transport infrastructure on other side of door
	- two sockets invovled one on each side

### Addressing process
- to receive messages, process must have identifier
- host deivec has unique 32-biut ip adrersses
- Q: does IP address of host on which process runs suffice for indethifgyh tns he process
	- A: no, many processes can be running on same host
- Identifier includes both IP address and port numbers associated with process on host
- Example: port unmbers:
	- Http server: 80
	- mail server : 25
- to send http messages to gaia.cs.umass.edu web server
	- jkasbd

### Application Lyaer protocols

1. defines tyes of mnessages excvahnged
	- request repsosne
2. message sytnax
	- fields in msasges and how they are defined
3. messag semantics
	- onfn

HTTP hyper texttransfer protocol
	client-server model

htttp
- client server model
- uses web address as a reference to a webserver
- uses tcp
- two types:
	- two types of connections:
		- non persistent one object sent over tcp connection
		- persistent mkultiple objects over single tcp conneft - default modei

webserver: streos wevb server softwarera nd websites componetn flkes

https: erquest response
	reqeust:
	![[Pasted image 20240516082426.png]]
		get
		post
		head
		put
	response
	![[Pasted image 20240516082441.png]]
		200 OK
		301 moved permanently
		400 bad request
		404 not found

HTTPS Cookies
- http GET/response nteraction is stateless
- No notion of multi-step exchanges of HTTP messages to complete a Web "transaction"
- No need for client/server to track state of multi-step exchange
- all http requests are indepenednt 
- no need for client/server to recover 

four components
cooke hieader line of http response mssage
cookie header line in enxt http request message
cookie file kept on user's host, maanged by users browswer
back end database at website

![[Pasted image 20240516083937.png]]

WHat cookies can be used for:
- authorization
- shopping carts
- recommendations
- user session state (web email)

![[Pasted image 20240516084356.png]]

Challenge: how to keep state?
- at protocol endpoints: maintain state at sender/ receiver over multiple transactions
- in messages: cookies in http messages carry state
- 