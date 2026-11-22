# Experiment 10: Connection-Oriented Client-Server Applications using TCP and UDP

## Aim
To study client-server communication and observe the use of TCP and UDP protocols using Cisco Packet Tracer.

## Requirements
- Cisco Packet Tracer
- 1 PC (Client)
- 1 Server-PT (Server)
- 1 Cisco 2960 Switch
- Copper Straight-Through cables

## Theory
The client-server model consists of a client that requests services and a server that provides them.

**TCP (Transmission Control Protocol):**
- Connection-oriented protocol.
- Provides reliable data transmission.
- Used by HTTP and FTP.

**UDP (User Datagram Protocol):**
- Connectionless protocol.
- Does not guarantee delivery.
- Commonly used by DNS queries.

## Procedure

1. Add one PC, one Cisco 2960 switch and one Server-PT.
2. Connect the PC and server to the switch using Copper Straight-Through cables.
3. Configure Server0:
   - IP address: `192.168.10.2`
   - Subnet mask: `255.255.255.0`
   - DNS server: `192.168.10.2`
4. Configure PC0:
   - IP address: `192.168.10.1`
   - Subnet mask: `255.255.255.0`
   - DNS server: `192.168.10.2`
5. Enable HTTP under Server0 → Services → HTTP.
6. Enable DNS under Server0 → Services → DNS.
7. Add a DNS A record:
   - Name: `www.lab.com`
   - Address: `192.168.10.2`
8. Open the web browser on PC0 and visit:

```text
http://www.lab.com
```

9. Switch to Simulation Mode and enable DNS and HTTP event filters.
10. Observe the packets using Capture / Forward.

## Observations
- DNS queries use UDP.
- HTTP communication uses TCP.
- The client successfully accesses the server using its domain name.

## Result
Successfully configured a client-server application and observed TCP and UDP communication using Cisco Packet Tracer.

## Viva Questions
1. What is the client-server model?
2. What is TCP?
3. What is UDP?
4. What is the difference between TCP and UDP?
5. Why is TCP called connection-oriented?
6. What is the purpose of DNS?
7. Which transport protocol does HTTP use?
8. What are the default port numbers of HTTP and DNS?
