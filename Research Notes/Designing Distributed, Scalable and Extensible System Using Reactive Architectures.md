# Designing Distributed, Scalable and Extensible System Using Reactive Architectures
## Paper Link

https://ieeexplore.ieee.org/document/8745176

## Research Questions

The goal of this paper is to describe a proposed architecture for efficient and extensible data processing in context of distributed systems, with focus on the following elements:

- extensible, scalable and lightweight interoperability model between distributed heterogeneous digital components
- resilient, fault-tolerant and scalable mechanisms for data processing.

## Brief Summary

The primary components used in the proposed solution architecture are the following architectural approaches: **REST Architectural Style** and **Actor Model**; while the main imposed requirements are: **modularity**, **extensibility**, **high scalability** and **loose-coupling**.

Below are some definitions of distributed system in the paper:

- Engineers usually consider a system to be distributed if it implies some level of complexity – separated autonomous components, but with some level of dependency in between.
- Andrew S. Tanenbaum: A collection of independent computers that appears to its users as a single coherent system

Moreover, some advatanges of distributing things have been mentioned that are:

- Horizontal scalability or scaling out and parallelism
- Performance
- Resilience and reliability
- Technology diversity
- Segregation of responsibilities and specialization 
- Evolution-ready
- Business improvement 
- Costs optimization 

When it comes to interaction between two separate systems, the primary choices of the architects are **Application Programming Interfaces** (APIs) or **Messaging Mechanism**.Messaging mechanism is ideal for decoupling in space (distributed) and time (asynchronous) interacting parties.

To meet the today’s demands for software systems, “**The Reactive Manifesto**” was formulated. According to the formulated principles, if we need a scalable, flexible, extensible, resilient and robust concurrent system, we need to take care of the following architectural aspects:

- Responsiveness: quick and consistent results
- Resiliency: react to failures
- Elasticity: react to load
- Message Driven: react to events

On the other hand, **Actor Model** theory, due to its different way of abstraction for implementation of concurrent systems, helps engineers from software sector to enhance many critical aspects in distributed system design and implementation - at the high level it can be called “distributed computing framework”. Also, it is fully compatible with the “*The Reactive Manifesto*”. 

Below are described the components of the proposed reactive architecture. The architecture is divided in four layers:

### Producer Layer (PL)

It is composed of any source of data and/or event e.g. sensors, devices, servers, applications, big systems, etc.

### Queue Layer (QL)

It acts as a kind of buffer between the senders (PL) and the data consumers. To rise the performance of the data flow, the queues are recommended to be kept on a
performant medium such as RAM. It is recommended to use some component for persistence (e.g. database). when producer is not able to communicate directly with the message broker component, there is an Adapter component that can accept messages from producer in some prefined light format e.g. JSON through RESTful HTTP API.

### Coordinator Layer (CL)

The **most important layer for data processing**, with reference to scalability, fault-tolerance, speed of execution is the CL layer, which is based on **Actor Model theory**. After the produced in PL messages are put in the appropriate queue, workers will extract one by one item from the queue according to the configuration for each type of message and call a configured API for the message to be processed. Use of a persistent component is recommended.

### Business Logic Layer (BLL)

The BLL is responsible for effective data processing and ensures the extensibility of the system:

- logic behind each component in each layer can be easily adjusted or replaced
- new components can be added
  
Here, the data can be:

- processed in the system
- sent for processing of just forwarded outside the system 
- used as a trigger (WebHook) for some internal/external process 
- processed with such novel technique as Serverless Computing, usually offered as a service by Cloud providers 

## Findings

A scalable and extensible architecture was proposed using actor model approach and with respect to reactive architecture principles in order to cover the main issues raised by modern distributed software systems.

## Suggested Future Work

None

## Relevance to my work

Helped me to understand the advatanges of distributing things, and the criteria of  a scalable, flexible, extensible, resilient and robust concurrent system that must be satisfied in our proposed framework.
