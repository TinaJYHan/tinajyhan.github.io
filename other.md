---
layout: default
title: Experiences & Skills
---

<main markdown="1">

<h1 class="page-title serif">工作與經歷 (Experiences)</h1>

## <i class="fas fa-briefcase"></i> 工作經歷 (Employment)

{% for job in site.data.employment %}
<h3>{{ job.title }}</h3>
<p><strong>{{ job.period }}</strong> | <em>{{ job.organization }}</em> · {{ job.location }}</p>
<ul>
{% for duty in job.duties %}
<li>{{ duty }}</li>
{% endfor %}
</ul>
{% endfor %}


## <i class="fas fa-project-diagram"></i> 科研項目 (Grants & Projects)

<ul>
{% for grant in site.data.grants %}
<li><strong>{{ grant.role }}</strong>: {{ grant.title }}{% if grant.number != "" %} (編號: {{ grant.number }}){% endif %}</li>
{% endfor %}
</ul>


## <i class="fas fa-tools"></i> 技能與語言 (Skills & Languages)

### 語言 (Languages)
<ul>
{% for lang in site.data.skills.languages %}
<li><strong>{{ lang.name }}</strong> ({{ lang.level }})</li>
{% endfor %}
</ul>

### 專業軟件 (Software Skills)
<ul>
{% for sw in site.data.skills.software %}
<li><strong>{{ sw.name }}</strong> ({{ sw.note }})</li>
{% endfor %}
</ul>

### 其他技能 (Other Skills)
<ul>
{% for skill in site.data.skills.other %}
<li>{{ skill }}</li>
{% endfor %}
</ul>


## <i class="fas fa-chalkboard-teacher"></i> 研學經歷 (Training)

<ul>
{% for t in site.data.training %}
<li>{{ t.name }} ({{ t.location }})</li>
{% endfor %}
</ul>

</main>
