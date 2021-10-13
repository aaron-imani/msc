# Survey on Application Programming Interfaces in Software Defined Networks and Network Function Virtualization
## Paper Link

https://www.sciencedirect.com/science/article/pii/S2666285X21000467

## Research Questions

Over a decade, REST is widely used for architectural style in API design followed by RPC. These styles are used extensively in various domains. This paper presents the survey of such APIs in the world of Software-Defined Networks (SDN) and Network Function Virtualization (NFV).

## Brief Summary

The paper discussed the different categories of APIs and has conducted a schematic analysis of such APIs in the world of Software-Defined Networks (SDN) and Network Function Virtualization (NFV). Concerning SDN, the APIs responsible for interaction between the controller and applications are well known as northbound APIs (NBIs) and the APIs that are interface between controller and data plane are known as southbound APIs (SBIs).

The literature of **NBIs** is grouped based on the following categories: 
- Controller-based: It is is designed to integrate core services with its functionality.
- Intent-based: The usage of NBIs for a specific application requirement are defined in their respective natural language
- Portability: It resolves compatibility issues by providing low level abstraction across different versions of OpenFlow or SBIs. Also, it provides better packet processing on data plane.
- Programmability: Programmability can be used for high-level languages in SDN.
- Virtualization: In virtualization the underlying network devices can reduce capital expenditure and operational expenditure by allowing sharing of resources.

The paper has also gathered the classification and comparison of NBIs in abovementioned properties.

The northbound interfaces that are currently using can be grouped as follows: RESTful APIs, specialized ad-hoc APIs and programming languages. 

Finally, the authors have concluded the below statements:

- REST is more expressive than SOAP
- SOAP is more composable than REST
- SOAP and REST are good in terms of configurable
- It depends on the developer to choose service-oriented architecture or resource-oriented architecture i.e., whether the developer is interested in expressivity of the system or composability of the
system.

## Findings

-  This paper presents the importance of APIs towards orchestration of services
in SDN and NFV platform.

- Helps practitioners and researchers in SDN and NFV field to follow guidelines and standards for designing higher quality services.

- Provides a ready reference for developing effective and efficient orchestration approaches towards micro services in SDN and NFV domains


## Suggested Future Work

The use cases from NBIs to be implemented in SDN based NFV platform for better understanding of the results.
  
## Relevance to my work

Got some general information about the existing APIs and their classification in SDNs.

