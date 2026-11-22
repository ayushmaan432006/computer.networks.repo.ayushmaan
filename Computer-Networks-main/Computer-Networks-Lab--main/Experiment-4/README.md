# Experiment 4: Study and Configuration of Network IP Addressing

## 1. Aim

To study IP addressing and configure IP addresses, subnet masks and default gateways on computers using Cisco Packet Tracer.

## 2. Requirements

- Computer/Laptop
- Cisco Packet Tracer
- Two PCs
- One 2960 Switch
- Copper Straight-Through cables

## 3. Theory

An IP (Internet Protocol) address is a logical address assigned to a device connected to a network. It is used to identify devices and enable communication between them.

### Important Components

1. **IP Address:** Uniquely identifies a device on an IP network.
2. **Subnet Mask:** Identifies the network and host portions of an IP address.
3. **Default Gateway:** The router address used to communicate with devices outside the local network.

### Types of IP Addresses

- **IPv4:** Uses a 32-bit address represented in dotted decimal notation.
- **IPv6:** Uses a 128-bit address represented in hexadecimal notation.

## 4. Practical Implementation Using Cisco Packet Tracer

### Step 1: Create the Network Topology

1. Open Cisco Packet Tracer.
2. Add two PCs (PC0 and PC1).
3. Add one 2960 switch.
4. Connect both PCs to the switch using Copper Straight-Through cables.

### Step 2: Configure PC0

1. Click PC0.
2. Navigate to Desktop → IP Configuration.
3. Select Static.
4. Enter the following configuration:

| Parameter | Value |
|---|---|
| IP Address | 192.168.1.1 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 192.168.1.254 |

### Step 3: Configure PC1

1. Click PC1.
2. Navigate to Desktop → IP Configuration.
3. Select Static.
4. Enter:

| Parameter | Value |
|---|---|
| IP Address | 192.168.1.2 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 192.168.1.254 |

The default gateway is optional for communication within the same subnet.

### Step 4: Test Connectivity

1. Open PC0.
2. Navigate to Desktop → Command Prompt.
3. Execute:

```bash
ping 192.168.1.2
```

Successful replies indicate that both computers can communicate.

### Step 5: Verify IP Configuration

Execute the following command on both PCs:

```bash
ipconfig
```

Verify the IP addresses and subnet masks.

## 5. Observation Table

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |

Both computers belong to the same network, 192.168.1.0/24.

## 6. Result

Successfully studied and configured IP addressing on computers using Cisco Packet Tracer and verified connectivity using the ping command.

## 7. Conclusion

IP addressing enables devices to communicate over computer networks. The experiment demonstrated static IP configuration, subnet masks, default gateways and connectivity testing.

## 8. Viva Questions

**Q1. What is an IP address?**  
An IP address is a logical address assigned to a device for identification and communication over a network.

**Q2. What is IPv4?**  
IPv4 is a 32-bit addressing scheme represented using four decimal octets.

**Q3. What is IPv6?**  
IPv6 is a 128-bit addressing scheme designed to provide a much larger address space.

**Q4. What is a subnet mask?**  
A subnet mask identifies the network and host portions of an IP address.

**Q5. What is the default gateway?**  
It is the router used to communicate with devices outside the local network.

**Q6. What is static IP addressing?**  
It is the process of manually assigning an IP address to a device.

**Q7. What is dynamic IP addressing?**  
It is the automatic assignment of IP addresses using DHCP.

**Q8. What is the purpose of the ping command?**  
It tests connectivity between two network devices.

**Q9. What is a private IP address?**  
An IP address reserved for use within private networks.

**Q10. What is the subnet mask of a /24 network?**  
255.255.255.0.
