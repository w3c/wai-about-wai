---
title: "Sitemap"
nav_title: Sitemap
github:
  repository: w3c/wai-about-wai
  path: '_about/sitemaps/sitemap.md'
permalink: /about/translating/sitemaps/general/
ref: /about/translating/sitemaps/general/
lang: en
doc-note-type: draft

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 7 September 2023.</p>
  <p><strong>Editor:</strong> Rémi Bétin.</p>

inline_css: |
  dl.translations > div {
    margin-block-end: 1em;
  }
---

{::nomarkdown}
{% include box.html type="start" h="2" title="Summary" class="full" %}
{:/}

This page lists most pages on the WAI website, and their translated versions, when existing.

{::nomarkdown}
{% include box.html type="end" %}

{% include excol.html type="all" %}
{% assign sections=site.data.navigation | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
{%- for section in sections -%}
  {% include excol.html type="start" %}
  <h2>
  {%- if section.name.en -%}
    {{ section.name.en }}
  {%- else -%}
    {{ section.name }}
  {%- endif -%}</h2>
  {% include excol.html type="middle" %}
  {% assign sections-pages=section.pages | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
  {%- for page in sections-pages -%}
    <h3>
      <a href="{{ page.url | relative_url }}">
      {%- if page.name.en -%}
        {{ page.name.en }}
      {%- else -%}
        {{ page.name }}
      {%- endif -%}
      </a>
    </h3>
    {% assign translations=site.pages | where_exp:"item", "item.lang != 'en'" | where_exp:"item", "item.lang !=  nil" | where_exp:"item", "item.ref == page.url" | sort: "item.lang" %}
    {%- for t in translations -%}
      {% capture t-date %}{{t.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
      {% assign original=site.pages | where_exp:"item", "item.lang == 'en'" | where_exp:"item", "item.ref == t.ref" | first %}
      {% capture en-date %}{{original.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
      <dl>
        <div>
          <dt>[{{ t.lang }}] <a href="{{ t.url | relative_url }}">
            {{ t.title }}</a></dt>
          <dd>
          {%- if t-date < en-date -%}
          {% include_cached icon.html name="warning" %} Needs update
          {%- else -%}
          {% include_cached icon.html name="check-circle" %} Up-to-date
          {%- endif -%}
          </dd>
        </div>
      </dl>
    {%- endfor -%}
    {% assign page-subpages=page.pages | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
    {%- for subpage in page-subpages -%}
      <h4>
        <a href="{{ subpage.url | relative_url }}">
        {%- if subpage.name.en -%}
          {{ subpage.name.en }}
        {%- else -%}
          {{ subpage.name }}
        {%- endif -%}
        </a>
      </h4>
      {% assign translations=site.pages | where_exp:"item", "item.lang != 'en'" | where_exp:"item", "item.lang !=  nil" | where_exp:"item", "item.ref == subpage.url" | sort: "item.lang" %}
      {%- for t2 in translations -%}
        {% capture t2-date %}{{t2.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
        {% assign original2=site.pages | where_exp:"item", "item.lang == 'en'" | where_exp:"item", "item.ref == t2.ref" | first %}
        {% capture en2-date %}{{original2.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
        <dl>
          <div>
            <dt>[{{ t2.lang }}] <a href="{{ t2.url | relative_url }}">
              {{ t2.title }}</a></dt>
            <dd>
            {%- if t2-date < en2-date -%}
              {% include_cached icon.html name="warning" %} Needs update
            {%- else -%}
              {% include_cached icon.html name="check-circle" %} Up-to-date
            {%- endif -%}
            </dd>
          </div>
        </dl>
      {%- endfor -%}
    {%- endfor -%}
  {% endfor %}
{% include excol.html type="end" %}
{% endfor %}
{:/}