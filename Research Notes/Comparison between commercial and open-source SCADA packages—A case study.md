# Comparison between commercial and open-source SCADA packages—A case study
## Paper Link

https://www.sciencedirect.com/science/article/abs/pii/S092037961000030X

## Research Questions

- What are the potential tests to evaluate SCADA packages?
- Which of the FTV-SE, PVSS, EPICS, and Tango Controls is a more suitable SCADA package?

## Brief Summary

They have evaluated two commercial (FTV-SE and PVSS) and two open-source (EPICS and TANGO) SCADA packages to select one of them for *SPIDER* (Source for the Production of Ions of Deuterium Extracted from Rf plasma) at *PRIMA* (Padova Research on Injectors Megavolt Accelerated). They tested the SCADA packages in terms of application set-up and performance in four diferrent scenarios.

## Findings

### FTV-SE

\+ A very good product in terms of easiness of development, features and graphical quality

\- It needs an intermediate layer (Kepware technology) to communicate with third-party devices

\- Currently limited to the MS Windows operating system

### TANGO

\+ Richness of tools and the possibility of customizing a system writing code with effective and multi-platform object oriented programming languages like Java, C++ and Python

\- Comprehension of its structure requires more efforts than the other SCADAs

\- A strong programming skill is needed

\- A special effort is necessary to implement the data exchange in an efficient way

### PVSS

\+ PVSS proved better in terms of communication set-up

\+ Availability of a user interface from where to choose, for instance, the driver and polling group to be associated with each variable

\+ Better documentation and is strongly supported by CERN

### EPICS

\+ The EPICS network performance was better than the PVSS one

\+ It is the CODAC group choice, it is open-source and open-licensed and it does not depend on market policies.

\-  The communication in EPICS had to be configured through script files



## Suggested Future Work

None

## Relevance to my work

I want to use this paper in the literature review of my summer paper.
