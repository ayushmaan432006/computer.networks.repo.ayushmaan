# Experiment 6: Router Configuration using Cisco Packet Tracer

## Aim
To configure a router and establish communication between two different networks using Cisco Packet Tracer.

## Requirements
- Cisco Packet Tracer
- 1 Cisco 1941 Router
- 2 PCs
- Copper Straight-Through cables

## Theory
A router is a networking device that connects different networks and forwards data packets between them. Each router interface is assigned an IP address belonging to the network connected to it.

## Procedure

1. Add one Cisco 1941 router and two PCs.
2. Connect PC0 to GigabitEthernet0/0 and PC1 to GigabitEthernet0/1 using Copper Straight-Through cables.
3. Open the router CLI and configure its interfaces:

```bash
enable
configure terminal

interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit

interface gigabitEthernet 0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
exit

end
show ip interface brief
```

4. Configure PC0:
   - IP address: 192.168.1.2
   - Subnet mask: 255.255.255.0
   - Default gateway: 192.168.1.1

5. Configure PC1:
   - IP address: 192.168.2.2
   - Subnet mask: 255.255.255.0
   - Default gateway: 192.168.2.1

6. Open the command prompt on PC0 and test connectivity:

```bash
ping 192.168.2.2
```

## Observations
- Both router interfaces are configured with different network addresses.
- The router interfaces become active after executing `no shutdown`.
- Successful ping replies indicate communication between the two networks.

## Result
Successfully configured a Cisco 1941 router and established communication between two different networks.

## Viva Questions
1. What is a router?
2. What is the purpose of the `no shutdown` command?
3. What is a default gateway?
4. What is the difference between a router and a switch?
5. What does the `show ip interface brief` command display?
6. Why are different network addresses assigned to the two router interfaces?
