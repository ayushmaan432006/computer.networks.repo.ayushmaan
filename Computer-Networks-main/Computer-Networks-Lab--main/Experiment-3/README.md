# Experiment 3: Study and Installation of Various Network Devices

## 1. Aim

To study different networking devices, understand their functions and simulate their installation and interconnection using Cisco Packet Tracer.

## 2. Requirements

- Computer/Laptop
- Cisco Packet Tracer
- PCs
- Hub
- Switch
- Router
- Server
- Wireless Access Point
- Appropriate network cables

## 3. Theory

Networking devices are hardware components used to connect computers and other devices, enable data transmission and manage communication within a network.

### 1. Hub
- Connects multiple devices in a LAN.
- Broadcasts incoming data to all connected ports.
- Operates at the Physical Layer (Layer 1).

### 2. Switch
- Connects multiple devices within a LAN.
- Uses MAC addresses to forward data frames to the appropriate port.
- Operates primarily at the Data Link Layer (Layer 2).

### 3. Router
- Connects different networks.
- Forwards packets using IP addresses.
- Operates at the Network Layer (Layer 3).

### 4. Modem
- Performs modulation and demodulation.
- Enables communication through an ISP's transmission medium.

### 5. Repeater
- Regenerates network signals.
- Extends the transmission distance.
- Operates at the Physical Layer.

### 6. Wireless Access Point
- Allows wireless devices to connect to a wired network.
- Provides wireless network connectivity.

### 7. Network Interface Card (NIC)
- Provides network connectivity to a computer.
- Contains a MAC address used for communication.

## 4. Practical Implementation Using Cisco Packet Tracer

### Step 1: Add Network Devices

Open Cisco Packet Tracer and add the following devices:

- Two PCs
- One Server
- One Hub
- One Switch (2960)
- One Router
- One Wireless Access Point

### Step 2: Connect the Devices

Use the Connections option (lightning bolt) and select Copper Straight-Through cables.

Establish the following connections:

| From | To |
|---|---|
| PC0 | Switch |
| PC1 | Switch |
| Server | Switch |
| Switch | Router |
| Hub | Switch |
| Access Point | Switch |

### Step 3: Configure IP Addresses

Configure the following IP addresses:

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |
| Server | 192.168.1.3 | 255.255.255.0 |

To configure an IP address:

1. Click the device.
2. Navigate to Desktop.
3. Open IP Configuration.
4. Enter the IP address and subnet mask.

### Step 4: Observe Network Devices

Open each device and examine its configuration options, ports and interfaces.

- PC: Desktop, Config and Physical tabs.
- Switch: Config and CLI tabs.
- Router: Config and CLI tabs.
- Server: Services, Config and Desktop tabs.
- Access Point: Config and Physical tabs.

### Step 5: Test Connectivity

Open PC0 → Desktop → Command Prompt.

Execute:

```bash
ping 192.168.1.2
```

To test connectivity with the server:

```bash
ping 192.168.1.3
```

Successful replies indicate that communication between the devices is working.

**Note:** This is a basic LAN connectivity demonstration. Router and access point connections are included for device identification and observation; their advanced configurations are not part of this basic test.

## 5. Observation Table

| Device | Function | OSI Layer |
|---|---|---|
| Hub | Broadcasts data | Physical |
| Switch | Forwards frames using MAC addresses | Data Link |
| Router | Connects different networks | Network |
| Repeater | Regenerates signals | Physical |
| Modem | Modulates and demodulates signals | Depends on implementation |
| Access Point | Provides wireless connectivity | Primarily Data Link |
| NIC | Provides network connectivity | Physical and Data Link |

## 6. Applications

- Hubs and switches are used to connect devices in LANs.
- Routers connect multiple networks.
- Repeaters extend network coverage.
- Modems provide internet connectivity.
- Wireless access points provide Wi-Fi connectivity.
- NICs enable computers to communicate over networks.

## 7. Result

Successfully studied various networking devices, understood their functions and simulated their installation and interconnection using Cisco Packet Tracer.

## 8. Conclusion

Different networking devices perform different functions in computer networks. The experiment provided practical knowledge of hubs, switches, routers, repeaters, modems, wireless access points and network interface cards.

## 9. Viva Questions

**Q1. What is a hub?**  
A hub is a networking device that connects multiple devices and broadcasts incoming data to all its ports.

**Q2. What is a switch?**  
A switch connects devices in a LAN and forwards frames using MAC addresses.

**Q3. What is a router?**  
A router connects different networks and forwards packets using IP addresses.

**Q4. What is the difference between a hub and a switch?**  
A hub broadcasts data to all ports, whereas a switch forwards data to the appropriate destination port.

**Q5. What is the function of a repeater?**  
It regenerates signals to extend network transmission distance.

**Q6. What is a modem?**  
A modem performs modulation and demodulation to enable communication over a transmission medium.

**Q7. What is a NIC?**  
A Network Interface Card provides network connectivity to a computer.

**Q8. What is a MAC address?**  
A MAC address is a hardware-level address associated with a network interface.

**Q9. What is a wireless access point?**  
It allows wireless devices to connect to a wired network.

**Q10. At which OSI layer does a router operate?**  
Network Layer (Layer 3).

**Q11. At which OSI layer does a switch operate?**  
Data Link Layer (Layer 2), for a standard Layer 2 switch.

**Q12. What is the purpose of a server?**  
A server provides services and resources to other computers called clients.
