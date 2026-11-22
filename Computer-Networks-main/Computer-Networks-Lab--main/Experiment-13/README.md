# Experiment 13: DHCP Server Implementation

## Aim
To implement a DHCP server using Cisco Packet Tracer and automatically assign IP addresses to client computers.

## Requirements
- Cisco Packet Tracer
- 1 Server-PT
- 1 Cisco 2960 Switch
- 3 PCs
- Copper Straight-Through cables

## Theory
DHCP stands for Dynamic Host Configuration Protocol. It automatically assigns IP addresses and other network configuration parameters to devices on a network.

DHCP follows the DORA process:
1. Discover
2. Offer
3. Request
4. Acknowledge

DHCP uses UDP port 67 on the server and UDP port 68 on the client.

## Procedure

1. Add one Server-PT, one Cisco 2960 switch and three PCs.
2. Connect all devices to the switch using Copper Straight-Through cables.
3. Configure Server0 with static IP address `192.168.10.10` and subnet mask `255.255.255.0`.
4. Open Server0 → Services → DHCP.
5. Enable DHCP.
6. Configure the DHCP pool:
   - Pool Name: LAN
   - Default Gateway: 192.168.10.1
   - DNS Server: 8.8.8.8
   - Start IP Address: 192.168.10.100
   - Subnet Mask: 255.255.255.0
   - Maximum Users: 50
7. Click Add.
8. Open each PC → Desktop → IP Configuration.
9. Select DHCP to obtain an IP address automatically.
10. Verify the assigned addresses using:

```bash
ipconfig
```

11. Test connectivity between PCs using:

```bash
ping 192.168.10.101
```

## Observations
- The server automatically assigns IP addresses to the client PCs.
- Each client receives a unique IP address.
- DHCP eliminates the need for manual IP configuration.

## Result
Successfully implemented a DHCP server and assigned IP addresses dynamically to client computers using Cisco Packet Tracer.

## Viva Questions

1. What is DHCP?
2. What is the full form of DHCP?
3. What is the DORA process?
4. What is the difference between static and dynamic IP addressing?
5. Which transport protocol does DHCP use?
6. What are DHCP server and client port numbers?
7. What is a DHCP scope or pool?
8. What happens when a DHCP server is unavailable?
9. What is a DHCP lease?
10. What is the purpose of the subnet mask?
