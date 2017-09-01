---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
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
    {% if pub.url %}[Paper]({{pub.url}}).{% endif %}
    {% if pub.slides %}[Slides]({{pub.slides}}).{% endif %}
    {% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}



