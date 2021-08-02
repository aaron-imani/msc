# A Comparative Analysis of the Architecture of Control Systems of Physical Research Facilities
## Paper Link

https://link.springer.com/article/10.1134/S1547477120040123

## Research Questions

- A comparative analysis of these EPICS, TANGO, and CX

## Brief Summary

Although any “mature” CS can be potentially used for the automation of any facility, there are significant architectural differences between the systems which influence both the rationality of application for certain facilities and the convenience of interoperation with other CS’s. 

All modern CS’s are constructed according to a distributed three-tier model, which aims to separate the business logic of control programs (upper tier) from the direct operation with the equipment (lower tier). The middle tier is connecting; it provides data exchange between the control programs and the equipment and solves many routine tasks.

## Findings

- CX allows the direct data exchange from an arbitrary CS.
- EPICS assumes operating only with the EPICS, but allows creating “gateway servers” into other CS's.
- TANGO does not allow direct access to other CS’s

## Suggested Future Work

- Analyze at least the FESA framework
- A comparative analysis would be incomplete without comparing efficiency:
  - By the rate of transmitting large volumes of data
  - By the rate of transmitting large volumes of scalar-data.
  - By the response time.

## Relevance to my work

I want to use this paper in the literature review of my summer paper.
