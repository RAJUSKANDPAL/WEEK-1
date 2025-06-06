## What is the OSI model?
OSI or the Open Systems Interconnection model is a set of rules and protocols that explains how a computer system communicates over the internet .The OSI model was developed by the International Organisation for Standardization (ISO). It consists of seven distinct layers and each layer has specific functionalities and responsibilities ranging from physical hardware connections to high level application interaction.

Each layer in the OSI model interacts with the layers immediately above and below it, encapsulating it and transmitting data in an organized manner. This method assists network specialists in troubleshooting difficulties since faults may be isolated to a single layer. The OSI model serves as a universal language for networking, allowing diverse systems to interact successfully. 

The OSI model was the first standard for network communications, and all major computer and telecommunications firms embraced it in the early 1980s. It was introduced in 1983 by representatives from major computer and telecommunications firms, and ISO accepted it as an international standard in 1984.

## The OSI model consists of the following seven layers 
Application Layer (Layer 7)

Presentation Layer (Layer 6)

Session Layer (Layer 5)

Transport Layer (Layer 4)

Network Layer (Layer3)

Data Link Layer Layer 2)

Physical Layer (Layer 1)

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/582ec9d41c483de67f012633320be41fd98d56b8/1%20OSI.webp)

## Application Layer
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/7d7a9a2f6be7b5e9b57f9bafdeaecb72e8f5ed5c/2%20APPL.webp)

The Application Layer connects end-user apps to the network's underlying services.This layer offers protocols and services used directly by end-user applications to communicate over the network. The Application Layer's key capabilities are resource sharing, remote file access, and network administration.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/3%20APPL.webp)

The application layer facilitates communication between applications and provides services to end users using protocols like as HTTP, SMTP, FTP, DNS, and DHCP. These protocols provide the rules and standards for data exchange, guaranteeing compatibility among different systems. 

## Functions of the Application Layer
The primary roles of the application layer are listed below.

**1.Network Virtual Terminal (NVT):** Allows users to connect to a remote host.

**2.File Transfer Access and Management (FTAM):** This program enables users to access and retrieve files from a remote host, as well as manage and control files from a distant computer.

**3.Mail Services:** Offer email service.

**4.Directory Services:** This program offers distributed database sources and access to global information about numerous objects and services.

## Key Application Layer Protocols:

**1.HTTP (Hypertext Transfer Protocol):** A protocol for accessing the web and transferring hypertext content.

**2.SMTP (Simple Mail Transfer Protocol)** is used to send emails.

**3.FTP (File Transfer Protocol):** A method for transmitting files between computers.

**4.DNS (Domain Name System)** resolves domain names to IP addresses.

**5.DHCP (Dynamic Host Configuration Protocol)** assigns IP addresses to network devices.

**6.POP3/IMAP (Post Office Protocol/Internet Message Access Protocol)** is used to retrieve email from servers.

**7.Telnet:** A protocol for remote login and file access on distant computers.

**8.SNMP (Simple Network Management Protocol)** is used for monitoring and managing network devices.

**9.NFS (Network File System):** NFS is a protocol for remotely accessing file systems.

**10.TFTP (Trivial File Transfer Protocol)** is a simplified version of FTP that does not require authentication.

## Presentation Layer

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/4%20PRESEN.webp)

The Presentation Layer, also known as the Syntax Layer, is responsible for translating data between the application layer and network format. It guarantees that data transmitted from one system's application layer is readable by the application layer of another system. This layer is responsible for data formatting, encryption, and compression, allowing multiple systems to communicate with one another.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/5%20PRESEN.webp)

The Presentation Layer plays an important role in data translation and code conversion. It converts data to a format that the application layer understands. As an example, it may convert data from ASCII to EBCDIC. It also includes encryption mechanisms to protect data during transmission and compression protocols to minimize data size for more efficient delivery.

## Working of the Presentation Layer -
**1.Data Translation:** The conversion of data into a standardized format (for example, EBCDIC to ASCII).

**2.Data compression** reduces data size to improve bandwidth and performance.

**3.Data Encryption and Decryption:** Protects data during transmission (e.g., SSL/TLS).

**4.Syntax and Semantics:** Ensures data is correctly interpreted across systems.

**5.Interoperability** bridges data format discrepancies between devices.

## Presentation Layer Protocols
To conduct translations or other required functions, the Presentation Layer must follow the protocols outlined below:


**1.The Apple Filing Protocol (AFP)** is a proprietary network protocol that supports macOS and its predecessors. This is essentially a network file control protocol created exclusively for Mac-based systems.

**2.The Lightweight Presentation Protocol (LPP)** is a protocol that provides ISO presentation services on top of TCP/IP-based protocol stacks.

