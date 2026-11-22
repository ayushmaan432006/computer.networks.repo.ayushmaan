# Experiment 2: Study of Basic Network Commands

## 1. Aim

To study and execute basic networking commands used to examine network configuration, test connectivity and troubleshoot network-related problems.

## 2. Requirements

- Computer/Laptop
- Cisco Packet Tracer
- Two PCs in Packet Tracer
- Network connection between the PCs

## 3. Theory

Network commands are instructions used to obtain information about network configuration, check connectivity and diagnose networking problems.

The following commands are commonly used:

### 1. ipconfig

Displays the IP configuration of a computer, including:
- IP Address
- Subnet Mask
- Default Gateway

**Command:**
```bash
ipconfig
```

### 2. ping

Checks connectivity between two devices by sending ICMP echo requests.

**Command:**
```bash
ping 192.168.1.2
```

A successful response indicates that the destination is reachable.

### 3. tracert

Displays the route taken by packets to reach a destination.

**Command:**
```bash
tracert 192.168.1.2
```

It is useful for identifying network routing problems.

### 4. arp

ARP stands for Address Resolution Protocol. It maps IP addresses to MAC addresses.

**Command:**
```bash
arp -a
```

Displays the ARP table.

### 5. netstat

Displays network connection information and statistics.

**Command:**
```bash
netstat
```

### 6. nslookup

Used to query DNS servers and obtain domain name information.

**Command:**
```bash
nslookup google.com
```

This requires an appropriately configured DNS server.
<img width="734" height="711" alt="image" src="https://github.com/user-attachments/assets/c9e13c85-47a4-49d5-a1fd-a771f4afeed1" />


## 4. Practical Implementation Using Cisco Packet Tracer

1. Open Cisco Packet Tracer.
2. Add two PCs to the workspace.
3. Connect the PCs through a network connection.
4. Configure the IP addresses:
   - PC0: 192.168.1.1
   - PC1: 192.168.1.2
5. Configure the subnet mask on both PCs as 255.255.255.0.
6. Open PC0.
7. Navigate to Desktop → Command Prompt.
8. Execute the following commands individually.

### Command 1: ipconfig
```bash
ipconfig
```
Displays the IP address, subnet mask and default gateway.

### Command 2: ping
```bash
ping 192.168.1.2
```
Checks connectivity between PC0 and PC1.

### Command 3: arp
```bash
arp -a
```
Displays the IP-to-MAC address mappings stored in the ARP table.

### Command 4: tracert
```bash
tracert 192.168.1.2
```
Displays the route to the destination.

### Command 5: netstat
```bash
netstat
```
Displays network connection information.

### Command 6: help
```bash
help
```
Displays the commands supported by the Packet Tracer command prompt.

**Note:** Packet Tracer supports a limited set of commands. Some commands available in Windows Command Prompt, including `nslookup`, may not be supported in its simulated environment.

## 5. Observation Table

| Command | Function |
|---|---|
| ipconfig | Displays IP configuration |
| ping | Tests network connectivity |
| arp -a | Displays ARP table |
| tracert | Traces the route to a destination |
| netstat | Displays network connection information |
| help | Displays available commands |

## 6. Result

Successfully studied and executed basic networking commands using Cisco Packet Tracer to examine IP configuration, test connectivity and understand network troubleshooting.

## 7. Conclusion

Basic networking commands help administrators monitor, configure and troubleshoot computer networks. The experiment provided practical knowledge of IP addressing, connectivity testing, ARP and network diagnostics.

## 8. Viva Questions

**Q1. What is an IP address?**  
An IP address is a logical address assigned to a device on a network for identification and communication.

**Q2. What is a subnet mask?**  
A subnet mask identifies the network and host portions of an IP address.

**Q3. What is the purpose of ping?**  
It checks whether a destination device is reachable over a network.

**Q4. What is TTL?**  
Time To Live is a field that limits the lifetime or number of routing hops of an IP packet.

**Q5. What is DNS?**  
Domain Name System translates domain names into IP addresses.

**Q6. What is DHCP?**  
Dynamic Host Configuration Protocol automatically assigns IP configuration to devices.

**Q7. What is ARP?**  
Address Resolution Protocol maps IPv4 addresses to MAC addresses on a local network.

**Q8. What is the difference between IP and MAC addresses?**  
An IP address is a logical network address, whereas a MAC address is a hardware-level address associated with a network interface.

**Q9. What is the purpose of tracert?**  
It identifies the route taken by packets to reach a destination.

**Q10. What is a default gateway?**  
It is the router used to forward traffic to destinations outside the local network.

**Q11. What happens when a ping request times out?**  
It means no response was received within the allowed time. Possible causes include connectivity problems, filtering or an unreachable destination.

**Q12. What is the difference between TCP and UDP?**  
TCP is connection-oriented and provides reliable delivery, whereas UDP is connectionless and does not guarantee delivery.
