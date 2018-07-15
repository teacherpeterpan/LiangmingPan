---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Jifan Yu, **Liangming Pan**, Juanzi Li, and Xiaoping Du"
    title: "Predicting Concept-based Research Trends with Rhetorical Framing"
    keywords: "CCKS18"
    month: "August"
    year: "2018"
    booktitle: "In Proceedings of *3th China Conference on Knowledge Graph and Semantic Computing* **(CCKS 2018)**"
    address: "Tianjin, China"
    url: "/publications/CCKS18_Paper.pdf"

  - author: "**Liangming Pan**, Xiaochen Wang, Chengjiang Li, Juanzi Li, and Jie Tang"
    title: "Course Concept Extraction in MOOCs via Embedding-Based Graph Propagation"
    keywords: "IJCNLP17"
    month: "December"
    year: "2017"
    booktitle: "In Proceedings of *the 8th International Joint Conference on Natural Language Processing* **(IJCNLP 2017)**"
    address: "Taipei, Taiwan"
    pages: " pages 875--884"
    url: "/publications/IJCNLP17_Paper.pdf"
    slides: "/publications/IJCNLP17_Slides.pdf"

  - author: "**Liangming Pan**, Chengjiang Li, Juanzi Li, and Jie Tang"
    title: "Prerequisite Relation Learning for Concepts in MOOCs"
    keywords: "ACL17"
    month: "July"
    year: "2017"
    address: "Vancouver, Canada"
    booktitle: "In Proceedings of *the 55th Annual Meeting of the Association for Computational Linguistics* **(ACL 2017)**"
    pages: " pages 1447--1456"
    url: "/publications/ACL17_Paper.pdf"
    slides: "/publications/ACL17_Slides.pdf"

  - author: "**Liangming Pan**, Zhigang Wang, Juanzi Li and Jie Tang"
    title: "Domain Specific Cross-Lingual Knowledge Linking Based on Similarity Flooding"
    keywords: "KSEM16"
    month: "October"
    year: "2016"
    address: "Passau, Germany"
    booktitle: "In Proceedings of *the 9th International Conference on Knowledge Science, Engineering and Management* **(KSEM 2016)**"
    pages: "pages 426--438"
    url: "/publications/KSEM16_Paper.pdf"
    slides: "/publications/KSEM16_Slides.pdf"

  - author: "Yan Zhang, Hailong Jin, **Liangming Pan** and Juanzi Li"
    title: "RiMOM results for OAEI 2016"
    keywords: "OAEI16"
    month: "October"
    year: "2016"
    address: "Kobe, Japan"
    booktitle: "In Proceedings of *the 11th International Workshop on Ontology Matching co-located with the 15th International Semantic Web Conference* **(OM@ISWC 2016)**"
    pages: "pages 210--216"
    url: "/publications/OAEI16_Paper.pdf"

  - author: "Zhigang Wang, **Liangming Pan**, Juanzi Li, Shuangjie Li, Mingyang Li and Jie Tang"
    title: "Boosting to Build a Large-Scale Cross-Lingual Ontology"
    keywords: "CCKS2016"
    month: "September"
    year: "2016"
    address: "Beijing, China"
    booktitle: "In Proceedings of *1th China Conference on Knowledge Graph and Semantic Computing* **(CCKS 2016)**"
    pages: "pages 41--53"
    url: "/publications/CCKS16_Paper.pdf"
    slides: "/publications/CCKS16_Slides.pdf"

  - author: "王巍巍, 王志刚, **潘亮铭**, 刘阳, 张江涛"
    title: "双语影视知识图谱的构建研究"
    keywords: "BMKG"
    journal: "北京大学学报(自然科学版)"
    type: "Journal"
    number: "1"
    pages: "25--34"
    volume: "52"
    year: "2016"
    month: "January"
    url: "/publications/BMKG_Paper.pdf"

---

# Publications
<hr>
## Full Publication List (in chronological order)

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}
    {% if pub.pages %},{{pub.pages}}{% endif %}<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}.
    {% if pub.url %}[[Paper]]({{pub.url}}).{% endif %}
    {% if pub.slides %}[[Slides]]({{pub.slides}}).{% endif %}
    {% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}



