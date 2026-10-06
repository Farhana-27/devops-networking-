# Notes
## Intro to Networking Fundamentals 
A. Overview of computer netowrks and ther importance in modern infrastucture & Devops 

B. Network basics/Types of Networks -> LAN, WAN etc.

C. Key networking components -> Routers, Switches, Firewalls 

D. IP addressing (IPv4 & IPv6)

E. MAC addresses 

F: Ports and Protocols (TCP, UDP)

### A: Computer Networks 
- Definition -> connecting devices to share information
- Purpose -> Communication and resource sharing 
#### Core Types of Computer Networks
1. LAN (Local Area Network) e.g. Home Wi-Fi 
2. WAN (Wide Area Network) e.g. Internet 
#### Importance in modern infrastructure 
- Foundation -> enables communication between devices 
- Resource sharing -> facilitates sharing of files, printers and more 
- Internet Functionality -> critical for browsing, streaming and communication 
- Application support -> backbone of app connectivity and data transfer 
#### Networking in DevOps 
- Server Interaction -> Enables communication between servers and applications
- Deployment -> Critical for launching and updating applications 
- Management -> Crucial in monitoring and managing infrastructure 
- Optimisation -> Enhances troubleshooting, performance and scalability 
### B: Network basics/Types of Networks -> LAN, WAN etc.
#### Types of Networks 
1. LAN 
- - Small area, like a home or office 
- -  Commects devices and share resources 
2. WAN 
- - Large area, like a city, country or a larger region 
- - Connects multiple LANs 
### C. Key networking components -> Routers, Switches, Firewalls 
#### Switches, Routers and Firewall
Switches 

- Connect devices within the same network 
- Manage data flow within a LAN 

Routers 

- Direct traffic between networks 
- Connect different networks 

Firewalls 

- Protect networks from unauthorised access 
- Monitor and control incoming & outgoing network traffic 

### D. IP addressing (IPv4 & IPv6)

#### IP Addresses 

IP Addressing -> Unique identifiers for devices on a network

#### IPv4 
- 192.168.0.5 
- - 32-bit address 
- - Format -> four decimal numbers seperated by dots 

#### IPv6 
- 2001:0db8:85a3:0000:0000:8a2e:0390:7334
- - 128-bit address 
- - Format -> eight groups of four hexidecimal deigits seperated by colons 


- IP address -> stands for internet protocol address 
- IPv4 -> each group can vary from 0 to 255 and provides 4.3 billion unique addresses 
- With the rapid growth of the internet, IPv4 addresses are becoming scarce - that is why IPv6 comes in 
- IPv6 -> The transition is essential for the growth of the internet. Includes enhancements like simplfied address assignment and improved security features 
- IP addresses enables devices to identify and communicate with each other on the network. Without IP addresses, devices wouldn't know where to send or recieve data. 

### E. MAC addresses 

#### MAC Addresses 

MAC Addresses -> Unique identifiers assigned to network interfaces (Media Access Control Address)

Format 
- 48-bit address 
- Example: 00:1A:2B:3C:4D:5E

Function 
- Operates at the data link layer of the OSI model - data link layer is responsible for node to node transfer. 
- Facilitates device identification within a local network 

Importance 

- Essential for network communication and security 

### F: Ports and Protocols (TCP, UDP)
#### Ports & Protocols: TCP, UDP 

- What are ports? -> Logical endpoints for communication. Think of ports are logical doors on your device. Each door is numbered and each number is used for a specific type of network communication e.g. web traffic typically goes through port 80 (HTTP) and port 443 for HTTPS. These ports help facilitate communcation between devices. When your computer wants to send or rreceive  data is uses these ports to make sure that the data goes to the right place. 

- Definition of Protocols -> Rules governing data transmission. Rules of the road for data transmission. Common protocols include HTTP, FTP, SNTP and more. Protocols are languages devices use to talk to each other. 

- Importance -> Facilitates communication between devices. Without ports and protocols our device communication would be a mess. Ports make sure the data gets to the application and protocols makes sure data is understandble and properly formatted for smooth communication. 

#### Transmission Control Protocol (TCP)

- It is the postman of the internet. It ensures that data sent from one device reaches another device accuratley and in the correct order. It is a protocol which means there is a set of rules that is folllows. 

##### Characteristics of TCP 
1. Connection-oriented -> This means that before any data is sent, a connection is sent between two devices. A bit like a phone call, you need to dial and get connected first.

2. Requires a 'handshake' -> This is the process where the two devices agree to communication. Its like when two people handshake when they agree on something. In networking this handshake is a three step process to make sure that both devices are ready to send and rreceive  data. 

3. Reliable data transfer -> TCP makes sure that all data is sent correctly. If any data is lost or corrupted, TCP will send it. 

##### Functions of TCP 
1. Ensures data is delivered in order -> TCP make sure the data is delivered in the correct order. 
2. Error-checking and flow control -> this is to prevent congestion. 
3. Any bidirectional communication -> communication happens back and forth 

