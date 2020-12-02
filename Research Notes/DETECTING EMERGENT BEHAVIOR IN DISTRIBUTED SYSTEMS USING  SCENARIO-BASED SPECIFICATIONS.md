# DETECTING EMERGENT BEHAVIOR IN DISTRIBUTED SYSTEMS USING SCENARIO-BASED SPECIFICATIONS

## Paper Link

https://drive.google.com/file/d/165k6cGIa7biq6AqHw0x8QHV5SzYOZ747/view

## Research Questions

- What is the definition of *indeterminism* in behavior of distributed systems?
- How to detect and remove *implied scenarios* during field use of distributed systems?

## Brief Summary

Having used a mine sweeping robot as a case study, the paper has defined the below concepts:

* partial Message Sequence Chart (pMSC)
* projection
* Equivalent Finite State Machine (eFSM) for a projection
* Semantic causality
* Domain theory
* State value
* Identical states

By creating projections for every process of message chart sequences of possible scenarios of the case study, eFSMs can be defined for each of them. The paper has stated that *indeterminism* happens when identical states emerge in generated eSFMs. 

One of the challenging contributions of this paper is to define state value independent from domain experts' preferences. this makes the used methodology work as an automated algorithms since the state values are calculated base on Semantic Causality concept which itself does not depend on domain expert judgements.

eFSMs from MSCs with state values will lead the identical states which are defined by the paper to be detected and merged. This way the emergent behavior can be detected during field use of a system which mitigates expenses by 20 times comparing with detecting and removing them in design phase.

## Findings

- Definition of *indeterminism* in behavior of distributed systems
- Detection of failures and removal of faults during field use of distributed systems
- Automating the specification and design review of the distributed system and detect a subset of unwanted run time behaviors, including implied behaviors.

## Suggested Future Work

* Automating the process of resolving the detected emergent behavior is intended
* Being extended to a comprehensive framework for model based analysis and testing of distributed software systems
* Being modified to take the UML’s sequence diagrams as input and thus incorporate the analysis and design of distributed object oriented systems
* Being extended to verify the design of multi-agent systems
* Being extended to verify system requirements against containing particular illegal scenarios

## Relevance
TBW




