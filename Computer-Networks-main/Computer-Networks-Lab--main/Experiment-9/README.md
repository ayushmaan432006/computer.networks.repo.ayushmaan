# Experiment 9: Simulation of Routing Protocols

## Aim
To simulate and study the implementation of a dynamic routing protocol using Cisco Packet Tracer.

## Requirements
- Cisco Packet Tracer
- 2 Cisco 1941 Routers
- 2 Cisco 2960 Switches
- 2 PCs
- Copper Straight-Through cables

## Theory
Routing protocols allow routers to exchange routing information and determine paths for forwarding packets between different networks.

RIP (Routing Information Protocol) is a distance-vector routing protocol that uses hop count as its routing metric. RIP version 2 supports classless routing and subnet masks.

## Procedure

1. Create a topology with two routers, two switches and two PCs.
2. Connect each PC to a switch and each switch to its respective router.
3. Connect the two routers using their GigabitEthernet interfaces.
4. Configure Router0:

```bash
enable
configure terminal
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
interface gigabitEthernet 0/1
ip address 10.0.0.1 255.255.255.252
no shutdown
exit
router rip
version 2
no auto-summary
network 192.168.1.0
network 10.0.0.0
end
```

5. Configure Router1:

```bash
enable
configure terminal
interface gigabitEthernet 0/0
ip address 10.0.0.2 255.255.255.252
no shutdown
exit
interface gigabitEthernet 0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
exit
router rip
version 2
no auto-summary
network 192.168.2.0
network 10.0.0.0
end
```

6. Configure PC0 with IP address `192.168.1.2`, subnet mask `255.255.255.0` and gateway `192.168.1.1`.
7. Configure PC1 with IP address `192.168.2.2`, subnet mask `255.255.255.0` and gateway `192.168.2.1`.
8. Verify routing tables:

```bash
show ip route
```

9. Test connectivity from PC0:

```bash
ping 192.168.2.2
```

## Observations
- Both routers exchange routing information using RIP version 2.
- Routes learned through RIP are marked with `R` in the routing table.
- Successful ping replies confirm communication between the two networks.

## Result
Successfully simulated dynamic routing using RIP version 2 in Cisco Packet Tracer.

## Viva Questions
1. What is a routing protocol?
2. What is RIP?
3. What is the difference between static and dynamic routing?
4. What is the maximum hop count in RIP?
5. What is the difference between RIP version 1 and version 2?
6. What does the `no auto-summary` command do?
7. What does the letter R represent in the routing table?
8. Which command displays the routing table?
