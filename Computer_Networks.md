1. Introduction to Computer Networks
Definition and goals of networking
Network types: LAN, MAN, WAN, PAN
Network topologies: Bus, Ring, Star, Mesh, Hybrid
Switching techniques: Circuit, Packet, Message switching
Transmission modes: Simplex, Half-duplex, Full-duplex
Network performance metrics (bandwidth, latency, throughput)

2. Physical Layer
Data and signals
Digital vs analog transmission
Encoding techniques: NRZ, Manchester, AMI, ASK/FSK/PSK
Multiplexing: FDM, TDM, WDM
Transmission media:
Guided: Coaxial, Twisted Pair, Fiber Optic
Unguided: Radio, Microwave, Satellite
Circuit switching vs packet switching
Error detection (Parity, CRC)
Data rate & channel capacity (Nyquist, Shannon laws)

3. Data Link Layer
Framing (Byte stuffing, Bit stuffing)
Error detection & correction
Flow control:
  Stop and Wait
  Sliding Window
  Go-Back-N
  Selective Repeat
MAC protocols:
  ALOHA, Slotted ALOHA
  CSMA/CD, CSMA/CA
Ethernet (IEEE 802.3)
Switching: Store-and-forward, Cut-through
PPP, HDLC

4. Network Layer
Logical addressing: IPv4 & IPv6
Classful & classless addressing
Subnetting & Supernetting
ARP, RARP, DHCP, ICMP
Routing algorithms:
  Distance Vector
  Link State
  Dijkstra’s Algorithm
Routing protocols:
  RIP, OSPF, BGP
Router architecture & forwarding
NAT, CIDR

5. Transport Layer
Process-to-process delivery
Connection-oriented vs connectionless
UDP: Header, use cases
TCP:
  Header format
  3-way Handshake
  Flow control, Congestion control
  Slow start, Tahoe, Reno
Ports & sockets
QoS: Traffic shaping, Leaky bucket, Token bucket

6. Application Layer
DNS
DHCP
Email: SMTP, POP3, IMAP
FTP, TFTP
HTTP/1.1, HTTP/2, HTTP/3
WebSocket basics
Peer-to-peer networks (BitTorrent concept)

7. Network Security & Cryptography
CIA triad: Confidentiality, Integrity, Availability
Symmetric encryption (AES, DES)
Asymmetric encryption (RSA, ECC)
Hashing (MD5, SHA)
Digital signatures & certificates
SSL/TLS
Firewalls, IDS/IPS
Threats: DoS, DDoS, Malware, Phishing

8. Wireless & Mobile Networks
802.11 Wi-Fi architecture
BSS, ESS, channels, roaming
Bluetooth basics
Cellular networks: 1G to 5G
Mobile IP
Ad-hoc networks (MANET)

9. Emerging Topics (Optional but useful)
SDN (Software Defined Networking)
NFV (Network Function Virtualization)
IoT networking
Cloud networking
QUIC protocol
6G basics

## Data Flow
1. simplex :
   Unidirectional communication.
   One device transmits, and the other device receives.
   ex: keyboard 
2. Half duplex :
   Communication is in both directions, but not at the  same time.
   If one device is sending, the other can only receive, and vice versa.
   example: walkie-talkies 
3. Full duplex :
   communication is in both directions simultaneously.

## Elements of protocol 
1. message encoding
2. message formatting and encapsulation
3. message timing
4. message size
5. message delivery options
   a. Unicast: when the sender sends data to a single targeted system.   
   b. Multicast: when the sender sends data to more than one targeted system.  
   c. Broadcast: when the sender sends data to all devices without knowing the target.

## Components of a computer network
1. Nodes:
   1. end node
   2. intermediary node:
      1. switches
      2. wireless access point
      3. routers
      4. security devices (firewall)
      5. bridges
      6. hubs
      7. repeaters
      8. cell tower 
3. Media
4. Services

## classification of computer network 
1. LAN: Local Area Network:
2. MAN: Metropolitan area network:
3. WAN: Wide Area network
4. Internet

## topology 
### Bus topology  
   <img width="1516" height="872" alt="image" src="https://github.com/user-attachments/assets/a9078a4f-a5e5-48bd-bdc4-e20ee66af215" />       
   
