# Experiment 8: Examine Network Address Translation (NAT)

## Aim
To study and configure Network Address Translation (NAT) using Cisco Packet Tracer.

## Requirements
- Cisco Packet Tracer
- 1 PC
- 1 Cisco 2960 Switch
- 2 Cisco 1941 Routers
- 1 Server
- Copper Straight-Through cables

## Theory
Network Address Translation (NAT) is used to translate private IP addresses into public IP addresses when devices communicate with external networks.

PAT (Port Address Translation), also called NAT Overload, allows multiple devices to share a single public IP address by using different port numbers.

## Procedure

1. Create a topology consisting of a PC, switch, two routers and a server.
2. Connect the devices using Copper Straight-Through cables.
3. Configure Router0 with:
   - Inside interface: 192.168.1.1
   - Outside interface: 200.0.0.1
4. Configure NAT on Router0:

```bash
access-list 1 permit 192.168.1.0 0.0.0.255
ip nat inside source list 1 interface gigabitEthernet 0/1 overload
```

5. Configure the default route:

```bash
ip route 0.0.0.0 0.0.0.0 200.0.0.2
```

6. Configure Router1:
   - G0/0: 200.0.0.2
   - G0/1: 203.0.113.1

7. Configure PC0:
   - IP: 192.168.1.2
   - Gateway: 192.168.1.1

8. Configure Server0:
   - IP: 203.0.113.2
   - Gateway: 203.0.113.1

9. Test connectivity from PC0:

```bash
ping 203.0.113.2
```

10. Verify NAT translations on Router0:

```bash
show ip nat translations
show ip nat statistics
```

## Observations
- The PC uses a private IP address.
- Router0 translates the private source address into its outside interface address.
- NAT translation entries can be viewed using the `show ip nat translations` command.

## Result
Successfully configured and examined NAT Overload (PAT) using Cisco Packet Tracer.

## Viva Questions
1. What is NAT?
2. Why is NAT used?
3. What is the difference between static NAT and dynamic NAT?
4. What is PAT?
5. What is a private IP address?
6. What is the purpose of `ip nat inside`?
7. What is the purpose of `ip nat outside`?
8. Which command displays NAT translations?
