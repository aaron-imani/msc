# SQAF-DS: A Software Quality Assessment Framework for Dependable Systems
## Paper Link

https://ieeexplore.ieee.org/document/6649907

## Research Questions

How to to reduce the time and cost for dependability assessment

## Brief Summary

The paper has proposed a way to reduce the effort for dependability assessment; Software Quality Assessment Framework for Dependable Systems (**SQAFDS**). SQAF-DS intends to reduce the time and cost thorough using test cases as a means of the assessment. Since test cases are developed as one of the software engineering tasks during software development, it can be reused for dependability assessment means. 

To elaborate on the proposed method, the dependability requirements that are derived from the results of dependability analysis should be converted into depandability properties in a way that depends on the formal checking methods are going to be used. On the other hand, test cases should be converted in a same way to a proper input for the formal checking tool. The formal checking can be Model checking, equivalence checking, and set inclusion. If the formal checking tool returns *TRUE* it means that the dependability property has been included in a test case (or is an equivalent of it). In this case, if the test has been passed then the dependability property has been implemented well. Otherwise, if the formal checking tool returns *FALSE*, we don't know whether the dependability property has been implemented well or not and we need to do other dependability assessment techniques to figure it out.

## Findings

Reduce the cost of software quality assessment thorough using test cases as a means of the assessment

## Suggested Future Work

A full-scale safety assessment on system-level dependability requirements and test cases of a control software of nuclear reactor protection system in Korea

## Relevance to my work

I studied this paper to get some ideas about software quality assessment as the evaluation part of the summer paper
