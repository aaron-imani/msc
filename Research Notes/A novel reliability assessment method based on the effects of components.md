# A novel reliability assessment method based on the effects of components
## Paper Link

https://ieeexplore.ieee.org/document/8854711

## Research Questions

- How to describe the component-based software based on the graph theory?
- What are the factors that influence the reliability of components?
- How to define the component importance?
- How to measure the system reliability with the consideration of component importance?
## Brief Summary

The paper has proposed a novel reliability evaluation method focusing on analyzing the impacts of different components based on the below three parameters:

- **Self-influence**: The self-influence of component Ci can be described by the frequency of visits to Ci during the single complete operation of the software system
- **Failure influence**: If a component Ci depends on many other components at the same time, that is, information can flow from many other components to Ci. And it means that failures of Ci will have a greater impact on the software reliability.
- **Fault propagation influence**: If many other components depend on the component Ci at the same time, that is, information can flow from component
Ci to many other components. And it means that failures of Ci
have more paths and wider range to propagate, which will
have a large impact on the system reliability.

Each of the above parameters can be defined if we model the component-based software using a directed graph. All of the aforementioned parameters will be calculated for each component to calculate the component importance. Afterwards, the computed components' importance will be used to calculate the overall reliability of the componenet-based software system.

## Findings

A novel reliability assessment method based on the effects of components by involving other component importance factors i.e. Failure influence and Fault propagation influence that improves the precision of reliability assessment.

## Suggested Future Work

- Verifying the feasibility of the proposed approach by using a real system and updating the results with the consideration of the change in reliability
- Determining the exact quantitative condition of weight coefficient
  
## Relevance to my work

This paper can be helpful for dynamic backup section of our summer paper. Using the proposed method, we know from which component we should create a backup.
