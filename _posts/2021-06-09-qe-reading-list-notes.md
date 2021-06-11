---
title: 'Notes of QE Reading List Papers'
date: 2021-06-09
permalink: /posts/2021/06/qe-reading-list-notes/
tags:
  - research
  - thinking
---


This page records the summary and my own understanding of each paper in PhD reading list for QE.

<!-- TOC -->
- [1. A Unified Approach to Global Program Optimization](#1-a-unified-approach-to-global-program-optimization)
- [2. The Program Dependence Graph and Its Use in Optimization](#2-the-program-dependence-graph-and-its-use-in-optimization)

### 1. A Unified Approach to Global Program Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/1-A%20Unified%20Approach%20to%20Global%20Program%20Optimization.pdf)

* **Abstract** 
  * <center> technique is presented for global analysis of program structure in order to perform compile time optimization of object code generated for expressions. The global expression optimization presented includes constant propagation, common subexpression elimination, elimination of redundant register load operations, and live expression analysis. A general purpose program flow analysis algorithm is developed which depends upon the existence of an "optimizing function." The algorithm is defined formally using a directed graph model of program flow structure, and is shown to be correct. Several optimizing functions are defined which, when used in conjunction with the flow analysis algorithm, provide the various forms of code optimization. The flow analysis algorithm is sufficiently general that additional functions can easily be defined for other forms of global code optimization. </center>

### 2. The Program Dependence Graph and Its Use in Optimization [[PDF]](https://github.com/haoxintu/haoxintu.github.io/blob/master/files/2-The%20Program%20Dependence%20Graph%20and%20Its%20Use%20in%20Optimization.pdf)

* **Abstract**
  *  <center>  In this paper we present an intermediate program representation, called the program dependence graph (PDG), that makes explicit both the data and control dependences for each operation in a program. Data dependences have been used to represent only the relevant data flow relationships of a program. Control dependences are introduced to analogously represent only the essential control flow relationships of a program. Control dependences are derived from the usual control flow graph. Many traditional optimizations operate more efficiently on the PDG. Since dependences in the PDG connect computationally related parts of the program, a single walk of these dependences is sufficient to perform many optimizations. The PDG allows transformations such as vectorization, that previously required special treatment of control dependence, to be performed in a manner that is uniform for both control and data dependences. Program transformations that require interaction of the two dependence types can also be easily handled with our representation. As an example, an incremental approach to modifying data dependences resulting from branch deletion or loop unrolling is introduced. The PDG supports incremental optimization, permitting transformations to be triggered by one another and applied only to affected dependences. </center>