#### User Datagram Protocol (UDP)
- UDP is a simple protocol used to send and receive  data. Unlike TCP, UDP is connectionless. 

##### Characteristics of UDP 
1. Simple protocol to send and receive data.

2. Prior communication not required (can be a double-edged sword). Pro -> data can be sent immediatley without waiting for the connection to be established. Con -> there is no gurantee that the data will reach its destination 

3. Connectionless 

4. Fast but less reliable 

##### Functions of UDP 
1. Suitable for real-time applications (e.g. video streaming)

2. DNS 

3. VPN - Virtual private network 

##### TCP vs UDP 

<table>
<tr>
<th>Comparison</th>
<th>TCP</th>
<th>UDP</th>
</tr>
<tr>
<td>Connection</td>
<td>Connection -oriented</td>
<td>Connectionless</td>
</tr>
<td>Reliability</td>
<td>Reliable, ensures data delivery and order </td>
<td>Less reliable, no gurantee of deliver or order </td>
</tr>
<tr>
<td>Speed</td>
<td>Slower due to overhead of connection setup</td>
<td>Faster, no connection or handshake setup is required</td>
</tr>
<tr>
<td>Error - checking</td>
<td>Error-checking and flow control</td>
<td>No error-checking or flow control</td>
</tr>
<tr>
<td>Use-cases</td>
<td>Web browsing, email, file transfer</td>
<td>Video streaming, online gaming, DNS, VPN</td>
</tr>
</table>

## OSI Model 
#### The 7-layers of the OSI model 
#### Why do we need a communication model?
- Provides a standard framework that simplifies the way devices and applications communicate over a network. 
#### Application independence 
-  Without a standard model, applications must understand the underlying network 
- Imagine having different versions of your application/software for WiFi, Ethernet,Fiber etc. 
#### Simplified Network Equipment Managment 
- Upgrading network equipment is difficults without a standard model 
#### Decoupled innovation 
- Innovations can happen in each layer independently, without affecting the entire system 

#### 7 layers of Application 
<table>
<tr>
<td>Application</td>
<td> -> End user layer

-> HTTP, FIP, IRC, SSH, DNS</td>
</tr>
<tr>
<td>Presentation</td>
<td>-> Syntax user layer

   -> SSL, SSH, IMAP, FTP, MPEG, JPEG</td>
</tr>
<tr>
<td>Session</td>
<td> -> Sync and send to port 

-> API's, Sockets, Winsock</td>
</tr>
<tr>
<td>Transport</td>
<td>-> End-to-end Connections 

-> TCP, UDP</td>
</tr>
<tr>
<td>Network</td>
<td>-> Packets

-> IP, ICMP, IPSec, IGMP</td>
</tr>
<tr>
<td>Data-link</td>
<td>-> Frames 

-> Ethernet, PPP, Switch, Bridge</td>
</tr>
<tr>
<td>Physical</td>
<td>-> Physical Structure

-> Coax, Fibre, Wireless, Hubs, Repeaters</td>
</tr>
</table>

#### Layer 1: Physical Layer 
- Function -> Transmits raw bit steam over a physical medium 
- Components -> Cables, Switches and Network interface cards 

-> This deals with the hardware connection including cables, switches and network interface cards. Physical medium can be copper that transmitts electric signals, fibre, light waves and wifi. There is no device addressing here -> that means that all data is processed by all devices. Think of it like shouting in a room without saying any names. This is the limitation at layer 1 and it is solved in Layer 2. 
#### Layer 2: Data Layer 
- Function -> This layer provides node-to-node data transfer and detects, possibly corrects, errors that may occure in the Physical Layer. It ensures that data is transferred correctly between adjacent network nodes. 
- Components -> Mac addresses, Switched and Bridges  
- Think of it as a traffic cop, that ensures data packets are sent and received correctly between differnt network nodes. Its all about maintaining a reliable network link between different devices. In layer 1 data is sent randomly and not in order. Layer 2 puts your data packets into frames where it is actually organised, like envelopes carrying the data to ensure it gets to the right place. 
#### Layer 3: Network Layer 
- Function -> Determines how data is sent to the recipient. Manages packet forwarding including routing through intermediate routers. 
- Components -> IP addresses, Routers 
- Decides the best path for data to travel. Data in this layer are organised in packets. Packets are like little parcels that carry data from one device to another. IP addresses handle where packets go to. Routers are components that allow it to do its job. 
#### Layer 4 Transport Layer 
- Function -> Provides reliable data transfer services to the upper layers. Segments and reassembles data. 
- Components -> TCP, UDP 
- Think of it like the delivery service that make sure your data packets arrive safely and in the right sequence.
#### Layer 5: Session Layer 
- Function -> Manages sessions between applications. Establishes, maintains and terminates connections
- Components -> Session management protocols 
- Establishing means getting a session started like when you login to a website for example. Maintaining means keeping the session alive ensuring that any conversions or requests can continue smoothly. Terminating would be closing any session e.g. logging out or closing the browser 
#### Layer 6: Presentation Layer 
- Function -> Translates data between the application later and the network. Ensures that data is in a usable format 
- Components -> Encryption, data formatting 
- Sometimes known as the syntax layer. Why? Because it ensures that the data being sent is in a readble and usable format. Think of it like a translator that converts your data into a format that the application layer (layer 7) can understand. Encryption is for security. 
#### Layer 7: Application Layer 
- Function -> Provides network services directly to applications. End-user layer 
- Components -> HTTP, FTP, SMTP
- It is the top layer of the OSI model. Everything happens that you the user can interact with. FTP is when your are transferring files between different servers generally. SMTP is being used when sending emails. 

