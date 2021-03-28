# eTDP: Enhanced Topology Discovery Protocol for Software-Defined Networks
## Paper Link

https://ieeexplore.ieee.org/document/9218155

## Research Questions

- How to decrease network traffic and latency between between the control plane and the forwarding plane in SDNs that happens due to topology discovery?
- How to remove previous configurations needed in SDN switches in order to discover topology?
- How to distribute topology discovery task between forwarding devices?

## Brief Summar

The paper aims to enhance the existing toplogy discovery protocols by removing the need of previous configurations in SDN switches, plug-and-play controller/switch provisioning, delegating neighbour discovery to the forwarding devices. Generally, the proposed protocol uses a divide and conquer approach to divide the topology discovery task among network devices. This is doable by creating a control tree. 

The proposed mechanism is scalable in terms of the required number of packets with respect to the number of SDN controllers. The obtained results also show that the overall number of packets generated per switch is not affected by increasing the number of SDN controllers. Moreover, it has been demonstrated that eTDP provides a suitable approach for discovering the network topology with discovery times of under 0.08 ms in the three considered networks.

## Findings

- Automatic discovery of the network without requiring previous IP configurations or controller knowledge of the network
- Distribute topology discovery tasks among network devices
- Reducing overload in controller performance to reinforce the current topology discovery service in SDN

## Suggested Future Work

None

## Relevance to my work

The general idea of distributing topology discovery between network devices can be useful for removing the central node on tango controls and make the devices auto-discoverable by the other devices in the network.
