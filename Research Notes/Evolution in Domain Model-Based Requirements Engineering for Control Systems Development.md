# Evolution in Domain Model-Based Requirements Engineering for Control Systems Development

## Paper Link

https://ieeexplore.ieee.org/document/5328510

## Research Questions

- What are the different modification paths of the domain model of Control Systems?
- What are the consequences of the changes applied to the domain model of Control Systems towards requirements modelling and the identification of projects with similar requirements?

## Brief Summary

The paper has invsetigated the effects of model evolution on the domain model-based requirements engineering approach and developed a classification of possible domain model modifications. For each such class, its impact on the similarity search is analyzed and appropriate countermeasures to limit these harmful impacts is derived.

The requirements engineering can be accelerated using a *domain model*. That approach enabled (1) a fast design of the requirements model, and (2) an identification of concluded projects with similar requirements in order to re-use developed artifacts. However, due to the innovativeness, flexibility, and customer orientation of control systems development, the domain model is subject to continuous change and it can not be assumed to be *static*.

In order to enable a valuable support even with an evolving domain model, we have to identify counter measures to limit the impacts of the consequences.

### Model-Driven Similarity Search

Two projects are called *similar*, if there exist indications that parts of the control system software of one project could be reused for the other. An indication is given, if parts of the requirements models
of the projects match. An indication is given, if parts of the requirements models of the projects match.

For this comparison task. the deductive object manager ConceptBase is employed that implements the knowledge representation language *Telos*. Using an elaborated method in the paper, an *overall ranking* is computed for each project. The projects containing similarities within the highly weighted areas of the new project’s requirements model are ranked higher.

### Domain Model Evolution

As a result of modifications to control systems, some problems would be arised in model comparison. The modified domain model may not match with already existing requirements models using a specific role.

Imagine that an element in a former control system project already contained a specific *element* *i*. But at that time it has not been part of the domain model. We then face the problem that model comparison will not match the *element i* of the modified domain model with the conceptually same element of the old requirements model. The old requirements model will get a lower ranking than it should get.

### Classification of Modifications

To support the continuous evolution of the domain model we systematically analyse the different types of modifications. The proposed investigation reveals quite clearly the problems caused by a modification: the comparison queries need to be updated manually in some cases, even with updated queries the ranking is not always accurate, and the existing requirements models can not be updated automatically in all cases.

### Counter Measures

The main goal of any counter measure is to reestablish an accurate ranking of similar requirements models. Furthermore, the need for manual updates, for example, of the comparison queries or of existing requirements models should be kept to a minimum. Two kinds of measures to help achieving these goals are suggested by the paper:

1. **Robust queries**

   * Using **identifiers** instead of names within the queries will solve the problem of name changes.

   * The definition and application of **generic queries** instead of a set of hard coded queries 	eliminates the need to define separate queries for.

2. **Support for Updating Existing RE Models**

   To support the update of existing requirements models, we require that any model modifications, at the domain model as well as at each concrete requirements model, are performed using proposed tool environment. Using the start and the end time of each modification session, we can deduce the changes using the *diff* operator (Given two points in time t1 and t2, the *diff* operator computes all objects added (resp. deleted) within a model from its version at time t1 to
   its version at time t2.). 

   In a first step all the objects of the previous domain model version that are connected to the added objects via some link relationship are identified and they are called *anchor objects*. Then,  the *diff* operator is applied to each existing requirements model to compute its project-specific extensions. After that,  the *anchor objects* of the domain model modification with the *anchor objects* of the project-specific extensions are compared. 

   For project-specific extensions with at least one matching anchor object, the corresponding project is added to the list of projects that are possibly affected by the domain model modification. 

   In the last step, the tool environment presents a graphical view of all these projects to the user. To enhance readability, the view is adjusted to highlight the *anchor objects* and the extension, so that the user can faster decide whether the project is really affected.

## Findings

- Classification of possible modifications to control systems
- Countermeasures for problems caused by modifying control systems in domain model-based  requirements engineering

## Suggested Future Work

* Broaden the domain model to capture more than just combustion engines
* Support control systems development for modern hybrid engines
* The successful application of a new technology or solution within some projects makes it
  a good candidate for inclusion in the domain model. The same holds for well-proven solutions to design problems. A tool that supports the identification of such candidates in former projects and the specification of them as domain model extensions can be developed in the future.

## Relevance to my work

The discussed control system in the paper is Engine Control Systems. Almost same problems can arised in the ARTTA4 project in case of future modification to the software control system and the paper has devised possible solutions for the arised problems in case the requirements engineering adopted for the project is domain model-based.
