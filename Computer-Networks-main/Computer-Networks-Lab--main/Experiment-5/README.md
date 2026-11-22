# Experiment 5: Connect the Computers in Local Area Network (LAN)

## 1. Aim

To connect multiple computers in a Local Area Network using a network switch and establish communication between them.

## 2. Requirements

- Cisco Packet Tracer
- Four PCs
- One 2960 Switch
- Copper Straight-Through cables

## 3. Theory

A Local Area Network (LAN) is a computer network that connects devices within a limited geographical area, such as a laboratory, office or building.

A switch is used to connect multiple computers in a LAN. It forwards data frames to the appropriate destination using MAC addresses.

### Star Topology

In this experiment, a star topology is used, where all computers are connected to a central switch.

Advantages:
- Easy to install and manage.
- Easy to identify connection failures.
- Failure of one cable does not affect other connected devices.

## 4. Practical Implementation Using Cisco Packet Tracer

### Step 1: Create the Network Topology

1. Open Cisco Packet Tracer.
2. Add four PCs and one 2960 switch.
3. Arrange the devices in a star topology.

### Step 2: Connect the Computers

Use Copper Straight-Through cables to establish the following connections:

| Computer | Switch Port |
|---|---|
| PC0 | FastEthernet0/1 |
| PC1 | FastEthernet0/2 |
| PC2 | FastEthernet0/3 |
| PC3 | FastEthernet0/4 |

### Step 3: Configure IP Addresses

Configure the following static IP addresses:

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.10.1 | 255.255.255.0 |
| PC1 | 192.168.10.2 | 255.255.255.0 |
| PC2 | 192.168.10.3 | 255.255.255.0 |
| PC3 | 192.168.10.4 | 255.255.255.0 |

To configure an IP address:

1. Click the PC.
2. Navigate to Desktop → IP Configuration.
3. Select Static.
4. Enter the IP address and subnet mask.

### Step 4: Test Connectivity

Open PC0 → Desktop → Command Prompt.

Execute:

```bash
ping 192.168.10.2
```

Test connectivity with the remaining computers:

```bash
ping 192.168.10.3
ping 192.168.10.4
```

Successful replies indicate communication between the computers.

### Step 5: Observe Packet Transmission

1. Switch to Simulation mode.
2. Select Add Simple PDU.
3. Click PC0 as the source and PC1 as the destination.
4. Use Auto Capture/Play to observe packet transmission.

## 5. Observation Table

| Source | Destination | Expected Result |
|---|---|---|
| PC0 | PC1 | Successful |
| PC0 | PC2 | Successful |
| PC0 | PC3 | Successful |

## 6. Result

Successfully connected multiple computers in a Local Area Network using a switch and verified communication using the ping command.

## 7. Conclusion

A LAN enables multiple computers to communicate within a limited geographical area. The experiment demonstrated star topology, switch-based connectivity, IP addressing and packet transmission.

## 8. Viva Questions

**Q1. What is LAN?**  
LAN stands for Local Area Network. It connects devices within a limited geographical area.

**Q2. What is a switch?**  
A switch connects multiple devices in a LAN and forwards frames using MAC addresses.

**Q3. What is star topology?**  
A topology in which all devices are connected to a central device such as a switch.

**Q4. What is the advantage of star topology?**  
Failure of one device or cable generally does not affect the other connections.

**Q5. What is the purpose of an IP address?**  
It identifies a device on an IP network.

**Q6. What is a MAC address?**  
A hardware-level address associated with a network interface.

**Q7. What is the purpose of ping?**  
It tests connectivity between network devices.

**Q8. Can computers communicate without a router in a LAN?**  
Yes, devices in the same IP subnet can communicate through a switch without a router.

**Q9. What is an ICMP packet?**  
ICMP is a network-layer protocol used for error reporting and diagnostic operations such as ping.

**Q10. What happens if the central switch fails?**  
Communication between devices connected through that switch is disrupted.
