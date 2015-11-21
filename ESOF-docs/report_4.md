# 4th Report - ESOF

## Index

1. [Introduction](#introduction)
2. [Testability](#testability)
3. [Test Statistics](#test-statistics)
4. [Critical Analysis](#critical-analysis)



## Introduction

> Software testability is the degree to which a software artifact (i.e. a software system, software module, requirements- or design document) supports testing in a given test context. If the testability of the software artifact is high, then finding faults in the system (if it has any) by means of testing is easier.

>  _Definition from [Wikipedia]_
[Wikipedia]: https://en.wikipedia.org/wiki/Software_testability

In this report we will check **Rust**'s degree of testability by analising some factors like:
- **Controllability**: The degree to which it is possible to control the state of the component under test (CUT) as required for testing.
- **Observability**: The degree to which it is possible to observe (intermediate and final) test results.
- **Isolateability**: The degree to which the component under test (CUT) can be tested in isolation.
- **Separation of concerns**: The degree to which the component under test has a single, well defined responsibility.
- **Understandability**: The degree to which the component under test is documented or self-explaining.
- **Heterogeneity**: The degree to which the use of diverse technologies requires to use diverse test methods and tools in parallel.



## Testability 

By talking with some contributtors to the **Rust Project** and by reading the [Test chapter] on **Rust** blog we learned that Rust turns the test driven approach very easy and that the language lends itself well to testing because first Rust has no inheritance or other convoluted form of dependency which makes the testing of isolated componentes much easier. For example, when we want to give a certain behavior to a set of types, we create a trait and implement it for each type and the trait itself can be tested independently. 

During the tests, the compiler performs the heavy lifting when it comes to common bugs, so you can focus on other things and the language is a good match with unitary tests which leads to easily composable code. It is very simple to maintain coverage and to deploying the service. 

For Rust, the usual practice is having tests right below where something is defined. 

One of the biggest concerns about the testability of Rust is the lack of support for coverage analysis tools. 

Now we will show how to test Rust Code.

Rust contains the **test attribute** and the **ignore attribute**,both of them are used in different situations but all the aprroaches use the same basic tools.

 ## Test
  
At its simplest, a test in Rust is a function that's annotated with the **test** attribute.

![alt tag](https://github.com/martapips/rust/blob/master/ESOF-docs/res/test.png?raw=true)


[Test chapter]:https://doc.rust-lang.org/book/testing.html


## Test Statistics

## Critical Analysis
PODEMOS USAR ISTO NA CRITICAL ANALYSIS MAS AINDA N TÁ BEM ESTRUTURADO.

By the simple expedient of discouraging shared mutable state, Rust leans toward being testable. testability will mostly boil down to your design. You can use global state, you can mix I/O within your routines, ... and if you do things get more complicated to test. One can write a convoluted mess of code in any language, Rust is no exception.


