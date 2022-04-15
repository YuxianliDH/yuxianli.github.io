---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
### Conference

 1. Under review.


### Journal

1. [TR'2022] **Haoxin Tu**, He Jiang, Zhide Zhou, Yixuan Tang, Zhilei Ren, Lei Qiao, and Lingxiao Jiang, "Detecting C++ Compiler Front-end Bugs via Grammar Mutation and Differential Testing", on IEEE Transactions on Reliability, 2022. [[Authors' Draft]](https://haoxintu.github.io/files/tr-2022-draft.pdf) [[Bug Reports]](https://github.com/haoxintu/CCOFT/blob/main/reported-bugs.md)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
