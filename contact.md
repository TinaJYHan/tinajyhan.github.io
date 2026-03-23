---
layout: default
title: Contact
---

<main style="display: flex; align-items: center; justify-content: center; flex-direction: column;" markdown="1">
<div class="contact-container" style="width: 100%;">
    <h1 class="page-title serif" style="margin-bottom: 0.5rem;">聯絡方式 (Contact)</h1>
    <p class="contact-text">Feel free to reach out for academic collaborations or inquiries.</p>

    <div class="contact-links">
        <a href="mailto:tina.h.c@foxmail.com" class="contact-btn">
            <i class="fas fa-envelope"></i>
            tina.h.c@foxmail.com
        </a>

        {% if site.google_scholar != "" %}
        <a href="{{ site.google_scholar }}" class="contact-btn" target="_blank" rel="noopener">
            <i class="fab fa-google-scholar"></i>
            Google Scholar
        </a>
        {% endif %}

        {% if site.orcid != "" %}
        <a href="{{ site.orcid }}" class="contact-btn" target="_blank" rel="noopener">
            <i class="fab fa-orcid"></i>
            ORCID
        </a>
        {% endif %}

        {% if site.researchgate != "" %}
        <a href="{{ site.researchgate }}" class="contact-btn" target="_blank" rel="noopener">
            <i class="fab fa-researchgate"></i>
            ResearchGate
        </a>
        {% endif %}
    </div>
</div>
</main>
