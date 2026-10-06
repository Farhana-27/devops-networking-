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
#### OSI Layers: POV of sender & receiver 
#### Port and Protocol RECAP 