# Data Communication & Computer Networks Projects

* * * 

## Project 1: Socket Programming
* Implement FTP using Socket to send and receive data
* Functions: PUT, GET, LIST
##### Usage
* Server:
<code>./myftpserver <PORT></code>
* Client:
<code>./myftpclient <SERVER_IP> <PORT> <LIST|GET|PUT> <FILE_TO_GET|FILE_TO_PUT></code>
![Socket](https://github.com/CatherineZHANG0980/Computer-Networking/blob/master/project-1/Socket.png)

* * * 

## Project 2: Erasure Coding Scheme and Multiplexing FTP
* Enhanced FTP with erasure coding scheme for data recovery
* Monitor multiple servers and clients without blocking by select() and multiple thread
* Functions: PUT, GET, LIST
##### Usage
* Server: <code>./myftpserver serverconfig.txt</code>
* Client: <code>./myftpclient clientconfig.txt <list|get|put> <file></code>
 
##### Reference
[Erasure Coding]:https://www.backblaze.com/blog/reed-solomon/
 
* * * 

## Project 3: NAT
* Build an NAT program to forward UDP traffic
* Provide multiple classes of service to difference classes of traffic by Token Buckets
* Environment: 
  * VM A: 2 network interfaces
    * eth0: Virtual, internal network
    * eth1: Department network
  * VM B, VM C: 1 network interfaces
    * eth0: VIrtual, internal network
 * Monitor packets on the NFQUEUE
 * Identify packets matching the criteria by looking up or create NAT entries
 * Modify the packets, i.e. recalculate checksum
 * Decide whether to accept or reject packets
 
##### Usage
 * Run <code>./nat<IP><LAN><MASK><bucket size><fill rate></code> 
 
![NAT](https://github.com/CatherineZHANG0980/Computer-Networking/blob/master/project-2/NAT.png)
