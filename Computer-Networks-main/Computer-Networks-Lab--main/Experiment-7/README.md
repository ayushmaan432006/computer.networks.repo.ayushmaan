# Experiment 7: Establish Peer-to-Peer Network Connection Using Switch and Router

## Aim
To establish a peer-to-peer network connection between two computers using a switch and router in a LAN.

## Requirements
- Cisco Packet Tracer
- 2 PCs
- 1 Cisco 2960 Switch
- 1 Cisco 1941 Router
- Copper Straight-Through cables

## Theory
A peer-to-peer network allows two or more computers to communicate and share resources directly.

A switch connects multiple computers within a LAN, while a router connects the LAN to other networks and can act as the default gateway.

## Procedure

1. Add two PCs, one Cisco 2960 switch and one Cisco 1941 router.
2. Connect both PCs to the switch using Copper Straight-Through cables.
3. Connect the switch to the router's GigabitEthernet0/0 interface.
4. Configure the router:

```bash
enable
configure terminal
interface gigabitEthernet 0/0
ip address 192.168.3.1 255.255.255.0
no shutdown
exit
end
show ip interface brief
```

5. Configure PC0:
   - IP address: 192.168.3.2
   - Subnet mask: 255.255.255.0
   - Default gateway: 192.168.3.1

6. Configure PC1:
   - IP address: 192.168.3.3
   - Subnet mask: 255.255.255.0
   - Default gateway: 192.168.3.1

7. Open PC0's Command Prompt and execute:

```bash
ping 192.168.3.3
```

8. Verify communication with the router:

```bash
ping 192.168.3.1
```

## Observations
- Both PCs are connected to the same switch.
- The router is connected to the switch and configured as the default gateway.
- Successful ping replies confirm communication between the two PCs.

## Result
Successfully established peer-to-peer communication between two computers using a switch and router in a LAN.

## Viva Questions
1. What is a peer-to-peer network?
2. What is the role of a switch in a LAN?
3. What is the role of a router?
4. What is a default gateway?
5. What is the purpose of the ping command?
6. Can two computers in the same subnet communicate without a router?
