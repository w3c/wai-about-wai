---
title: "French Translations"
nav_title: French translations progress
github:
  repository: w3c/wai-about-wai
  path: '_about/sitemaps/sitemap-fr.md'
permalink: /about/translating/sitemaps/sitemap-fr/
ref: /about/translating/sitemaps/sitemap-fr/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a draft documentation to guide volunteer translators.

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 13 September 2023.</p>
  <p><strong>Editor:</strong> Rémi Bétin.</p>

inline_css: |
  dl.translations > div {
    margin-block-end: 1em;
  }
---
{::nomarkdown}
{% include box.html type="start" h="2" title="Summary" class="full" %}
{:/}

This page lists the status of French translations for most pages on the WAI website.

{::nomarkdown}
{% include box.html type="end" %}

<ul class="results-by-category">
  <li class="results-by-category__item">
    <span class="results-by-category__number">13</span> 
    <span class="results-by-category__label">Up-to-date</span>
  </li>
  <li class="results-by-category__item">
    <span class="results-by-category__number">9</span> 
    <span class="results-by-category__label">Need update</span>
  </li>
  <li class="results-by-category__item">
    <span class="results-by-category__number">188</span> 
    <span class="results-by-category__label">Missing</span>
  </li>
</ul>

{% include excol.html type="all" %}
{% assign sections=site.data.navigation | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
{%- for section in sections -%}
  {% include excol.html type="start" %}
  <h2>
  {%- if section.name.en -%}
    {{ section.name.en }}
  {%- else -%}
    {{ section.name }}
  {%- endif -%}
  </h2>
  {% include excol.html type="middle" %}
  {% assign sections-pages=section.pages | where_exp:"item", "item.mainnav != false and item.hide != true" -%}
  {%- for page in sections-pages -%}
    {% assign pagedata=site.pages | where_exp:"item", "item.lang == 'en'" | where_exp:"item", "item.ref == page.url" | first %}
    {%- capture issue_body_update | newline_to_br -%}
I would like to update the [French] translation of the following resource:
- Page URL: {{page.url | absolute_url}}
- Github Repository: [{{pagedata.github.repository}}](https://github.com/{{pagedata.github.repository}})

I have read the information on Translating WAI Documents at https://www.w3.org/WAI/about/translating/

I will wait for confirmation that the resource is ready for translation.

https://github.com/w3c/wai-translations/labels/translation-update
    {%- endcapture -%}
    {%- capture issue_body_new | newline_to_br -%}
I would like to translate into [French] the following resource:
- Page URL: {{page.url | absolute_url}}
- Github Repository: [{{pagedata.github.repository}}](https://github.com/{{pagedata.github.repository}})

I have read the information on Translating WAI Documents at https://www.w3.org/WAI/about/translating/

I will wait for confirmation that the resource is ready for translation.

https://github.com/w3c/wai-translations/labels/initial-translation
    {%- endcapture -%}
    {% assign t=site.pages | where_exp:"item", "item.lang == 'fr' and item.ref == page.url" | first %}
    {%- capture page_title -%}
      {%- if t != nil -%}
        <a href="{{ t.permalink | relative_url }}"> {{ t.title }} ({{ pagedata.title }})
      {%- elsif t == nil and pagedata.permalink != nil -%}
        <a href="{{ pagedata.permalink | relative_url }}">{{ pagedata.title }}
      {%- elsif t == nil and pagedata.permalink == nil and page.name.en != nil -%}
        <a href="{{ page.url | relative_url }}">{{ page.name.en }}
      {%- else -%}
        <a href="{{ page.url | relative_url }}">{{ page.name }}
      {%- endif -%}
      </a>
    {%- endcapture -%}
    {% capture t-date %}{{t.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
    {% capture en-date %}{{pagedata.last_updated | date: '%s' | plus: 0 }}{% endcapture %}
    {%- capture t_status -%}
      {%- if t == nil -%}none
      {%- elsif t.size != 0 and t-date < en-date -%}outdated
      {%- elsif t.size != 0 and t-date >= en-date -%}uptodate
      {%- endif -%}
    {%- endcapture -%}
    {% include box.html type="start" title=page_title h="3" %}
    {%- case t_status -%}
      {%- when "none" -%}
        <p>{% include_cached icon.html name="ex-circle" %} No translation available</p>
        <p><a href="https://github.com/w3c/wai-translations/issues/new?title=[fr]+{{pagedata.title | url_encode}}&body={{issue_body_new | url_encode}}">Volunteer to translate this page</a></p>
      {%- when "outdated" -%}
        <p><mark>{% include_cached icon.html name="warning" %} Translation needs update</mark><p>
        <p><a href="https://github.com/w3c/wai-translations/issues/new?title=[fr]+{{pagedata.title | url_encode}}&body={{issue_body_update | url_encode}}">Volunteer to update the translation</a></p>
      {%- when "uptodate" -%}
        <p>{% include_cached icon.html name="check-circle" %} Up-to-date</p>
    {%- endcase -%}
    {% include box.html type="end" %}
  {% endfor %}
{% include excol.html type="end" %}
{% endfor %}
{:/}