# 3rd Report - ESOF

## Index

1. [Introduction](#introduction)
2. [Logical View](#logical-view)
3. [Implementation View](#implementation-view)
4. [Process View](#process-view)
5. [Deployment View](#deployment-view)
6. [Critical Analysis](#critical-analysis)

## Introduction

This report aims to explain some apects relating the software architecture of the Rust project, according to the [4+1 Architecture view model].

![alt tag](https://raw.githubusercontent.com/martapips/rust/master/ESOF-docs/res/4plus1.gif)

[4+1 Architecture view model]:https://en.wikipedia.org/wiki/4%2B1_architectural_view_model

## Logical View

This kind of view concerns the functionality that the language provides to the end-user. The UML diagrams that can be used to represent the logical view are: [Sequece Diagram], [Communication Diagram] and [Class Diagram].

[Sequece Diagram]:https://en.wikipedia.org/wiki/Sequence_diagram
[Communication Diagram]:https://en.wikipedia.org/wiki/Communication_diagram
[Class Diagram]:https://en.wikipedia.org/wiki/Class_diagram

## Implementation View

This view shows the program from a different prespective than the previous one. From the prespective of the programmer. It is used the [Component Diagram] to show the programmer the program's different components.

[Component Diagram]:http://www.tutorialspoint.com/uml/uml_component_diagram.htm

## Process View

This view is foccused on the runtime behaviour of the program. It is in this view that the programs processes are explained as well as the way they use to communicate between them. [Activity Diagrams] are the ones used to describe this view.

![alt tag](https://github.com/martapips/rust/blob/master/ESOF-docs/res/processDiagram.jpg?raw=true)

[Activity Diagrams]:https://en.wikipedia.org/wiki/Activity_diagram

## Deployment View

This view shows the program in the system engineer's prespective.  To represent this view we use [Deployment Diagrams].

![alt tag](https://github.com/martapips/rust/blob/master/ESOF-docs/res/deploymentDiagram.jpg?raw=true)

[Deployment Diagrams]:https://en.wikipedia.org/wiki/Deployment_diagram

## Critical Analysis
