---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
### Conference
 * [ICSE 2023] **Haoxin Tu**, "Boosting Symbolic Execution for Heap-based Vulnerability Detection and Exploit Generation", in *the Doctoral Symposium Track of IEEE/ACM International Conference on Software Engineering (ICSE 2023)*. [[PDF]](https://haoxintu.github.io/files/icse23-ds-paper.pdf) [[Poster]](https://haoxintu.github.io/files/icse23-ds-poster.pdf)
 * [ESEC/FSE 2022] **Haoxin Tu**, Lingxiao Jiang, Xuhua Ding, and He Jiang, "FastKLEE: Faster Symbolic Execution via Reducing Redundant Bound Checking of Type-Safe Pointers", in *the Tool Demonstrations Track of ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022)*. [[PDF]](https://haoxintu.github.io/files/fse2022-FastKLEE.pdf) [[Source Code]](https://github.com/haoxintu/FastKLEE) [[Video Demo]](https://youtu.be/iLLlZD384zM) [[Slides]](https://haoxintu.github.io/files/FastKLEE-slides.pdf)
 * [ISSRE 2022] **Haoxin Tu**, He Jiang, Xiaochen Li, Zhilei Ren, Zhide Zhou, and Lingxiao Jiang, "RemGen: Remanufacturing A Random Program Generator for Compiler Testing", in *the 33rd IEEE International Symposium on Software Reliability Engineering (ISSRE 2022)*. [[PDF]](https://haoxintu.github.io/files/issre2022-camera-ready.pdf) [[Source Code]](https://github.com/haoxintu/RemCCG) [[Slides]](https://haoxintu.github.io/files/RemGen-slides.pdf)


### Journal

 * [TR 2022] **Haoxin Tu**, He Jiang, Zhide Zhou, Yixuan Tang, Zhilei Ren, Lei Qiao, and Lingxiao Jiang, "Detecting C++ Compiler Front-end Bugs via Grammar Mutation and Differential Testing", in *IEEE Transactions on Reliability*, 2022. [[IEEE Early Access]](https://ieeexplore.ieee.org/document/9777893) [[Authors' Draft]](https://haoxintu.github.io/files/tr-2022-draft.pdf) [[Bug Reports]](https://github.com/haoxintu/CCOFT/blob/main/reported-bugs.md)
 * [2023] **Haoxin Tu**, Zhide Zhou, He Jiang, Imam Nur Bani Yusuf, Yuxian Li, and Lingxiao Jiang, "LLM4CBI: Taming LLMs to Generate Effective Test Programs for Compiler Bug Isolation", under review on IEEE TSE. [[arXiv]](https://haoxintu.github.io)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