### Ring topology  
   <img width="588" height="600" alt="image" src="https://github.com/user-attachments/assets/1a410b77-2185-4327-acee-00389a0279a8" />  
   
### Start topology   
   <img width="1080" height="864" alt="image" src="https://github.com/user-attachments/assets/010e03b4-1768-4a6c-85c6-9cb13e209587" />  
   
### Tree topology
   <img width="625" height="468" alt="image" src="https://github.com/user-attachments/assets/adc5343b-0278-4dc4-adb6-676cb1e4c352" />  
   
### Mesh topology
   <img width="768" height="549" alt="image" src="https://github.com/user-attachments/assets/d973c835-253b-412b-92b1-1b0a7c7199b3" />  
   
### Hybrid topology 
   <img width="1070" height="558" alt="image" src="https://github.com/user-attachments/assets/fe8473e1-113e-436d-a319-ee91b1df07db" />  
   
### comparison
Bus: Cheap, simple, unreliable    
Star: Easy management, central dependency  
Ring: Ordered access, low fault tolerance  
Mesh: High reliability, costly  
Tree: Scalable, backbone dependent  
Hybrid: Flexible, complex  

## Address 
1. IP address: Internet Protocol:  used by the router to forward the data, changes based on location
2. MAC address: Media Access Control: used by the switch to forward the data, does not change based on location
3. PORT address: used to reach the right process in a computer

## switching techniques  
Switching is the technique used to transfer data from a source to a destination through intermediate network nodes (switches).  

1. Circuit Switching  
   A dedicated physical path is established between sender and receiver before data transfer starts.  
   No data loss once connection is established  
   Reliable for real-time communication  
   Wastes resources when idle   
2. Message Switching (Store-and-Forward)  
   Entire message is sent to an intermediate node, stored, then forwarded.  
   Message stored fully before forwarding   
   Not suitable for real-time communication  
   Early telegraph systems  
3. Packet Switching  
   Data is divided into small packets, each sent independently through the network.  
   Possible packet loss or reordering  
   Scalable  
   Types:
   1. Datagram Packet Switching (connectionless)  
      Each packet can take a different path  
      No prior connection setup  
   2. Virtual Circuit Packet Switching (connection-oriented)  
      Logical path is established  
      All packets follow the same route  

   ## OSI model
   The OSI (Open Systems Interconnection) Model is a 7-layer reference framework developed by International Organization for Standardization to standardize how data is transmitted over a network.
   It's a guideline, not a protocol. 
   ### Order of layers
   <img width="713" height="768" alt="image" src="https://github.com/user-attachments/assets/c900c9a7-ed3e-4cdc-96f4-c0097ae6b8a0" />

   1. Application layer  
      Provides network services directly to user applications.  
      Key Functions:  
      1. File transfer  
      2. Email  
      3. Web services  
   2. Presentation layer  
      Formats and translates data for the application layer.  
      Key Functions:     
      1. Data encryption/decryption == SSL/TLS encryption      
      2. Data compression    
      3. Format translation (ASCII, JPEG, MP  
   3. Session layer  
      Manages sessions (connections) between applications.  
      Key Functions:  
      1. Session establishment  
      2. Session maintenance  
      3. Session termination  
      4. Checkpointing
      5. dialogue control
   4. Transport layer  
      Ensures reliable or fast delivery of data.  
      Key Functions:  
      1. Segmentation & reassembly  
      2. Flow control   
      3. Error control  
      4. TCP (reliable) UDP (fast, unreliable)  
   5. Network layer  
      Determines the best path for data delivery.  
      Key Functions:  
      1. Logical addressing (IP)  
      2. Routing  
      3. Packet forwarding  
   6. data link layer
      Ensures error-free transfer between adjacent nodes.  
      Key Functions:  
      1. Framing   
      2. MAC addressing  
      3. Error detection  
      4. Flow control  
   7. physical layer  
       Transmits raw bits over a physical medium.  
       Key Functions:  
       1. Bit transmission  
       2. Voltage levels  
       3. Cable types  
       4. Data rate

### packet construction and transmission
<img width="634" height="369" alt="image" src="https://github.com/user-attachments/assets/83b1d543-1922-4771-aa17-40bac032d569" />





   
