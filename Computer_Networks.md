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

### Data Flow
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

### Elements of protocol 
1. message encoding
2. message formatting and encapsulation
3. message timing
4. message size
5. message delivery options
   a. Unicast: when the sender sends data to a single targeted system.   
   b. Multicast: when the sender sends data to more than one targeted system.  
   c. Broadcast: when the sender sends data to all devices without knowing the target.

### Components of a computer network
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
   


   
