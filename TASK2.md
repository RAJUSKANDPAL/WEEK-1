## The TCP/IP Model
The TCP/IP model is a four-layer communication framework that ensures dependable data exchange across interconnected networks. It defines a standard protocol suite for transmitting information, allowing reliable and efficient delivery. Each layer has its own specific role in managing network communication, which is essential for understanding and utilizing modern networking systems. TCP/IP is also applied in private network environments like intranets and extranets.
Originally developed by the U.S. Department of Defense in the 1970s, the TCP/IP model uses standardized protocols. Unlike the OSI model, which has seven layers, the TCP/IP model simplifies the structure to four layers. It outlines the procedures for breaking down data into packets, addressing, transporting, routing, and delivering them reliably. With minimal central control, TCP/IP is resilient to device failures and enhances network reliability.

![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/1.webp)


## Purpose of TCP/IP
TCP/IP enables systems with diverse network types (such as fiber optics, wireless, and copper cables) to interoperate effectively. It facilitates seamless connectivity between LANs, WANs, and the internet. Without this model, global networking on a large scale would not be achievable.
A critical aspect of TCP/IP is ensuring data accuracy and integrity, guaranteeing that the recipient receives exactly what the sender transmitted. It achieves this by dividing the data into packets and reassembling them correctly at the destination.

## Difference between TCP and IP
The two main protocols in the IP suite serve specific functions and have numerous differences. The key differences between TCP and IP include the following:  

**TCP**    
1.It ensures a reliable and orderly delivery of packets across networks.

2.TCP is a higher-level smart communications protocol that still uses IP as a way to transport data packets, but it also connects computers, applications, web pages and web servers.

3.TCP understands holistically the entire stream of data that these assets require to operate and it ensures the entire volume of data needed is sent the first time.

4.TCP defines how applications can create channels of communication across a network.

5.It manages how a message is assembled into smaller packets before they're transmitted over the internet and reassembled in the right order at the destination address.

6.TCP operates at Layer 4, or the transport layer, of the Open Systems Interconnection (OSI model).

**IP**  
1.IP is a low-level internet protocol that facilitates data communications over the internet.

2.IP delivers packets of data that consist of a header, which contains routing information, such as the source and destination of the data and the data payload itself.

3.It defines how to address and route each packet to ensure it reaches the right destination. Each gateway computer on the network checks this IP address to determine where to forward the message.

4.IP is limited by the amount of data it can send. The maximum size of a single IP data packet, which contains both the header and the data, is between 20 and 24 bytes. This means that longer strings of data must be broken into multiple data packets that have to be sent independently and then reorganized into the correct order.

5.It provides the mechanism for delivering data from one network node to another.
 
## Layers of TCP/IP Model
In contrast to the OSI model, which has seven layers, TCP/IP has four interconnected ones. Each layer does a certain task with the data that is being broadcast over the network channel, and data passes from one layer to the next.

### Application Layer (Layer 1)
### Transport Layer(TCP/UDP) (Layer 2)
### Network/Internet Layer(IP) (Layer 3)
### Network Access Layer (Layer 4)
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/2.avif)

## 1. Application layer
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/3.avif)  
This is the TCP/IP model's top layer, responsible for facilitating communication between user-facing programs and the network. It handles activities such as preparing data for applications and sending it to the transport layer for further processing.

The application layer maintains a smooth connection between the application and the user for data interchange and provides a variety of capabilities such as remote system management, e-mail services, and so on.  

## Key responsibilities:
1.Supports application protocols such as HTTP, FTP, SMTP, and DNS.  
2.Allows software applications to communicate with each other over networks.  
3.Manages data formatting, encryption, and session management.  

## 2.Transport Layer  
![image](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/4.avif)  

Ensures that data is reliably transmitted between hosts. It includes the TCP and UDP protocols.   
**TCP:**   Provides reliable, connection-oriented communication, error correction, and flow control.  
**UDP:**   Delivers faster, connectionless transmission without reliability guarantees.Handles segmentation and reassembly of data into smaller packets.Responsible for port addressing, which allows multiple applications on the same device to communicate.Manages end-to-end message delivery, acknowledgments, and retransmission of lost data.
Ensures data integrity through checksums and flow regulation through sliding windows and congestion control.


## 3.Internet Layer  
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/5.avif)

Internet Layer Manages the delivery and routing of data packets.    
It assigns unique IP addresses to devices and calculates the most efficient routes.  
**IP:** Manages addressing and packet forwarding.   
**ICMP:** Reports errors and diagnostics.  
**ARP:** Resolves IP addresses to MAC (hardware) addresses.Responsible for packet fragmentation and reassembly across different networks.Routes packets independently, determining the best path based on routing tables and network conditions.  
Ensures logical addressing and decouples network hardware from software protocols  

## 4. Network Access Layer  
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/6.avif)

