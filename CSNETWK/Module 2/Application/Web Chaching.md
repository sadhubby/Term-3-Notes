
Goal: satsify client requeqst without involvingorigin server
decrese the load on origin server

browser sends all http requests to chace
	if object in chace: achace returns object to client
	else: cache request object from origin server, caches received object then returns object to client

why web caching?
web cache acts as both client and server
	server for iriginal requesting client
	client to origin server
server tells cache about objects allowable caching in response header

reduces response time for client requestiost since aacahce is closer toclient 

email application protocols
- store and forward amethod of sending, storing and retreiving electronic messages
- relise on threee separate protocols for operation
	- SMTP - simple mail transfer protocol (sending)
	- POP - Post Office Protocol (retrievcing)
	- IMAP - Internet Message Access Protocl (retrieving)

DNS 
Domain Name SYstem
Services
- hostname to ip address translation
- host aliasing
- mail server aliasing 
- load distribution
- when a particular host name deployed duplicated web servers

Root DNS Servers
13 logical root name servers worlwide each server replicated many times
official, contant of last resort by name that can not resolve name
incredible important internet function
	internet countlyt function wihtout 
	DNSSEC - provides sercuitityu
ICANN Internet corporation for assigned named nad numvers

TLD and Authoritative Servers
- Top Level Domain Servers
	- reponsielble ofr .com.org.net.edu.jobs and all contry top level domains (the country domain)
	- bnetwokr solutions authortiateive registryu
- authortiate dns server
	- orginazations own dns server

Local DNS name server
	when host makes dnms query, it is sent to its local dns server
		local dns server returns reply answer
			- from uits local cahce of recent name to address translation paiurs
			- forwarding qrueqohjasdbjbasdmbas

DNS name resolution
Iterated query: 
- contracted server replies with name of server to contact
- i dont know this name but ask this server

Recvusierve query: 
	puts burnde of name resolution on contact name server
	heavy load at upper levels of hierarchy

![[Pasted image 20240520081843.png]]


![[Pasted image 20240520082058.png]]




![[Pasted image 20240520082340.png]]
![[Pasted image 20240520082854.png]]
![[Pasted image 20240520083252.png]]
![[Pasted image 20240520083940.png]]
![[Pasted image 20240520084017.png]]
![[Pasted image 20240520084042.png]]
![[Pasted image 20240520084147.png]]
![[Pasted image 20240520084309.png]]
![[Pasted image 20240520084419.png]]
![[Pasted image 20240520084607.png]]
![[Pasted image 20240520084702.png]]
![[Pasted image 20240520084732.png]]
![[Pasted image 20240520084908.png]]
![[Pasted image 20240520085042.png]]
![[Pasted image 20240520085144.png]]
![[Pasted image 20240520085243.png]]
![[Pasted image 20240520085251.png]]
![[Pasted image 20240520085403.png]]
