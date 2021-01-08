# Extracting Interdependent Requirements and resolving conflicted requirements of safety and security for industrial control systems

## Paper Link

https://ieeexplore.ieee.org/document/7366481?section=abstract

## Research Questions

* How to extract interdependent **safety** and **security** requirements and resolve conflicting safety and security requirements?
* What are the possible relationships between safety and security requirements in a software system?

## Brief Summary

In Industrial Control Systems (**ICS**) there are many safety and security requirements that need to be satisfied. Sometimes, satisfying some safety requirements may undermine security requirements, and vice versa. On the other hand in specific scenarios we observe that there are safety requirements and security requirements that help each other to reach their defined goals.

Thus, It's highly recommended to distinguish between the different relationships between safety and security requirements to resolve the possible conflict between them. As proposed in the paper, there are 3 general relationships between a safety and security requirement:

1- unrelated: a relationship when a safety requirement and a security requirement have no effect on each other goals

2- interdependent: a relationship when a safety requirement and a security requirement help each other to reach their goals

3- conflicting: a relationship when a safety requirement and a security requirement undermine each other in reaching their goals

To handle interdependent safety and security requirements, a *goal-based method to analyze and extract security requirements that help enhance safety goals* is proposed in the paper. Generally, it includes involving security threads from outside of the system as a subset of the traditionally obtained safety hazard set. Then, safety and security requirements are extracted from the new hazard set; corresponding security policy is designed and detailed techniques are applied to enhance the safety state.

A severity-based requirement conflicts resolution method for identifying and resolving conflicts in order to integrate safety and security requirements is proposed in the paper. The basic steps are briefly as follows:

1- 

	* Identify assets that need to be protected
	* Conduct hazard and risk analysis

2- 

	* Evaluate threats and risks **by domain experts**
	* Analyze occurrence probability for each hazard and threat and the effects and corresponding severities it may bring
	* Update hazards, threads, accidents and their occurrence probability related to a newly adopted technology
	* Construct a risk matrix (Here risk means risk and hazard) based on the occurrence probability of each thread or hazard and the severity of effects and corresponding severity level given **by experts**

3-  Analyze the results of risk analysis and risk evaluation.

4- Decompose each safety and security requirement into a form explained in the paper.

5- 

* Traverse the decomposed requirement items and locate requirement items that have the same condition and subject but opposite actions.
* Find countermeasures for conflicted safety and security requirements
* Evaluate the cost and feasibility of each requirement item in found countermeasures sets and assign a score between 0 to 1 for each item **by experts**. This score is called *evaluation score*.
* Calculate the *resolution value* of each conflicted requirement item by multiplying *risk value* by *evaluation score* of that requirement. The requirement item in a conflicted pair with a higher resolution value should have a higher priority.

6- Considering the context, resolve the conflict using one of following resolution measures:

	* Implement the requirement item with a higher priority in the conflicted pair
	* Try to avoid these conflicted actions by achieving the goal with another possible solution

## Findings

* Safety and security requirement analysis in industrial control systems to **identify** interdependent requirements and **resolve** conflicting requirements

## Suggested Future Work

* Improving the requirement conflict resolution method
* Decrease the roll of domain expert by **automating** the *evaluation score* calculation process and construction of the risk matrix
* If reliability requirement is considered within the proposed framework, a few new issues may arise. Theses issues can be covered in future research

## Relevance to my work

It can be used in the ARTTA4 project to identify interdependent requirements and resolve conflicting requirements.


