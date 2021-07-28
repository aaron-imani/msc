# UNIFYING ALL TANGO CONTROL SERVICES IN A CUSTOMIZABLE GRAPHICAL USER INTERFACE
## Paper Link

https://s3.cern.ch/inspire-prod-files-3/36227c2997b5796d1114d5f84325018b

## Research Questions

- How to unify all Tango Control services in a customizable graphical user interface?
- How to implementat a Taurus-based application as consistent as CSS but with a higher versatility?

## Brief Summary

Tango fits perfectly within SCADA definition, providing the communication channels and software tools
needed to manage large particle accelerators and other facilities, along with additional control services such as Archiving, Alarms and User Access. These services are managed by a collection of applications developed either by the core team or by other members of the community. Those applications provide a rich functionality and a full-featured control system, but also a diverse collection of look and feels and workflows that may be inconsistent and interfere with user interaction.

GUI consistency issues are not unique to Tango or to open-source control systems, as they may apply to any collaborative project on which each member needs to tune the generic tools to its own context. At ALBA, these problems were mostly solved once Taurus became the default GUI framework for all our applications, thus creating the opportunity to unify the user interaction with the whole control system. Although Taurus provides a consistent UI framework for all applications developed at ALBA, it still leaves uncovered those control services that are either completely Tango specific, not developed by ALBA or do not fit well in the current model URI's of Taurus. The same problem has been approached before by the EPICS community, developing a common UI framework to manage all the aspects of the control system. Hence, the implementation of a Taurus-based application as consistent as CSS but with a higher versatility.

## Findings

- Unified all Tango Control services in a customizable graphical user interface

## Suggested Future Work

Future integration of additional control systems and features in VACCA will be based in Taurus Schemas and Plugins mechanisms still under development, trying to keep backwards compatibility with existing Perspectives as much as possible.

## Relevance to my work

I want to use this paper in the literature review of my summer paper.
