---
title: About
permalink: /
---

<section id="about" class="prose" markdown="1">
<h2 class="sec"><span class="no">1.0</span>About</h2>

I am a Colombian-Australian designer and researcher based in Amsterdam, working on AI systems that open futures rather than foreclose them. Working from a queer mestiza perspective, my PhD at TU Delft's [DCODE Network]({{ site.dcode_url }}) (2021–2026), a Horizon 2020 Marie Skłodowska-Curie project, reorients design toward co-predictive relations: recoding simulations and digital twins from prediction, which pronounces the future, to co-performance, which opens it.

I am co-founder and Head of Design and Research at [Parallel Studio]({{ site.parallel_url }}), a practice working across design research, complex systems and human–AI relations — treating relational living and computational systems as a design material. Parallel builds instruments that let institutions see and work on those relations directly. My research develops co-prediction as a different basis for designing with computational intelligence, and I oversee its design and research for Pask, the studio's first product, through which that practice becomes possible.

I co-head [Monstrous Futurities: Practices in (Un)learning, (Un)making, and (Un)worlding]({{ site.monstrous_url }}), a two-year temporary Master's programme at the Sandberg Instituut which began in September 2025, run with Romany Dear. The programme engages monstrous imaginaries and their subversive potential through transdisciplinary practice, taking speculation and fabulation as ways of retaining hope and a sense of futurity while living in uncertainty. With Romany, I created a living curriculum and pedagogical framework enacted through a cyclical structure informed by students' lived experience and its intersections with transfeminist, queer, crip and post-human theories and practices.

Formerly Design Futures & Insight Lead at Deloitte Digital (AU–NL, 2015–2021), I supported organisations in participatory, civic-oriented strategic, service and product design initiatives. I co-founded Australia's first queer womxn-led makerspace (2014). My work has been featured internationally at the likes of PRIMER Festival, Telefónica Madrid, and TEDx Sydney. Recent writing appears in *AI & SOCIETY*, the DRS2026 proceedings, and *VOLUME* (upcoming).
</section>

<section id="currently">
<h2 class="sec"><span class="no">2.0</span>Currently</h2>
<ul class="index">
  <li>
    <span class="no">[01]</span>
    <span>
      <span class="t"><a href="{{ site.parallel_url }}">Parallel Studio ↗</a></span> — Founder, Design &amp; Research
      <span class="d">A practice working with relational living and computational systems as a design material — building instruments that let institutions see and work on those relations directly, beginning with Pask, the studio's first product.</span>
    </span>
  </li>
  <li>
    <span class="no">[02]</span>
    <span>
      <span class="t"><a href="{{ site.monstrous_url }}">Monstrous Futurities ↗</a></span> — Co-head, Sandberg Instituut
      <span class="d">Practices in (Un)learning, (Un)making, and (Un)worlding: a two-year temporary Master's programme (2025–2027, with Romany Dear) engaging monstrous imaginaries through transdisciplinary practice, speculation and fabulation.</span>
    </span>
  </li>
</ul>
</section>

<section id="writing">
<h2 class="sec"><span class="no">3.0</span>Writing</h2>
<ul class="index">
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for pub in pubs %}
  <li>
    <span class="no">[{{ forloop.index | prepend: '00' | slice: -2, 2 }}]</span>
    <span>
      <span class="t">{% if pub.link %}<a href="{% if pub.link contains '://' %}{{ pub.link }}{% else %}{{ pub.link | relative_url }}{% endif %}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}</span>
      — {{ pub.venue }}, {{ pub.date | date: "%Y" }}
      <span class="d">{{ pub.summary }}
      {% if pub.pdf %}<a href="{{ pub.pdf | relative_url }}">PDF ↓</a>{% endif %}
      {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">doi.org/{{ pub.doi }} ↗</a>{% endif %}</span>
    </span>
  </li>
{% endfor %}
</ul>
</section>

<section id="links">
<h2 class="sec"><span class="no">4.0</span>Links</h2>
<ul class="index">
  <li><span class="no">[01]</span><span><a href="{{ site.substack_url }}">Substack ↗</a> <span class="d">Newsletter — shorter, more frequent writing between the papers.</span></span></li>
  <li><span class="no">[02]</span><span><a href="{{ site.dissertation_doi }}">TU Delft Repository ↗</a> <span class="d">The dissertation of record, open access.</span></span></li>
  <li><span class="no">[03]</span><span><a href="{{ site.dcode_url }}">DCODE Network ↗</a> <span class="d">Horizon 2020 Marie Skłodowska-Curie research network (2021–2026).</span></span></li>
  <li><span class="no">[04]</span><span><a href="https://futuress.org/community/grace/">Futuress ↗</a> <span class="d">Community profile and writing.</span></span></li>
  <li><span class="no">[05]</span><span><a href="{{ site.instagram_url }}">Instagram ↗</a> <span class="d">@gracetortuga</span></span></li>
  <li><span class="no">[06]</span><span><a href="{{ site.x_url }}">X ↗</a> <span class="d">@grace_polifroni</span></span></li>
  <li><span class="no">[07]</span><span><a href="{{ site.linkedin_url }}">LinkedIn ↗</a></span></li>
  <li><span class="no">[08]</span><span><a href="mailto:{{ site.email }}">{{ site.email }}</a> <span class="d">The best way to reach me.</span></span></li>
</ul>
</section>
