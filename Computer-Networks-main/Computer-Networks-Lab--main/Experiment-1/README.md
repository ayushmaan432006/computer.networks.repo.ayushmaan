# Experiment 1: Study of Network Cables and Implementation of Straight-Through and Crossover Cables

## 1. Aim
To study different types of network cables and practically implement straight-through and crossover Ethernet cables using an RJ45 connector and a crimping tool.

## 2. Requirements
- UTP Ethernet cable (Cat5/Cat5e)
- RJ45 connectors
- Crimping tool
- Wire stripper or cable cutter
- LAN cable tester

## 3. Theory

Network cables are used to establish communication between computers and other networking devices.

### Types of Network Cables

1. **UTP (Unshielded Twisted Pair):** Consists of four pairs of twisted copper wires without additional metallic shielding. Commonly used in LANs.
2. **STP (Shielded Twisted Pair):** Contains additional shielding to reduce electromagnetic interference.
3. **Coaxial Cable:** Consists of a central conductor surrounded by insulation and metallic shielding.
4. **Optical Fibre Cable:** Transmits data using light signals through optical fibres.

### RJ45 Connector
RJ45 is an 8-pin modular connector commonly used for Ethernet networking. It connects network cables to computers, routers and switches.

### Wiring Standards

Two wiring standards are commonly used for Ethernet cables:

**T568A Standard**

| Pin | Wire Colour |
|---|---|
| 1 | White-Green |
| 2 | Green |
| 3 | White-Orange |
| 4 | Blue |
| 5 | White-Blue |
| 6 | Orange |
| 7 | White-Brown |
| 8 | Brown |

**T568B Standard**

| Pin | Wire Colour |
|---|---|
| 1 | White-Orange |
| 2 | Orange |
| 3 | White-Green |
| 4 | Blue |
| 5 | White-Blue |
| 6 | Green |
| 7 | White-Brown |
| 8 | Brown |

### Types of Ethernet Cables

**1. Straight-Through Cable**

A straight-through cable uses the same wiring standard at both ends.

- First end: T568B
- Second end: T568B
- Traditionally used to connect different types of networking devices, such as a computer to a switch.
  <img width="1597" height="940" alt="image" src="https://github.com/user-attachments/assets/8ebbe9b6-1313-424f-9313-2c17056f79bb" />

**2. Crossover Cable**

A crossover cable uses different wiring standards at the two ends.

- First end: T568A
- Second end: T568B
- Traditionally used to connect similar devices, such as two computers directly.
<img width="1865" height="1006" alt="image" src="https://github.com/user-attachments/assets/1d23d793-c6f2-43a5-b500-9ea9b0e97e09" />
## 4. Procedure

### Part A: Making a Straight-Through Cable

1. Take a UTP Ethernet cable of the required length.
2. Remove approximately 2–3 cm of the outer insulation using a wire stripper.
3. Separate and untwist the eight individual wires.
4. Arrange the wires according to the T568B colour sequence.
5. Straighten the wires and trim them evenly.
6. Insert all eight wires into an RJ45 connector in the correct order.
7. Ensure that the wires reach the end of the connector and the outer jacket is secured inside it.
8. Place the RJ45 connector inside the crimping tool.
9. Squeeze the crimping tool firmly to attach the connector.
10. Repeat the same procedure at the other end using the T568B standard.
11. Test the cable using a LAN cable tester.

### Part B: Making a Crossover Cable

1. Take another UTP Ethernet cable.
2. Strip the outer insulation at both ends.
3. Separate and straighten the eight wires.
4. Arrange the wires at the first end according to the T568A standard.
5. Insert the wires into an RJ45 connector and crimp it.
6. Arrange the wires at the second end according to the T568B standard.
7. Insert the wires into another RJ45 connector and crimp it.
8. Test the cable using a LAN cable tester.

## 5. Observation

| Cable Type | First End | Second End |
|---|---|---|
| Straight-Through | T568B | T568B |
| Crossover | T568A | T568B |

**LAN Tester Observations:**

- Straight-through cable: Pin 1 connects to 1, 2 to 2, and so on up to 8 to 8.
- Crossover cable: Pins 1 and 3 are exchanged, and pins 2 and 6 are exchanged. The remaining pins connect straight through.

## 6. Applications

- Straight-through cables are traditionally used to connect computers to switches and routers to switches.
- Crossover cables are traditionally used to connect similar networking devices.
- Ethernet cables are used to establish wired Local Area Networks (LANs).

## 7. Result

Successfully studied different types of network cables and implemented straight-through and crossover Ethernet cables using RJ45 connectors and a crimping tool.

## 8. Conclusion

Network cables play an important role in establishing wired communication between devices. Straight-through and crossover cables differ in their wiring arrangements and applications. The practical helped understand Ethernet wiring standards, RJ45 connectors and cable crimping techniques.

## 9. Viva Questions

**Q1. What is UTP?**  
UTP stands for Unshielded Twisted Pair. It consists of twisted copper wire pairs without additional shielding.

**Q2. What is RJ45?**  
RJ45 is an 8-pin modular connector commonly used in Ethernet networks.

**Q3. What is the difference between straight-through and crossover cables?**  
A straight-through cable has the same wiring standard at both ends, whereas a crossover cable has T568A at one end and T568B at the other.

**Q4. What is the purpose of a crimping tool?**  
It is used to attach RJ45 connectors securely to Ethernet cables.

**Q5. How many wires are present in an Ethernet cable?**  
Eight individual wires arranged in four twisted pairs.

**Q6. What is the purpose of a LAN tester?**  
It checks the continuity and correct pin connections of an Ethernet cable.

**Q7. What are T568A and T568B?**  
They are standard wiring schemes that define the colour arrangement of Ethernet cable wires.

**Q8. Which cable is traditionally used to connect two computers directly?**  
A crossover cable.

**Q9. Which cable is traditionally used to connect a computer to a switch?**  
A straight-through cable.

**Q10. What is the function of twisted pairs?**  
Twisting helps reduce electromagnetic interference and crosstalk.
