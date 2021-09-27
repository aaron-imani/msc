# Evaluation of Software Architecture Quality Attribute for an Internet Banking System
## Paper Link

https://arxiv.org/ftp/arxiv/papers/1312/1312.2342.pdf

## Research Questions

- Which Software Architecture Analysis method to use for an Internet Banking System?

## Brief Summary

The paper has compared below software architecture analysis methods:

- Software Architecture Analysis Method (SAAM) 
  - This is a five step method for analyzing software architectures
      1. Characterization of functionalities for a given domain.
      2. Mapping of this functionalities over the structural decomposition of architecture.
      3. Select the quality attributes for assessing the architecture
      4. To test the selected quality attribute, identify the concrete tasks.
      5. Overall Evaluation of Architecture for these tasks
  - Its main objective is Architectural suitability and risk analysis. 
  - It is associated with an architectural description language.
  - It is a practical and proven method and applied for examining architectures of user interface portion of interactive system.
- Scenario-based Software Architecture Analysis method (SAAM)
  - It is a structured scenario-based architectural analysis.
  - It includes five activities:
      1. Describe The Candidate Architecture
      2. Develop Scenarios
      3. Evaluate Each Scenario
      4. Reveal Scenario Interaction
      5. Weight Scenarios and Scenario Interactions
- Software Architecture Analysis Method for Evolution and Reusability (SAAMER)
  - It is a framework and a set of architectural views designed to evaluate software architecture for evolution and reuse.
  - It is based on SAAM which is a scenario based approach for software evaluation
  - This framework consists of four phases described below:
    1. Gathering
    2. Modeling
    3. Analyzing
    4. Evaluating
  - Every scenario is assigned a weight of affected components in the scenario divided by the total number of components in the current architecture (The closer the scenario weight is to one, the more reusable it is)

## Findings

-  SAAM provides better support for evaluation.
-  4+1 view model is best for analysis of portion of the architecture.
-  SAAM can also be implemented in small projects and can be tailored

## Suggested Future Work

- Review and evaluate the software quality which is not covered in this review
  
## Relevance to my work

Compared three different software architecture analysis methods helping me in devising our approach to evaluate Tango Controls