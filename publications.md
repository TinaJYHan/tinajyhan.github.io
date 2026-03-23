---
layout: default
title: Publications
---

<main markdown="1">

<h1 class="page-title serif">學術發表 (Publications)</h1>

## <i class="fas fa-file-alt"></i> 期刊論文 (Journal Articles)

<div class="pub-list">
{% for pub in site.data.publications.journal_articles %}
<div class="pub-item">
  {{ pub.citation | markdownify }}
  {% if pub.status == "under_review" %}<span class="pub-status">Under Review</span>{% endif %}
  {% if pub.doi != "" %}<a href="https://doi.org/{{ pub.doi }}" class="doi-link" target="_blank"><i class="fas fa-external-link-alt"></i> doi:{{ pub.doi }}</a>{% endif %}
</div>
{% endfor %}
</div>

## <i class="fas fa-users"></i> 會議論文 (Conference Proceedings)

<div class="pub-list">
{% for pub in site.data.publications.conference_proceedings %}
<div class="pub-item">
  {{ pub.citation | markdownify }}
  {% if pub.doi != "" %}<a href="https://doi.org/{{ pub.doi }}" class="doi-link" target="_blank"><i class="fas fa-external-link-alt"></i> doi:{{ pub.doi }}</a>{% endif %}
</div>
{% endfor %}
</div>

## <i class="fas fa-book"></i> 著作與譯作 (Books & Translations)

<div class="pub-list">
{% for pub in site.data.publications.books_translations %}
<div class="pub-item">
  {{ pub.citation | markdownify }}
  {% if pub.doi != "" %}<a href="https://doi.org/{{ pub.doi }}" class="doi-link" target="_blank"><i class="fas fa-external-link-alt"></i> doi:{{ pub.doi }}</a>{% endif %}
</div>
{% endfor %}
</div>

</main>