**3.NetWare Core Protocol (NCP)** is a network protocol for accessing files, printing, synchronizing clocks, sending messages, executing remote instructions, and providing more network services.

**4.Network Data Representation (NDR)** is the implementation of the OSI model's presentation layer, which offers or specifies numerous raw data types, built data types, and data representations.

**5.The External Data Representation (XDR)** is a standard that describes and encodes data.It is helpful for transferring data between computer architectures and has been used to convey data between a wide range of devices. Encoding is the conversion of local representation to XDR, while decoding is the conversion of XDR back into local representation.

**6.The Secure Socket Layer (SSL) protocol** safeguards data transmitted between web browsers and servers. SSL encrypts the connection between a web server and browser, protecting data from unauthorized access.

## Session Layer
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/6%20SESSN.webp)

The Session Layer monitors and supervises network connections between computers. It initiates, maintains, and terminates connections to ensure that data exchanges are efficient and orderly. The layer is in charge of session checkpointing and recovery, which allows sessions to continue after disruptions.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/7%20SESSN.webp)

The Session Layer protocols include Remote Procedure Call (RPC), which allows a program to perform a function on a distant host as if it were local, as well as the session formation phase in protocols such as NetBIOS and SQL. These services provide for reliable communication, particularly in complicated network contexts.

## Functions of the session layer

The session layer performs several distinct and crucial fucntions that are required for establishing and maintaining a safe and secure connection:


**1.Session Establishment:** It sets up and administers sessions between communication parties, which might be connection-oriented or connectionless. It also links sessions to transportation connections.

**2.Communication Synchronization:** The use of synchronization bits and checkpoints in the data stream guarantees dependable connectivity and recovery.

**3.Activity Management:** It allows the user to organize data into logical pieces known as activities. An action can be processed on its own, and each activity is separate from the activities that occur before and after it.

**4.Dialog management :** It  is the process of determining who has the right to speak next. Some programs employ a token system for half-duplex mode, in which only one person retains the token and transmits data, whilst others offer full-duplex mode, which allows for simultaneous data transfer.

**5.Data Transfer:** It handles data transmission between systems.

**6.Resynchronization:** This restores all tokens to the locations they were in after synchronization. The resynchronization options include set, abandon, and restart.

## Working of the Session Layer

1.The Session Layer coordinates communication sessions between programs across a network.

2.It creates connections and negotiates session settings such as authentication and communication direction (full or half-duplex).

3.It regulates data exchange by utilizing tokens to govern transmission rights and prevent collisions.

4.Synchronization mechanisms are used, including checkpoints for recovery in case of disturbances.

5.It promotes ordered communication by minimizing message loss, duplication, and mistakes produced by overlapping communication.

6.The Session Layer terminates the session, verifying that all data has been transmitted and all parties agree to close.

## Session Layer Protocols

Session Layer employs several protocols necessary for safe, secure, and accurate communication between two-ender user applications. The Session Layer provides or uses the following protocols:


**1.AppleTalk Data Stream Protocol (ADSP):** ADSP is a protocol designed by Apple Inc. that has a variety of characteristics that allow local area networks to be linked without any prior configuration. This protocol was released in 1985. This protocol strictly adhered to the OSI concept of protocol stacking. ADSP features two protocols: AppleTalk Address Resolution Protocol (AARP) and Name Binding Protocol (NBP), both of which are designed to allow the system to configure itself.

**2.Real-time Transport Control Protocol (RTCP):** RTCP is a protocol that offers out-of-band statistics and control information for an RTP (Real-time Transport Protocol) connection. The major goal of RTCP is to offer feedback on the quality of service (QoS) in media distribution by transmitting statistical information to streaming multimedia session participants on a regular basis, such as transmitted octet and packet counts, or packet loss.

**3.Point-to-Point Tunneling Protocol (PPTP)** is a protocol for establishing virtual private networks. PPTP employs a TCP control channel and a Generic Routing Encapsulation tunnel to encapsulate PPP (Point-to-Point Protocol) messages. This protocol offers security and remote access levels equivalent to traditional VPN (Virtual Private Network) offerings.

**4.Password Authentication mechanism (PAP)**: PAP is a password-based authentication mechanism used by the Point to Point Protocol (PPP) to validate users. Almost all network operating systems, including remote servers, support PAP. PAP authentication is performed at the initial link establishment and checks the client's identity via a two-way handshake (client provides data, and the server responds with Authentication-ACK (Acknowledgement) once the data supplied by the client is fully confirmed).

**5.Remote Procedure Call Protocol (RPCP)**: This protocol is used when a computer program allows a procedure (or subroutine) to run in a separate address space without the programmer explicitly coding the specifics for the distant interaction. This is essentially a type of client-server interaction, which is often accomplished via a request-response message-passing mechanism.

