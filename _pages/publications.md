---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
### Conference Paper
* [ICSE 2024] **Haoxin Tu**, Lingxiao Jiang, Debin Gao, and He Jiang, "Beyond a Joke: Dead Code Elimination Can Delete Live Code", in *Proceedings of 46th IEEE ACM International Conference on Software Engineering (ICSE-NIER 2024)*. [To appear]
 * [CCS 2023] Pansilu Pitigalaarachchi, Xuhua Ding, Haiqing Qiu, **Haoxin Tu**, Jiaqi Hong, and Lingxiao Jiang, "KRover: A Symbolic Execution Engine for Dynamic Kernel Analysis", in *Proceedings of the 2023 ACM SIGSAC Conference on Computer and Communications Security (CCS 2023)*. [[PDF]](https://haoxintu.github.io/files/ccs2023-KRover_camera_ready.pdf) [[Source Code]](https://github.com/KRoverSystems/KRover)
 * [ICSE 2023] **Haoxin Tu**, "Boosting Symbolic Execution for Heap-based Vulnerability Detection and Exploit Generation", in *the Doctoral Symposium Track of IEEE/ACM International Conference on Software Engineering (ICSE 2023)*. [[PDF]](https://haoxintu.github.io/files/icse23-ds-paper.pdf) [[Poster]](https://haoxintu.github.io/files/icse23-ds-poster.pdf)
 * [ESEC/FSE 2022] **Haoxin Tu**, Lingxiao Jiang, Xuhua Ding, and He Jiang, "FastKLEE: Faster Symbolic Execution via Reducing Redundant Bound Checking of Type-Safe Pointers", in *the Tool Demonstrations Track of ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022)*. [[PDF]](https://haoxintu.github.io/files/fse2022-FastKLEE.pdf) [[Source Code]](https://github.com/haoxintu/FastKLEE) [[Video Demo]](https://youtu.be/iLLlZD384zM) [[Slides]](https://haoxintu.github.io/files/FastKLEE-slides.pdf)
 * [ISSRE 2022] **Haoxin Tu**, He Jiang, Xiaochen Li, Zhilei Ren, Zhide Zhou, and Lingxiao Jiang, "RemGen: Remanufacturing A Random Program Generator for Compiler Testing", in *the 33rd IEEE International Symposium on Software Reliability Engineering (ISSRE 2022)*. [[PDF]](https://haoxintu.github.io/files/issre2022-camera-ready.pdf) [[Source Code]](https://github.com/haoxintu/RemCCG) [[Slides]](https://haoxintu.github.io/files/RemGen-slides.pdf)


### Journal Paper

 * [TR 2022] **Haoxin Tu**, He Jiang, Zhide Zhou, Yixuan Tang, Zhilei Ren, Lei Qiao, and Lingxiao Jiang, "Detecting C++ Compiler Front-end Bugs via Grammar Mutation and Differential Testing", in *IEEE Transactions on Reliability*, 2022. [[IEEE Early Access]](https://ieeexplore.ieee.org/document/9777893) [[Authors' Draft]](https://haoxintu.github.io/files/tr-2022-draft.pdf) [[Bug Reports]](https://github.com/haoxintu/CCOFT/blob/main/reported-bugs.md)
 *  [2023] **Haoxin Tu**, Lingxiao Jiang, Jiaqi Hong, Xuhua Ding, and He Jiang, "Concretely Mapped Symbolic Memory Locations
for Memory Error Detection", Major Revision on *IEEE TSE*. To appear. [[Source Code]](https://github.com/haoxintu/SymLoc)
 * [2023] **Haoxin Tu**, Zhide Zhou, He Jiang, Imam Nur Bani Yusuf, Yuxian Li, and Lingxiao Jiang, "LLM4CBI: Taming LLMs to Generate Effective Test Programs for Compiler Bug Isolation", Major Revision on *IEEE TSE*. [[arXiv]](https://haoxintu.github.io/files/llm4cbi-2023-arxiv.pdf) [[Source Code]](https://github.com/haoxintu/LLM4CBI)


### Ph.D. Thesis

 * Dissertation submitted to [DUT](https://www.dlut.edu.cn/):
   * **Research on Test Program Construction Approaches for Compiler Testing and Debugging**
     * **(in Chinese: 面向编译器测试与调试的程序构造方法研究)** [To appear]
 * Dissertation submitted to [SMU](https://www.smu.edu.sg/):
   * **Boosting Symbolic Execution for Software Reliability and Security (Proposed)** [To appear]


{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
