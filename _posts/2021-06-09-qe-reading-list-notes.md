---
title: 'Notes of QE Reading List Papers'
date: 2021-06-09
permalink: /posts/2021/06/qe-reading-list-notes/
tags:
  - research
  - thinking
location: "Singapore"
---


This page records the summary and my own understanding of each paper in PhD reading list for QE.

<!-- TOC -->
- [1. A Unified Approach to Global Program Optimization (POPL 1973)](#1-a-unified-approach-to-global-program-optimization-pdf)
- [2. The Program Dependence Graph and Its Use in Optimization (TOPLAS 1987)](#2-the-program-dependence-graph-and-its-use-in-optimization-pdf)
- [3. Yesterday, my program worked. Today, it does not. Why? (ESEC/FSE 1999)](#3-yesterday-my-program-worked-today-it-does-not-why-pdf)
- [4. Dynamically discovering likely program invariants to support program evolution (ICSE 1999)](#)

### 1. A Unified Approach to Global Program Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/1-A%20Unified%20Approach%20to%20Global%20Program%20Optimization.pdf)

* **Abstract** 
  * A technique is presented for global analysis of program structure in order to perform compile time optimization of object code generated for expressions. The global expression optimization presented includes constant propagation, common subexpression elimination, elimination of redundant register load operations, and live expression analysis. A general purpose program flow analysis algorithm is developed which depends upon the existence of an "optimizing function." The algorithm is defined formally using a directed graph model of program flow structure, and is shown to be correct. Several optimizing functions are defined which, when used in conjunction with the flow analysis algorithm, provide the various forms of code optimization. The flow analysis algorithm is sufficiently general that additional functions can easily be defined for other forms of global code optimization.

### 2. The Program Dependence Graph and Its Use in Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/2-The%20Program%20Dependence%20Graph%20and%20Its%20Use%20in%20Optimization.pdf)

* **Abstract**
  * In this paper we present an intermediate program representation, called the program dependence graph (PDG), that makes explicit both the data and control dependences for each operation in a program. Data dependences have been used to represent only the relevant data flow relationships of a program. Control dependences are introduced to analogously represent only the essential control flow relationships of a program. Control dependences are derived from the usual control flow graph. Many traditional optimizations operate more efficiently on the PDG. Since dependences in the PDG connect computationally related parts of the program, a single walk of these dependences is sufficient to perform many optimizations. The PDG allows transformations such as vectorization, that previously required special treatment of control dependence, to be performed in a manner that is uniform for both control and data dependences. Program transformations that require interaction of the two dependence types can also be easily handled with our representation. As an example, an incremental approach to modifying data dependences resulting from branch deletion or loop unrolling is introduced. The PDG supports incremental optimization, permitting transformations to be triggered by one another and applied only to affected dependences.

### 3. Yesterday, my program worked. Today, it does not. Why? [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/3-Yesterday%2C%20my%20program%20worked.%20Today%2C%20it%20does%20not.%20Why%3F%20.pdf)

* **Abstract**
  * Imagine some program and a number of changes. If none of these changes is applied (“yesterday”), the program works. If all changes are applied (“today”), the program does not work. Which change is responsible for the failure? We present an efficient algorithm that determines the minimal set of failure-inducing changes. Our delta debugging prototype tracked down a single failure-inducing change from 178,000 changed GDB lines within a few hours.


### 4. Dynamically discovering likely program invariants to support program evolution [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/4-Dynamically%20Discovering%20Likely%20Program%20Invariants%20to%20Support%20Program%20Evolution.pdf)

* **Abstract**
  * Explicitly stated program invariants can help programmers by identifying program properties that must be preserved when modifying code. In practice, however, these invariants are usually implicit. An alternative to expecting programmers to fully annotate code with invariants is to automatically infer invariants from the program itself. This research focuses on dynamic techniques for discovering invariants from execution traces. This paper reports two results. First, it describes techniques for dynamically discovering invariants, along with an instrumenter and an inference engine that embody these techniques. Second, it reports on the application of the engine to two sets of target programs. In programs from Cries's work on program derivation, we rediscovered predefined invariants. In a C program lacking explicit invariants, we discovered invariants that assisted a software evolution task.

