---
title: "Publications"
layout: single
permalink: /publications/
author_profile: true
classes: wide
---

Most recent publications on [Google Scholar]({{ site.data.main_info.google_scholar_recent }}).

<!-- <sup>‡</sup> indicates equal contribution. -->

<ul class="pub-list-compact">
  {% for paper in site.data.publications.papers %}
    <li>
      <span class="pub-title"><strong>{{ paper.title }}</strong></span>
      <span class="pub-meta-line">
        <span class="pub-authors">{{ paper.authors }}.</span>
        <span class="pub-venue"><em>{{ paper.venue }}.</em></span>
        <span class="pub-links-inline">
          {% if paper.paper_pdf %}<a href="{{ paper.paper_pdf | prepend: site.baseurl }}" target="_blank">Paper</a>{% endif %}
          {% if paper.slides %}<a href="{{ paper.slides | prepend: site.baseurl }}" target="_blank">Slides</a>{% endif %}
          {% if paper.poster %}<a href="{{ paper.poster | prepend: site.baseurl }}" target="_blank">Poster</a>{% endif %}
          {% if paper.video %}<a href="{{ paper.video }}" target="_blank">Video</a>{% endif %}
          {% if paper.code %}<a href="{{ paper.code }}" target="_blank">Code</a>{% endif %}
          {% if paper.data %}<a href="{{ paper.data }}" target="_blank">Data</a>{% endif %}
        </span>
      </span>
    </li>
  {% endfor %}
</ul>
