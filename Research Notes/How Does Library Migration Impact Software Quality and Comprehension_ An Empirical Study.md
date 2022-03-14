# How Does Library Migration Impact Software Quality and Comprehension? An Empirical Study
## Paper Link

https://link.springer.com/chapter/10.1007/978-3-030-64694-3_15

## Research Questions

- What is the impact of library migration on the quality of software design?
- Does migration improve the code readability?
- Can we leverage design and readability metrics to recommend better code examples of migration?

## Brief Summary

The authors studied the effects of library migration on software quality and readability using a dataset of library migrations. In addition, they have developed a tool to recommend migration code examples for different migration scenarios using the Java language. Their tool has been put to the test by conducting a survey among 10 experienced developers to verify its accuracy. According to the results, 59% of the developers opted for the first recommended code example for a particular migration. Moreover, their findings indicate that, in terms of software quality, library migration may increase software design quality metrics by decreasing coupling and cyclomatic complexity and increasing cohesion. It has also been reported that code readability can be improved through library migration.

## Findings

- Effects of library migration on software design quality and code readability
- A recommendation tool for suggesting migration codes to Java developers

## Suggested Future Work

- Including the execution of selected test cases, to avoid the introduction of regression
- Extending the structural metrics used to characterize software design quality, such as including the weighted method per class, response for a class, class stability, and depth of inheritance tree.
- Recommendation further leveraging API contextual information to recommend better APIs for usage, with respect to a given code fragment.

## Relevance to my work

Can be used to state the potential benefits of migration from Tango Controls to other libraries like gRPC or Ice.