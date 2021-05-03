# Principles of designing distributed data flow control systems with high resistance to malicious actions
## Paper Link

https://ieeexplore.ieee.org/document/8109565

## Research Questions

How to  design a distributed system for managing data flows and protecting computer networks from harmful effects

## Brief Summary

This paper has proposed a new approach to the development of a distributed data management system and protection against harmful effects. First, they have written about the disadvatanges of current approacches in this area. Modern distributed systems can be built both on the basis of **hierarchical** topology and **Peer-to-peer** technology. With a hierarchical topology, a device is selected to be a network master which can manage the network and make a decision. In this kind of distributed systems managing the entire system of protection and decision-making are performed by one device, and in case of its failure the network becomes unable to coordinate and detect attacks.

Another way is to build a protection system using Peer-topeer technology. In this case, all devices perform the same function and communicate among themselves for joint decision making. the drawback of this method is that each device is forced not only to analyze a significant amount of traffic, but also to process data received from other peer nodes, which significantly increases the load.

The proposed approach is based on Fog computing technology, which itself is based on using the computing power of physical devices. Thus, the protection
system will consist mainly of two groups of devices: 

- the nodes of the protection system: A segment of the local network which must to be protected will be assigned to one of the protection nodes. To get decision for the entire network, nodes must exchange data among themselves.

- the Fog Nodes: Divide Fog Nodes into **groups**, each of which would analyze data transmitted by defined protocol. Distribution by groups should be made at each start of the network. When adding new nodes to the network that can perform
Fog Node functions, they can join the **most loaded groups**. If you disable one of the Fog Nodes as a result of an external action (for example, shutdown by the user), the functions must be **redistributed**.

For each individual protocol, you should maintain a simple query database, which includes fields such as source and destination IP addresses and ports. When you **send** a request to an external network, the security node creates a new entry in the database that is distributed to the Fog Nodes. **Upon receipt** of the incoming packet, the security node checks the protocol on which the packet was sent, and passes the header of this packet to one of the Fog Nodes. The tasks of Fog Node are:

- Comparing addresses and ports with entries in the database 
- Analyzing flags that can indicate the sending of packets with specific content

After analyzing each packet, the Fog Node sends a preliminary decision to the security system node whether this packet can be recognized as legitimate or should be rejected. Packages with specific content should be labeled in a
special way and carried out additional analysis.

It has been suggested that to solve the problems of the distribution of functions, it is possible to use the principles underlying the SDN technology.

## Findings

- A new approach to the development of a distributed data management system and protection against harmful effects 

## Suggested Future Work

- The creation of a protocol for data exchange between elements of the protection system
- Use the developed system, first of all, to increase the level of security of computer networks.

## Relevance to my work

Got idea about the possibility of distributing security tasks among the devices