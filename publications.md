---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Daniel Haas, Jason Ansel, Lydia Gu, Adam Marcus"
    title: "Argonaut: Macrotask Crowdsourcing for Complex Data Processing"
    keywords: "Locu"
    month: "September"
    year: "2015"
    address: "Kohala Coast, Hawaii"
    booktitle: "International Conference on Very Large Data Bases"
    url: 2015vldb-argonaut.pdf
    bibtex: 2015vldb-argonaut.bib


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



