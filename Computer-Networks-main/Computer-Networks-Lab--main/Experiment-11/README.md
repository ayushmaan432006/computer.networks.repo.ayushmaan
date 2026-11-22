# Experiment 11: Study of Socket Programming and Client-Server Model

## Aim
To study client-server communication and observe TCP-based application communication using Cisco Packet Tracer.

## Requirements
- Cisco Packet Tracer
- 1 PC
- 1 Cisco 2960 Switch
- 1 Server-PT
- Copper Straight-Through cables

## Theory
Socket programming enables applications to communicate over a network.

A socket is an endpoint used for sending and receiving data. Communication generally involves an IP address and a port number.

The client-server model consists of:
- Client: Initiates communication.
- Server: Waits for requests and provides services.

FTP (File Transfer Protocol) is a client-server application that uses TCP for reliable communication.

TCP establishes a connection using a three-way handshake:
1. SYN
2. SYN-ACK
3. ACK

## Procedure

1. Add one PC, one switch and one Server-PT.
2. Connect the PC and server to the switch using Copper Straight-Through cables.
3. Configure PC0 with IP address `192.168.20.1` and subnet mask `255.255.255.0`.
4. Configure Server0 with IP address `192.168.20.2` and subnet mask `255.255.255.0`.
5. Open Server0 → Services → FTP.
6. Enable FTP and create a user with username `student` and password `123`.
7. Open PC0 → Desktop → Command Prompt.
8. Connect to the FTP server:

```bash
ftp 192.168.20.2
```

9. Enter the username and password.
10. Execute the `dir` command to view available files.
11. Switch to Simulation Mode and observe TCP and FTP packets.

## Observations
- The PC acts as the FTP client.
- The server provides the FTP service.
- The client establishes a TCP connection with the server.
- TCP connection establishment can be observed through SYN, SYN-ACK and ACK packets.

## Result
Successfully simulated client-server communication using FTP and observed TCP connection establishment in Cisco Packet Tracer.

## Viva Questions
1. What is socket programming?
2. What is a socket?
3. What is the client-server model?
4. What is the difference between a client and a server?
5. What is TCP?
6. What is FTP?
7. What is a port number?
8. What is the TCP three-way handshake?
9. What are SYN, SYN-ACK and ACK?
10. What is the difference between TCP and UDP?
