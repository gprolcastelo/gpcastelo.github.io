---
layout: page
title: Publications
---
<ul class="pub-list">
{% for pub in site.data.publications %}
  <li class="pub-item">
    <p class="pub-title">{{ pub.title }}</p>
    <p class="pub-meta">{{ pub.authors | replace: "Guillermo Prol-Castelo", "<strong>Guillermo Prol-Castelo</strong>" }} — <em>{{ pub.venue }}</em>, {{ pub.year }}</p>
    {% if pub.note %}<p class="pub-note">{{ pub.note }}</p>{% endif %}
    <p class="pub-links">
      {% if pub.doi_url %}<a href="{{ pub.doi_url }}" target="_blank" rel="noopener">DOI</a>{% endif %}
      {% if pub.pdf_url and pub.pdf_url != "" %} · <a href="{{ pub.pdf_url }}" target="_blank" rel="noopener">PDF</a>{% endif %}
      {% if pub.status %}<span class="pub-status">{{ pub.status }}</span>{% endif %}
    </p>
  </li>
{% endfor %}
</ul>