This layer is the model's lowest layer and is in responsible for establishing physical connections between devices in the same network segment. This layer is a hybrid of the data-link and physical layers, and it is in charge of maintaining the task of sending and receiving data in raw bits, i.e., binary format, via the physical communication modes in the network channel.  
**Function:** Controls the physical transfer of data over network hardware.  
Responsibilities include managing data transmission via wires, Wi-Fi, and other methods.  
Manages MAC addressing, framing, and error detection on the physical link.  
Ethernet, Wi-Fi, and other data communication technologies are all included.  
It uses the system's physical address to map the transmission path across the network channel.  

**When Sending Data (Sender to Receiver)**  
**The Application Layer**  
 A user sends data using an application (for example, opening a website in a browser).  
 The application prepares data for transmission (by HTTP, FTP, or SMTP).    
**Transportation Layer (TCP/UDP)**  
 TCP splits data into discrete segments and adds a header (including sequence numbers and source/destination ports).  
 Provides reliable delivery (TCP) or quick, connectionless delivery (UDP).  
 **Internet layer (IP)**  
 IP addresses are added to each packet (source and destination).   
 Determines which route the packet should take to reach its destination.  
**Link Layer (network access layer)**
 Converts packets into frames and assigns MAC (physical) addresses.  
 Data is transmitted as binary bits (0s and 1s) over a physical media (such as Ethernet or Wi-Fi).      
 
 **When Receiving Data (at the destination)**  
**Link Layer**  
 Receives information and reconstructs frames.   
 Passes frames to the Internet layer.  
**Internet Layer**   
 Checks the IP address to ensure it's the correct recipient.  
 Removes the IP header and passes the data to the Transport layer.  
**Transport Layer**  
 Reassembles TCP segments in the proper sequence.  
 Data integrity is verified via acknowledgments and checksums.  
**Application Layer**  
 The data is sent to the relevant program (for example, a browser shows a web page).  
 
 ![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/7.webp)

## Why is TCP/IP used over the OSI model?
**Simpler structure.**  
TCP/IP comprises only four levels, compared to OSI's seven, making it easier to implement and understand in practical systems.    
**Protocol-driven design.**  
TCP/IP was created around working protocols, whereas the OSI paradigm is more of a theoretical framework.  
**Flexibility and robustness**  
TCP/IP works well with various hardware and networks and incorporates error handling, routing, and congestion control.  
TCP/IP is an open standard, free to use, and not controlled by a particular body, resulting in worldwide acceptance.  
Actual Use Versus Conceptual Model The OSI model is useful for education and design concepts, but TCP/IP is the protocol used in real-world networks.  

## Advantages of TCP/IP Model   
**Interoperability :**   The TCP/IP model enables interoperability between computers and networks, increasing compatibility and cooperation across various systems.  
**Scalability :**   TCP/IP is extremely scalable, making it appropriate for both small and big networks, ranging from local area networks (LANs) to wide area networks (WANs) such as the internet.  
**Standardization :**   It is based on open standards and protocols, ensuring that different devices and software can work together without compatibility issues.  
**Flexibility :**   The model supports a wide range of routing protocols, data kinds, and communication techniques, making it adaptable to a variety of networking requirements.  
**Reliability :**  TCP/IP offers error-checking and retransmission mechanisms to ensure that data is transferred reliably over long distances and under a variety of network situations. 

## Disadvantages of TCP/IP Model
**Security Concerns:**   TCP/IP was not originally designed with keeping security in mind. While various security protocols are now available (such as SSL/TLS), they have been layered on top of the core TCP/IP paradigm, which might lead to vulnerabilities.  
**Inefficiency for Small Networks:**   For very small networks, the TCP/IP model's overhead and complexity may be superfluous and inefficient when compared to simpler networking protocols.  
**Limited by Address Space:**   While IPv6 addresses this issue, the earlier IPv4 system has a limited address space, which can cause address exhaustion in bigger networks.  
**Data Overhead:**   The transport protocol, TCP, includes a large amount of overhead to ensure reliable transmission. This can affect efficiency, particularly for little data packets and in networks where speed is critical.  

## Protocols Used:   
TCP/IP uses four core protocols: the Transmission Control Protocol (TCP), the User Datagram Protocol (UDP), the Internet Protocol (IP), the Internet Control Message Protocol (ICMP), Address Resolution Protocol (ARP), File Transfer Protocol (FTP), Hypertext Transfer Protocol (HTTP), Simple Mail Transfer Protocol (SMTP), and Domain Name System (DNS)  