**6.Sockets Direct Protocol (SDP)** is a protocol that allows socket streams to be sent over RDMA network fabrics. The goal of SDP is to offer an RDMA-accelerated alternative to the TCP protocol. The primary purpose is to do one specific action in a way that is transparent to the application.

## Transport layer

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/8%20TRSPT.webp)

The Transport Layer offers end-to-end communication services for applications. It enables comprehensive data transport, error recovery, and flow management between hosts. This layer divides and reassembles data to ensure efficient transmission and dependability through error detection and repair procedures.

![image](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/9%20TRSPT.webp)

This layer's protocols include the Transmission Control Protocol (TCP) and the User Datagram Protocol (UDP). TCP is connection-oriented and provides reliable data transport through error checking and flow management, making it ideal for applications such as web surfing and email. UDP is a connectionless protocol that provides quicker but less reliable transmission, making it appropriate for applications such as video streaming and online gaming.

## Working of the Transport Layer

1.The Transport Layer enables reliable and effective communication between end systems. It not only regulates flow and accommodates several applications at the same time, but it also ensures data transmission in an accurate and error-free way. It does this by utilizing a set of techniques and protocols for data transfer.

2.The transport layer's primary role is to provide application processes running on several hosts direct access to communication services.

3.The transport layer facilitates logical communication between application processes on distinct hosts. Application processes use the transport layer's logical communication to send messages to one another, even if they are executing on separate hosts and are not physically linked.

4.The transport layer protocols are implemented by the end systems, not the network routers.
For example, the network layer gets services from TCP and UDP, two transport layer protocols with differing capabilities.

5.Protocols at the transport layer enable multiplexing and demultiplexing. In addition, it provides bandwidth assurances, latency guarantees, and consistent data transfer.

6.Every program at the application layer can send a message using either TCP or UDP. The application can interact via one of these two protocols. The internet protocol on the internet layer will then be communicated with via TCP and UDP. Applications can read and write to the transport layer.

## Transport Layer Protocols

Transport Layer Protocol uses different protocols for better communication between two ends. Uses of protocol may differ from specifications. Below mention are some protocols used in Transport Layer


1.Transmission Control Protocol(TCP)

2.User Datagram Protocol (UDP)

3.Stream Control Transmission Protocol (SCTP)

## Network Layer

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/10%20NTWRK.webp)

The Network Layer manages data routing, forwarding, and addressing. It finds the optimum physical path for data to take to its destination depending on network circumstances, service priority, and other considerations. This layer manages logical addressing via IP addresses, as well as packet forwarding.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/11%20NTWRK.webp)

Data is exchanged as packets between devices via various logical network channels. It provides paths for data packet flows across the network. The network layer also organizes and controls the available data transport pathways.

## Functions of the Network Layer

Some of the most essential functions of the network layer are listed below.


**1.Assigning Logical Addresses**: It assigns unique IP addresses to devices to facilitate identification and communication across networks.

**2.Packetizing** wraps data in packets for efficient transmission.

**3.Host-to-Host Delivery**: This guarantees that data is transmitted from the sender to the appropriate receiver across networks.

**4.Forwarding** is the process of transporting packets from the input to the appropriate output interface in a router, depending on the destination address.

**5.Fragmentation and Reassembly**: Large packets are broken into smaller fragments for transmission and then reassembled at the destination.

**6.Logical subnetting** is the process of dividing larger networks into smaller subnetworks in order to improve routing and administration efficiency.

**7.Network Address Translation (NAT)** converts private IP addresses to public IP addresses for internet access, therefore preserving IP addresses and increasing security.

8.Routing finds the optimum route for packets to take across numerous networks.

## Working of the Network Layer

1.Each device is assigned a unique address (IP address) to identify it on the network.

2.Data is packed in little packets with labels indicating where it came from and where it is heading.

3.Routers choose the optimum way to take packets to their destination.

4.Packets pass via many routers before arriving at the intended device.

5.If a packet is too large, it is broken down into smaller bits to fit via the network.

6.At the destination, the fragments are reassembled into the original data.

7.If something goes wrong, such as the destination being unreachable, an error message is returned.

## Protocols Used at Network Layer

The protocols used at the Network Layer are:


1.IP (Internet Protocol)

2.ICMP (Internet Control Message Protocol)

3.ARP (Address Resolution Protocol)

4.RARP (Reverse Address Resolution Protocol)

5.NAT (Network Address Translation)

### Routing Protocols:

1.RIP (Routing Information Protocol)

2.OSPF (Open Shortest Path First)

3.BGP (Border Gateway Protocol)

4.IPSec (Internet Protocol Security)

5.MPLS (Multiprotocol Label Switching)

## Data Link Layer

![image](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/12%20DTA%20LNK.webp)

