---
title: "French Translations Progress"
nav_title: French Translations Progress
lang: en
last_updated: 2023-12-06
description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.

github:
  repository: w3c/wai-about-wai
  path: '_about/sitemaps/sitemap-fr.md'

permalink: /about/translating/sitemaps/sitemap-fr/
ref: /about/translating/sitemaps/sitemap-fr/

image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p>Developed as part of the <a href="https://www.w3.org/WAI/about/projects/wai-coop/">WAI-CooP project</a>, co-funded by the European Commission.</p>

#Custom frontmatter for this page
tlang: fr
---
{% assign tlangname=site.data.lang[page.tlang].name %}
{% assign alldocs=site.documents | concat: site.pages %}

{::nomarkdown}
{% include box.html type="start" h="2" title="Summary" class="full" %}
{:/}

This page lists the status of {{ tlangname }} translations for most pages on the WAI website.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{% include excol.html type="all" %}

{% include excol.html type="start" %}

## Priorities Status

{% include excol.html type="middle" %}

{::nomarkdown}
{% if site.data.translations-priorities %}
  {%- for prio in site.data.translations-priorities -%}
    {%- include t-status.html page=prio h="3" -%}
      {%- for priosub in prio.pages -%}
        {%- include t-status.html page=priosub h="3" -%}
        {% include box.html type="end" %}
      {%- endfor -%}
    {% include box.html type="end" %}
  {%- endfor -%}
{% endif %}
{:/}

{% include excol.html type="end" %}

## Sitemap

{::nomarkdown}
{% assign sections=site.data.navigation | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
{%- for section in sections -%}
  {% include excol.html type="start" %}
  <h3>
  {%- if section.name.en -%}
    {{ section.name.en }}
  {%- else -%}
    {{ section.name }}
  {%- endif -%}
  </h3>
  {% include excol.html type="middle" %}
  {% assign pages=section.pages | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
  {%- for p in pages -%}
    {%- include t-status.html page=p h="4" -%}
    {% assign subpages=p.pages | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
    {%- for subpage in subpages -%}
      {%- include t-status.html page=subpage h="5" -%}
    {% include box.html type="end" %}
    {% endfor %}
    {% include box.html type="end" %}
  {% endfor %}
{% include excol.html type="end" %}
{% endfor %}
{:/}