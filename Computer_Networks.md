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
3. PORT address: used to reach to right process in a computer

   
   



   