#### TCP/IP Model: A commonly used model
1. Application Layer -> HTTP, TLS, DNS 
2. Transport Layer -> TCP, UDP 
3. Internet Later -> IP 
4. Network Access Layer -> Ethernet, Wireless LAN 

#### OSI Layers: POV of sender & receiver 
##### POV of Sender 
"User sends a POST request to an HTTP web page
1. Layer 7 - Application -> POST request with JSON data to the HTTPS server 
2. Layer 6 - Presentation -> Serialise JSON to flat byte data strings 
3. Layer 5 - Session -> Request to esablish TCP connection/TLS
4. Layer 4 - Transport -> Sends SYN request to target port 443 which is HTTPS 
5. Layer 3 - Network -> SYN in an IP packets and add the source/destination IP 
6. Layer 2 - Data Link Layer -> Each packet goes into a single frame and adds the source/destination MAC addresses 
7. Layer 1 - Physical -> Eac hframe become string of bits which is converted into wither a radio signal (Wi-Fi), electrical signal (Ethernet), or light (Fibre)
##### POV of Receiver
"User sends a POST request to an HTTP web page"
1. Layer 1 - Physical -> Radio, electric or light is recieved and converted into digital bits 
2. Layer 2 - Data Link -> the bits from layer 1 is assembled into frame 
3. Layer 3 - Network -> The frame forms layer 2 are assembled into an IP packet 
4. Layer 4 - Transport -> The IP packets from layer 3 are assembled into TCP segments 
5. Layer 5 - Session -> The connection session is established 
6. Layer 6 - Presentation -> Decrypt and decompresses the data recieved 
7. Layer 7 - Application -> Interprets the HTTP request and processes it accordingly  

## DNS 
#### What is DNS?
- Domain Name System 
- DNS allows us to keep track of websites or host by name instead of an IP address 
- A bit like a contact list for the internet 
- A bit like you know someones name but not their phone number, you could just find their name and call them.

-> Definition: Translate domain names to IP addresses 

-> Role in Networking: Simplifies navigation on the internet. Essential for accessing websites and services 

#### DNS Components -> Nameservers & Zone files 
##### Name Servers 
- Load DNS settings and configurations
- Can be authoritative (hold the actual DNS servers when queried they provide the definite answer such as the IP address for a domain) or recursive (these servers do not hold the final answer. Can cash the information they receive to speed up future queries)
- Can find the NS of a domain doing the ~dig ns google.com OR ~ dig +short ns google.com

##### Zone files 
- Are stored inside the name servers 
- Store information about the domain 
- Organised and readable format 

#### DNS Components -> Records 
- A Zone file consists of multiple records. 
- Each record hosts name servers etc. 
- Entreis in a zone file with specific information 
- Components: Record name, TTL, Class, Type, Data 
1. Record name -> The domain name being queried 
2. Time to live (TTL) -> Indicates how long the record is valid (before refresh required)
3. Class -> Namespace of the record information 
4. Type -> Type of record (A or MX or AAAA etc)
5. NS -> Name server record 
6. Data -> The actual information corresponding to the record type. Like IP address for an A record 

##### DNS Records 
1. A -> Maps a domain name to an IPv4 address 

EXAMPLE google.com -> 216.58.204.79

2. AAAA -> Maps a domain name to an IPv6 address 

EXAMPLE google.com -> 2a00:1450:4009:81d::200e

3. CNAME -> Alias of one name to another. It allows you to point multiple domain names to the same IP address 

EXAMPLE www.google.com -> google.com 

4. MX -> Specifies the mail server responsible for receiving email for the domain (mail exchange) - essential for writing email to make sure email delivery is reliable

EXAMPLE google.com -> mailserver.google.com

5. TXT -> Allows domain administators to insert any test into DNS. Commonly used for verification purposes and to hold SPF (Sender Policiy Framework) data. Can be used to verify that you own the domain 

EXAMPLE google.com -> "v=spf1 include.com ~all"

#### How does DNS work?
#### Networking Debugging Tools: 'nloopup' and 'dig'
#### ./etc/hosts file 