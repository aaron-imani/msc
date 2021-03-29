# MDNS Based Automatic Discovery Method In Optical NMS
## Paper Link

https://ieeexplore.ieee.org/document/8121329

## Research Questions

- How to decrease automatic discovery time in the network management system?

## Brief Summary

The paper addresses reducing the time needed for topological discovery in network management systems. It has been mentioned that the common way to discover devices in a network automatically is by using the `ping` method that is one of the oldest and most widely used techniques in IP network. The idea is to use *ICMP echo replied messages* to determine whether the host is reachable. It also gives information about the distance of a node by calculating round-trip time (RTT).

There are some problems with this technique:

1- By growing the network, it takes much time to ping every IP address in the network one by one.

2- If the receiver node is not accessible, the sender should wait for a while to timeout, typically 2 seconds. Hence, using the Ping method is relatively inefficient, specifically when sending ping messages to many pending IP addresses.

3- Due to the long detection period and large network load, it is not proper for real-time topological discovery.

The proposed methodology by the paper is an mDNS-based approach. Briefly, in the proposed technique, a server asks the devices their IP addresses, port, and the services they provide. Then, it will store the responses in a database. When a device requests the server for a specific service, the server will respond to it with the corresponding information found in the database by executing a query on it.

Both the `Ping` method and the proposed method have been tested in a LAN network to measure the time needed to collect all IP nodes and services. The results show that the time needed by the MDNS-based method is 30% lower than the time `Ping` method needs to accomplish the same task.

## Findings

- A more efficient way to discover network devices automatically compared with the `Ping` method

## Suggested Future Work

None

## Relevance to my work

In my thesis, I want to remove Tango Host's role. For this purpose, I need to make the devices able to find each other automatically and independently from any node. This purpose gives a basic idea of what possibilities there are to do this.
