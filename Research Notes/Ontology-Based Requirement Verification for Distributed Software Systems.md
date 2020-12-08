# Ontology-Based Requirement Verification for Distributed Software Systems

## Paper Link

https://drive.google.com/file/d/12LmrL_yjp8MHaNPrPjDkCDChSTlGvlGy/view?usp=sharing

## Research Questions

- How to devise systematic and automated methodologies to analyze software requirements?
- How can we reduce the input needed by a systematic and automated methodologies to analyze software requirements of current approaches?

## Brief Summary

The paper intend to devise a systematic and automated methodologies to analyze software requirements that requires less input from user comparing with current workarounds. 

For this purpose, It has explained what Ontology is, it's usage in software engineering and the two views of it: Dynamic and Static Ontologies. These two types of ontologies are used in the paper to fill semantic causality table for for each state of the generated dynamic ontology from software system.

Having used a fleet management system as a case study, the paper has defined the below concepts:

* partial Message Sequence Chart (pMSC)
* projection
* Equivalent Finite State Machine (eFSM) for a projection
* Semantic causality
* Domain theory
* State value
* Identical states

The semi-automatic algorithm presented by the paper can be summarized in following steps:

1- Static Ontology Generation

2- Dynamic Ontology Generation

3- Build the domain theory of the problem by constructing and filling tables for each state in eFSMs of the problem

4- Calculating state values using the generated tables in previous step

5- Finding identical states and merging to detect emergent behavior

The proposed methodology in this research has been developed into an easy to use software tool (EBD) to automate the process of requirement analysis. The greatest
contributions of this methodology include *Consistency and increased level of automation*.

## Findings

- Removing the need of domain experts to find semantic causalities
- Reducing user input to automate the requirement verification process
- Partially Automating the specification and design review of the distributed system and detect a subset of unwanted run time behaviors, including implied behaviors.

## Suggested Future Work

* Incorporating the sequence diagram notation in requirement validation methodologies
* Extending the application to work with different UML development platforms such as IBM Rational Rose
* Implementing the proposed algorithm as a syntax checker to provide an automated tool
  to check and correct system designs
* Being extended to verify the design of multi-agent systems
* Devising algorithms to analyze design artifacts of other Agent Oriented Software Engineering (AOSE) methodologies such as GAIA.
