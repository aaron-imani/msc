# Evolution and Convergence of Alarm Systems in Tango
## Paper Link

https://s3.cern.ch/inspire-prod-files-0/01489ca1dacf98488022664493bff8c2

## Research Questions

- What is the status of the collaboration between Alba and Elettra Synchrotron sources for the convergence of its both alarms systems under the IEC62682 standard?
- What is the usage of HDB++ tools for logging and diagnostic of alarms?

## Brief Summary

Alarm Systems have been a common part of control system toolkits for decades. In the Synchrotron community some of the most common tools are **PANIC** and
**AlarmHandler** for Tango Control System, as well as **BEAST** Alarm System for EPICS. PANIC and AlarmHandler systems have coexisted within the Tango community for years, but at some point new members of the community asked whether to choose one or the other for their specific domain.

PANIC was developed by ALBA Synchrotron in 2007 as a Python alternative to the Tango Alarm System (AlarmHandler) which has differents as below:

- PANIC applies a distributed architecture
- It adds annunciator features and more flexibility in alarms declaration, allowing to execute python code for both the formula and the resulting action
- Enables the usage of wildcards for attribute selection
- Enables reusing the data from the alarm evaluation to generate rich-text emails or SMS messaging

The paper focus in the changes that allowed their convergence of Tango Control alarm systems into a single toolkit. Below summerizes the required changes:

- Alarm database has been dropped. Instead, Tango Database is used to store the alarm formulas and configuration
- It has been discarded the idea to maintain a separate Alarm logging, thus reusing the new HDB++ archiving for Tango

The PANIC API is currently connecting to two types of device servers, **PyAlarm**, developed in Python by ALBA Synchrotron, and **AlarmHandler**, developed in C++ by Elettra Sincrotrone. The AlarmHandler can be dedicated to **fast reaction** on critical conditions while PyAlarm **flexibility** provides its best usability on interacting with multiple devices or evaluating attribute evolution in time.

PANIC allows scaling by exporting each evaluated alarm as a new attribute. Alarm summaries can be done at client level (Alarm View) or at device server level (Alarm Group). When created at alarm level, it will behave as any other alarm, triggering actions and exporting a new attribute, so the system can be scaled to the next level. They can be accessed even from other Tango Control Systems, so the hierarchy can be expanded indefinitely.

## Findings

-  The status of the collaboration between Alba and Elettra Synchrotron sources for the convergence of its both alarms systems under the IEC62682 standard
-  The usage of HDB++ tools for logging and diagnostic of alarms
-  The required changes to converge Tango Control alarm systems into a single toolkit

## Suggested Future Work

None
  
## Relevance to my work

Made me acquainted with the Tango Controls famous alarm system, PANIC, and relevant concepts of alarming in a control system.