**TCP** ensures that data is delivered reliably and in the proper order.  
**UDP** is used in situations when data does not need to be transmitted consistently or fast, and TCP overhead is unnecessary.  
**IP** is the protocol that transmits data from one computer to another.     
**ICMP** is used to check for errors and manage traffic congestion.  
The **internet** cannot function properly without all four of these protocols. They collaborate to guarantee that data is supplied in a timely, reliable, and appropriate order.  
There are some other protocols also notable, and there are,
**Address Resolution Protocol (ARP):**  
ARP operates between the Internet Layer and the Network Access Layer. It is responsible for mapping a known IP address to its corresponding MAC (Media Access Control) address. This is crucial for enabling proper data transfer over a local network, as devices use MAC addresses for actual communication on the physical network.  
**Function:** Resolves IP addresses to hardware (MAC) addresses.   
**Use Case:** When a device wants to communicate with another device on the same LAN, it uses ARP to find the MAC address associated with the recipient’s IP.  

**File Transfer Protocol (FTP):**  
FTP is used for transferring files between systems over a TCP-based network such as the internet. It operates on a client-server model and uses separate control and data connections.  
**Function:** Transfers files from one host to another.  
**Ports:** Uses TCP port 21 for control and port 20 for data transfer.   
**Use Case:** Uploading website files to a web server or downloading files from a remote server.  

**Hypertext Transfer Protocol (HTTP):**  
HTTP is the foundation of data communication for the World Wide Web. It is used for transmitting web pages and multimedia content.  
**Function:** Facilitates communication between web browsers and web servers.  
**Port:** Typically operates over TCP port 80.    
**Use Case:** Loading web pages in a browser.   

**Simple Mail Transfer Protocol (SMTP):**  
SMTP is the standard protocol for sending emails across networks. It is used by email servers to transfer messages between systems and by client applications to send mail.  
**Function:** Sends and routes emails across servers.  
**Port:** Commonly uses TCP port 25 (or port 587 for secure transmission).  
**Use Case:** Sending messages from a client (like Outlook) to a mail server or between two mail servers.   

**Domain Name System (DNS):**    
DNS translates human-readable domain names (like www.celebaltech.com) into IP addresses that computers use to identify each other on the network.  
**Function:** Resolves domain names to IP addresses.  
**Port:** Uses UDP port 53 (and TCP for larger queries).  

## OSI Model vs. TCP IP Model
![image alt](https://github.com/RAJUSKANDPAL/WEEK-1/blob/9b68c8193142138e9d271ab09c39adf4e8161f40/8.avif)  

| TCP/IP MODEL                                                                   | OSI MODEL                                                          |   
|--------------------------------------------------------------------------------|--------------------------------------------------------------------|
| TCP/IP model comprises 4 layers.                                               | The OSI model consists of 7 layers.                                |
|                                                                                |                                                                    | 
| This model comprises a session and presentation layer in the application layer | The OSI model has separate session and presentation layers         |   
|                                                                                |                                                                    |  
|                                                                                |                                                                    |  
| The transport layer in this model provides a packet delivery protocol.         | In this model the transport layer does not have any such protocols |   
|                                                                                |                                                                    |   
| This model is implemented during network communication.                        | This model is used as a reference model for the network channel    |   
|                                                                                |                                                                    | 

 ## Uses of TCP/IP    
 Here are some of the most useful applications of TCP/IP models:  
1.The World Wide Web uses TCP/IP to transport data between web browsers and servers.  
2.Email applications like Outlook, Thunderbird, and Gmail employ TCP/IP protocols to send and receive messages.  
3File Transfer: FTP, SFTP, and other file transfer services use TCP/IP to send files from one computer to another.  
3.Networking: TCP/IP connects computers in a network.  
4.VPNs employ TCP/IP to encrypt data before it is transmitted over a public or private network.    
5.Internet of Things: Many smart home devices communicate and send data using TCP/IP.  
6.Voice Over Internet Protocol (VOIP): VOIP services like Skype and Google Voice use TCP/IP to send calls over the internet.  

## References  
[GFG](https://www.geeksforgeeks.org/tcp-ip-model)  
[Quizlet](https://quizlet.com/study-guides/tcp-ip-model-a665e1a2-923d-4017-950a-7c5b50234215)  
[Techtarget](https://www.techtarget.com/searchnetworking/definition/TCP-IP)  
[Linkedin](https://www.linkedin.com/posts/uche-okosa-6816ba234_cybersecuritylearning-activity-7217829979718361089-_YkK)  
[Quizlet](https://quizlet.com/gb/693190407/web-protocols-flash-cards)  
[Simplelearn](https://www.simplilearn.com/tutorials/cyber-security-tutorial/what-is-tcp-ip-model)  
[Checkpoint](https://www.checkpoint.com/cyber-hub/network-security/what-is-the-osi-model-understanding-the-7-layers/osi-model-vs-tcp-ip-model)  
[Imperva](https://www.imperva.com/learn/application-security/osi-model)  
[IBM](https://www.ibm.com/think/topics/osi-model)  
[Wikipedia](https://en.wikipedia.org/wiki/Internet_Protocol)  
[Vdocipher](https://www.vdocipher.com/blog/how-does-streaming-work)  
[Amazon](https://aws.amazon.com/what-is/smtp)  
[Study CCNA](https://study-ccna.com/osi-tcp-ip-models/)  













