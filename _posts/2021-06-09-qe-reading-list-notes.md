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
- [4. Dynamically discovering likely program invariants to support program evolution (ICSE 1999)](#4-dynamically-discovering-likely-program-invariants-to-support-program-evolution-pdf)
- [5. Bandera: extracting finite-state models from Java source code (ICSE 2000)](#5-bandera-extracting-finite-state-models-from-java-source-code-pdf)
- [6. CUTE: a concolic unit testing engine for C (ESEC/FSE 2005)](#6-cute-a-concolic-unit-testing-engine-for-c-pdf)
- [7. code2vec: Learning Distributed Representations of Code (POPL 2019)(#)]

### 1. A Unified Approach to Global Program Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/1-A%20Unified%20Approach%20to%20Global%20Program%20Optimization.pdf)

* **Abstract:** A technique is presented for global analysis of program structure in order to perform compile time optimization of object code generated for expressions. The global expression optimization presented includes constant propagation, common subexpression elimination, elimination of redundant register load operations, and live expression analysis. A general purpose program flow analysis algorithm is developed which depends upon the existence of an "optimizing function." The algorithm is defined formally using a directed graph model of program flow structure, and is shown to be correct. Several optimizing functions are defined which, when used in conjunction with the flow analysis algorithm, provide the various forms of code optimization. The flow analysis algorithm is sufficiently general that additional functions can easily be defined for other forms of global code optimization.

* Detailed Summary

### 2. The Program Dependence Graph and Its Use in Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/2-The%20Program%20Dependence%20Graph%20and%20Its%20Use%20in%20Optimization.pdf)

* **Abstract:** In this paper we present an intermediate program representation, called the program dependence graph (PDG), that makes explicit both the data and control dependences for each operation in a program. Data dependences have been used to represent only the relevant data flow relationships of a program. Control dependences are introduced to analogously represent only the essential control flow relationships of a program. Control dependences are derived from the usual control flow graph. Many traditional optimizations operate more efficiently on the PDG. Since dependences in the PDG connect computationally related parts of the program, a single walk of these dependences is sufficient to perform many optimizations. The PDG allows transformations such as vectorization, that previously required special treatment of control dependence, to be performed in a manner that is uniform for both control and data dependences. Program transformations that require interaction of the two dependence types can also be easily handled with our representation. As an example, an incremental approach to modifying data dependences resulting from branch deletion or loop unrolling is introduced. The PDG supports incremental optimization, permitting transformations to be triggered by one another and applied only to affected dependences.

### 3. Yesterday, my program worked. Today, it does not. Why? [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/3-Yesterday%2C%20my%20program%20worked.%20Today%2C%20it%20does%20not.%20Why%3F%20.pdf)

* **Abstract:** Imagine some program and a number of changes. If none of these changes is applied (“yesterday”), the program works. If all changes are applied (“today”), the program does not work. Which change is responsible for the failure? We present an efficient algorithm that determines the minimal set of failure-inducing changes. Our delta debugging prototype tracked down a single failure-inducing change from 178,000 changed GDB lines within a few hours.


### 4. Dynamically discovering likely program invariants to support program evolution [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/4-Dynamically%20Discovering%20Likely%20Program%20Invariants%20to%20Support%20Program%20Evolution.pdf)

* **Abstract:** Explicitly stated program invariants can help programmers by identifying program properties that must be preserved when modifying code. In practice, however, these invariants are usually implicit. An alternative to expecting programmers to fully annotate code with invariants is to automatically infer invariants from the program itself. This research focuses on dynamic techniques for discovering invariants from execution traces. This paper reports two results. First, it describes techniques for dynamically discovering invariants, along with an instrumenter and an inference engine that embody these techniques. Second, it reports on the application of the engine to two sets of target programs. In programs from Cries's work on program derivation, we rediscovered predefined invariants. In a C program lacking explicit invariants, we discovered invariants that assisted a software evolution task.

### 5. Bandera: extracting finite-state models from Java source code [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/5-Bandera-%20extracting%20finite-state%20models%20from%20Java%20source%20code.pdf)

* **Abstract:** Finite-state verification techniques, such as model checking, have shown promise as a cost-effective means for finding defects in hardware designs. To date, the application of these techniques to software has been hindered by several obstacles. Chief among these is the problem of constructing a finite-state model that approximates the executable behavior of the software system of interest. Current best-practice involves hand construction of models which is expensive (prohibitive for all but the smallest systems), prone to errors (which can result in misleading verification results), and difficult to optimize (which is necessary to combat the exponential complexity of verification algorithms). The authors describe an integrated collection of program analysis and transformation components, called Bandera, that enables the automatic extraction of safe, compact finite-state models from program source code. Bandera takes as input Java source code and generates a program model in the input language of one of several existing verification tools; Bandera also maps verifier outputs back to the original source code. We discuss the major components of Bandera and give an overview of how it can be used to model check correctness properties of Java programs.

### 6. CUTE: a concolic unit testing engine for C [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/6-CUTE-%20a%20concolic%20unit%20testing%20engine%20for%20C.pdf)

* **Abstract:** In unit testing, a program is decomposed into units which are collections of functions. A part of unit can be tested by generating inputs for a single entry function. The entry function may contain pointer arguments, in which case the inputs to the unit are memory graphs. The paper addresses the problem of automating unit testing with memory graphs as inputs. The approach used builds on previous work combining symbolic and concrete execution, and more specifically, using such a combination to generate test inputs to explore all feasible execution paths. The current work develops a method to represent and track constraints that capture the behavior of a symbolic execution of a unit with memory graphs as inputs. Moreover, an efficient constraint solver is proposed to facilitate incremental generation of such test inputs. Finally, CUTE, a tool implementing the method is described together with the results of applying CUTE to real-world examples of C code.

### 7. code2vec: Learning Distributed Representations of Code [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/7-code2vec%20Learning%20Distributed%20Representations%20of%20Code.pdf)

* **Abstract:** We present a neural model for representing snippets of code as continuous distributed vectors ("code embeddings"). The main idea is to represent a code snippet as a single fixed-length code vector, which can be used to predict semantic properties of the snippet. To this end, code is first decomposed to a collection of paths in its abstract syntax tree. Then, the network learns the atomic representation of each path while simultaneously learning how to aggregate a set of them.
We demonstrate the effectiveness of our approach by using it to predict a method's name from the vector representation of its body. We evaluate our approach by training a model on a dataset of 12M methods. We show that code vectors trained on this dataset can predict method names from files that were unobserved during training. Furthermore, we show that our model learns useful method name vectors that capture semantic similarities, combinations, and analogies.
A comparison of our approach to previous techniques over the same dataset shows an improvement of more than 75%, making it the first to successfully predict method names based on a large, cross-project corpus. Our trained model, visualizations and vector similarities are available as an interactive online demo at http://code2vec.org. The code, data and trained models are available at https://github.com/tech-srl/code2vec.

### 8. Empirical Evaluation of the Tarantula Automatic Fault-Localization Technique [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/8-Empirical%20evaluation%20of%20the%20tarantula%20automatic%20fault-localization%20technique.pdf)

* **Abstract:** The high cost of locating faults in programs has motivated the development of techniques that assist in fault localization by automating part of the process of searching for faults. Empirical studies that compare these techniques have reported the relative effectiveness of four existing techniques on a set of subjects. These studies compare the rankings that the techniques compute for statements in the subject programs and the effectiveness of these rankings in locating the faults. However, it is unknown how these four techniques compare with Tarantula, another existing fault-localization technique, although this technique also provides a way to rank statements in terms of their suspiciousness. Thus, we performed a study to compare the Tarantula technique with the four techniques previously compared. This paper presents our study---it overviews the Tarantula technique along with the four other techniques studied, describes our experiment, and reports and discusses the results. Our studies show that, on the same set of subjects, the Tarantula technique consistently outperforms the other four techniques in terms of effectiveness in fault localization, and is comparable in efficiency to the least expensive of the other four techniques.
