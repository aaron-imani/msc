# From Requirements to Software Design - An Automated Solution for Packaging Software Components

## Paper Link

https://drive.google.com/file/d/1uc8TKeX8mPIuQ6dVOkhS-Q2ckbI8t5jm/view?usp=sharing

## Research Questions

* How to establish systematic and automated solutions to increase the quality of the design of the system while improving the efficiency of the design process?
* What clustering algorithm would be appropriate to be used in the proposed packaging solutions by the paper?
* How to define similarity measure for each process in the software under development (**SUD**)?

## Brief Summary

Despite existence of criteria for a good design in software engineering, the best design choices are not always obvious; particularly for more complex systems. Consequently, the quality of the system can be compromised due to over-looking details in the requirements such as the volume of message-passing between different components. 

Accordingly, adopting an automated workaround for different phases of software design would increase the quality of the design of the system while improving the efficiency of the design process. The paper aims at devising a systematic automated approach for packaging software components.

The proposed approach consists of three main phases:

1- Static Ontology Generation

2- Dynamic Ontology Generation

3- Package Diagram Recommendation

The first two phases have been discussed elaborately in [Ontology-Based Requirement Verification for Distributed Software Systems](https://github.com/alirezaimn/msc/blob/main/Research%20Notes/Ontology-Based%20Requirement%20Verification%20for%20Distributed%20Software%20Systems.md). In the third phase, the static ontology generated for the SUD is used to generate the first level of packaging. Following, for each group in the first level of packaging, a hierarchal clustering method called **Agglomerative clustering** is adopted to provide the SUD designer with multiple packaging options of different count of groups ( component clusters). 

The similarity measure is what leads the generated packaging solution to have high cohesion in each package and low coupling with packages. To reach this goal, a feature vector should be calculated for every process *i* in the package *P* of the first level packaging for the SUD such that the nth element of the vector indicated the communication size between the process *i* and process *n* of *P*.  Thus, the similarity measure for the process *i* and *j* in the package *P* of the first level packaging for the SUD is defined as (Communication size between *i* and *j* - Sum of absolute difference of communication sizes of *i* and *j* with process *h* which is not equal to *j* nor *j*).

The proposed method is used in a case study to demonstrate its applicability. 

## Findings

* a unique solution towards **automating** the software design process as part of a comprehensive framework for the analysis of software requirements and design
* providing software engineer with a comprehensive and optimal package diagram based on the system requirements in the early stages.

## Suggested Future Work

* Do empirical studies to investigate the effectiveness and the amount of time saving achieved by the proposed solution over manual designing of package diagrams.
* Being extended to help on more design decisions such as recommending design patterns based on the optimal architecture.
