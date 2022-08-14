---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
### Conference

 * [ESEC/FSE 2022] **Haoxin Tu**, Lingxiao Jiang, Xuhua Ding, and He Jiang, "FastKLEE: Faster Symbolic Execution via Reducing Redundant Bound Checking of Type-Safe Pointers", in *the Tool Demonstrations Track of ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2022)*. To appear. [[Source Code]](https://github.com/haoxintu/FastKLEE) [[Video Demo]](https://youtu.be/fjV_a3kt-mo)

 * [ISSRE'2022] **Haoxin Tu**, He Jiang, Xiaochen Li, Zhilei Ren, Zhide Zhou, and Lingxiao Jiang, "RemGen: Remanufacturing A Random Program Generator for Compiler Testing", in *the 33rd IEEE International Symposium on Software Reliability Engineering (ISSRE 2022)*. To appear.


### Journal

 * [TR'2022] **Haoxin Tu**, He Jiang, Zhide Zhou, Yixuan Tang, Zhilei Ren, Lei Qiao, and Lingxiao Jiang, "Detecting C++ Compiler Front-end Bugs via Grammar Mutation and Differential Testing", in *IEEE Transactions on Reliability*, 2022. [[IEEE Early Access]](https://ieeexplore.ieee.org/document/9777893) [[Authors' Draft]](https://haoxintu.github.io/files/tr-2022-draft.pdf) [[Bug Reports]](https://github.com/haoxintu/CCOFT/blob/main/reported-bugs.md)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
