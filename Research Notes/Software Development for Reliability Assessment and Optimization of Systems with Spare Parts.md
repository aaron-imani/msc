# Software Development for Reliability Assessment and Optimization of Systems with Spare Parts
## Paper Link

https://ieeexplore.ieee.org/document/8973241

## Research Questions

How to calculation of reliability indicators in an analytical and experimental way

## Brief Summary

To achieve the required reliability indicators, different strategies are used, such as:

- Backup
- Majorization
- The organization of fault-tolerant control systems
- Use of spare parts and accessories kits (*SPTA*)

The effect of the spare parts kit on the reliability of the system depends on the relationship between the time of replacement of the failed element with the operable spare part and the acceptable time of the interruption in the system operation. Since modern systems can consist of dozens aof components that must be considered when analyzing reliability, and formulas for calculating the reliability of a component with spare parts and consideration of the effect of structure on the overall reliability of the system are rather complicated, then manual analytical calculation is practically not realizable. It leads to the need to use automatic means of calculating reliability indicators for reliability schemes of systems and for further parametric optimization of the system. 

There are a few software products that can calculate, but all of them implement only one of the methods of assessing reliability: analytical or modeling. Because of the errors in the former and the experimental nature of the latter, we should buy multiple softwares and implement a model for each of the systems to be able to compare the results. This paper proporses a a software-algorithmic complex that realizes the calculation of reliability indicators in an analytical and experimental way.

The initial data for assessing the reliability of the system are:

- A structural and reliability scheme
- A list of components with indications of reliability indicators
- reliability targets for the systems under consideration

There are two global types of methods: theoretical and experimental. For the first one the paper has proposed a formula to assess reliability of the system in an analytical way. Moreover, the paper has estimated reiliability by the simulation modeling (the experimental way). They have used TensorFlow library to implement the system.

## Findings

- Creating software models of the estimated systems quickly and in a manual mode
- Optimize the individual SPTA kit in automatic mode
- Create reports with calculation results for use in the project documentation

## Suggested Future Work

- Visualize the calculation model for TensorBoard
- Implement a method for estimating reliability indicators based on modeling
- Create a universal interface for the operation of the computational core and the interface, including the ability to place the computational module and the graphical interface on different computers.

## Relevance to my work

- Learned the different strategies of achieving reliability goals
- Learned the effect of spare parts on reliability of a system
