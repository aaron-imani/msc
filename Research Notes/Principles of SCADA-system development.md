# Principles of SCADA-system development
## Paper Link

https://ieeexplore-ieee-org.ezproxy.lib.ucalgary.ca/document/8317243

## Research Questions

- What are the principles of control software design?
- What are the principles of SCADA-system development?

## Brief Summar

The paper aims at the principles of control software design. According to the introduction, SCADA systems emerged to answer the need for operator controlling production since robotic devices can’t be self-sustained entirely. Such systems usually are implemented with the devices below:
- Operator panels
- Programmable logic controllers (PLC)
- Frequency converters
- Electrical engines
- Sensors

Control software that is loaded to PLC, is consisted of some program parts which process signals in demanded ways. Firstly, the signal from sensors should be transformed from analog to numeric form. Then, it is compared with a fixed value from the operator panel. If there is a difference, the PI controller compensates deflection of the measuring value from fixed. One of the main tasks is to limit the signal from the operator panel because no one is insured from the human mistake. After compensation, the control signal is sent from the PI controller to the digital-analog converter and then to executing device. 

Control software is created in the main application Simatic Manager. The main principle of the control software is block structure. Firstly, creating the program starts from the Organization block (OB1). This unit communicates between the controller operating system and the user program. After that, the programming language is chosen by the user. There are three programming languages for this purpose:

- LAD (Ladder Diagram)
- STL (Statement list)
- FBD (Function Block Diagram)

Organization block contains function blocks (FB - containing that part of the program that has internal memory and can be repeatedly called in OB1), data blocks (DB - There are two types of such blocks. Global blocks, which can be accessed from all logical blocks in the program. Instances are blocks that communicate with specific function blocks. They store all the static and dynamic FB data to which they are attached) and function (FC - It differs from the functional block in that you cannot use static data in it).

The control software's main elements are the regulating circuits, the program of which is described in the functional blocks. This software solution allows storing static circuit data and continuously asking them in the OB1 block. The regulating circuits consist of a structure of functions. Functions that are realized in function blocks consist of simple elements of comparison, appropriation, bit logic, mathematical operations, etc. 

In conclusion, integration of designed control software, operator interface, devices of automation, and operator itself constitute SCADA system. 

## Findings

- Defining the building block of a control software system.

## Suggested Future Work

None

## Relevance to my work

I got a general overview of SCADA systems and how should a control software for such systems be constructed.