The Data Link Layer handles data flow between nodes as well as error detection and repair. It guarantees that data is routed to the appropriate device on a local network segment. This layer handles MAC (Media Access Control) addresses and is separated into two sublayers: Logical Link Control (LLC) and Media Access Control (MAC).

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/13%20DTA%20LNK.webp)

This layer's protocols and technologies include Ethernet, which establishes the rules for data transmission over local area networks (LANs), as well as Point-to-Point Protocol (PPP), which allows direct connections between two network nodes. It also has techniques for identifying and perhaps repairing problems in the Physical Layer.

### Sub-Layers in the Data Link Layer

The data connection layer is then separated into two sub-layers, which are as follows:


**1.The Media Access Control (MAC)** sublayer oversees device interactions, addresses frames, and controls physical media access. The data link layer takes information in the form of packets from the network layer, splits them into frames, and transfers them bit-by-bit to the physical layer.

**2.Logical Link Control (LLC)** This sublayer of the data connection layer is responsible for multiplexing and data flow between applications and other services, as well as giving error messages and acknowledgments.

## Protocols in Data link layer

There are various protocols in the data link layer, which are as follows:


1.Synchronous Data Link Protocol (SDLC)

2.High-Level Data Link Protocol (HDLC)

3.Serial Line Interface Protocol (SLIP)

4.Point to Point Protocol (PPP)

5.Link Access Procedure (LAP)

6.Link Control Protocol (LCP)

7.Network Control Protocol (NCP)

## Devices operating at the data link layer

**1.Switch** - It employs MAC addresses to route data packets to the appropriate device on a network.
Works with local area networks (LANs) to connect many devices.

**2.Bridge** - A bridge joins two or more LANs to form a single, unified network.
Operates at the Data Link Layer, forwarding frames depending on MAC addresses.
Used to minimize network traffic and segment networks.

**3.Network Interface Cards (NICs)**A network interface card (NIC) is a hardware component found in devices such as computers and printers.
Responsible for assigning MAC addresses to frames and ensuring correct network connectivity.
Operates at the Data Link Layer, preparing and transmitting frames via the physical media.

**4.Wireless Access Points (WAP)** -A WAP connects wireless devices to a wired network.
Manages wireless MAC addresses at the data link layer.
Communicates with devices via protocols such as Wi-Fi (IEEE 802.11).

**5.Layer Two Switches** - These are specialized switches that exclusively work at Layer 2, as opposed to multilayer switches.
Responsible for frame forwarding utilizing MAC address tables.

## Physical Layer

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/14%20PHY.webp)

The physical layer refers to the actual communication media and the technologies used to send data across the medium. At its core, data communication is the transmission of digital and electrical signals across multiple physical channels such as fiber-optic cables, copper wiring, and air. The physical layer incorporates technology standards and channel-specific metrics such as Bluetooth, NFC, and data transfer speeds.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/4c5ab8e7a0fa6db8a80e0c83758edeb27578c77e/15%20PHY.webp)

The physical layer transmits data bits from one or more devices (such as computer) to another(s). The physical Layer specifies the forms of encoding (how 0's and 1's are encoded in a signal). Its responsibility is to communicate unstructured raw data streams via a physical channel.
The Physical Layer performs modulation, bit synchronization, and transmission of raw binary data via the physical channel. At this tier, technologies such as fiber optics and wi-fi ensure that data physically travels from one network device to another.

## Services Offered by Physical Layer

1.Bit-by-Bit Transmission
2.Encoding and Decoding
3.Signal Transmission
4.Modulation and Demodulation
5.Transmission Modes
     The Physical Layer defines how data flows between devices. There are three main transmission modes  
     **(a) Simplex Mode** -Data flows in just one direction.  
     The sender can send data, but the recipient cannot return information.
     Consider a TV broadcast in which the station sends signals but receives no data from the TV.  
    **(b) Half-Duplex Mode** - Data moves in both ways, but only in one at a time.  
     The sender must wait for the receiver to complete before answering.
      For example, walkie-talkies need users to take turns speaking.  
    **(c) Full-Duplex Mode** - Data is sent in both ways simultaneously.  
     It improves transmission speed by enabling continuous data sharing.
     Consider telephone calls in which both persons may speak and listen at the same time.
6. Data Control
     The Physical Layer manages data timing and flow to prevent transmission mistakes and inefficiencies.  
     **(a) Synchronization** makes sure that the transmitter and receiver are in sync and that the bits are properly understood. For example, synchronization in              video streaming minimizes delays or distortions in audio and visual playing.  
     **(b) Flow Control** regulates the speed differential between the transmitter and receiver to guarantee seamless communication.
    For example, with USB connection, the data transfer rate is changed according to the capacity of the connected device.
    






















