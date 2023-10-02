---
title: "Sitemap CSV"
nav_title: Sitemap
github:
  repository: w3c/wai-about-wai
  path: '_about/sitemaps/sitemap-csv.md'
permalink: /about/translating/sitemap-csv/
ref: /about/translating/sitemap-csv/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a draft documentation to guide volunteer translators.

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

This page allows to copy-and-paste a CSV-formatted list of most of WAI resources and translated versions.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

<textarea id="story" name="story" rows="200" cols="130">
{%- assign alldocs=site.documents | concat: site.pages -%}
Level;Section;Original title;Original page;Language;Translated Title;Translated Page;Status&#13;&#10;
{%- for section in site.data.navigation -%}
{%- for page in section.pages -%}
{%- assign original=alldocs | where_exp:"item", "item.lang == 'en' or item.lang == nil" | where_exp:"item", "item.ref == page.url or item.url == page.url" | first %}
{%- assign versions=alldocs | where_exp:"item", "item.ref == page.url" -%}
{%- capture en-date %}{{original.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
{% for t in versions %}
{%- capture t-date %}{{t.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
Level 1;
{%- if section.name.en -%}"{{ section.name.en }}"{%- elsif section.name -%}"{{ section.name }}"{%- else -%}""{%- endif -%};{%- if original.title -%}"{{ original.title }}"{%- else -%}""{%- endif -%};{%- if original.url -%}{{ original.url | absolute_url }}{%- else -%}""{%- endif -%};{%- if t.lang -%}{{ t.lang }}{%- else -%}""{%- endif -%};{%- if t.title -%}"{{ t.title }}"{%- else -%}""{%- endif -%};"{{ t.url | absolute_url }}";
{%- if t.lang != 'en' and t-date < en-date -%}
"Needs update"
{%- elsif t.lang != 'en' and t-date >= en-date -%}
"Up-to-date"
{%- else-%}
""
{%- endif -%};&#13;
{%- endfor -%}
{%- for subpage in page.pages -%}
{%- assign original2=alldocs | where_exp:"item", "item.lang == 'en' or item.lang == nil" | where_exp:"item", "item.ref == subpage.url or item.url == subpage.url" | first %}
{%- assign versions2=alldocs | where_exp:"item", "item.ref == subpage.url" -%}
{%- capture en2-date %}{{original2.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
{% for t2 in versions2 %}
{%- capture t2-date %}{{t2.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
Level 2;
{%- if section.name.en -%}"{{ section.name.en }}"{%- elsif section.name -%}"{{ section.name }}"{%- else -%}""{%- endif -%};{%- if original2.title -%}"{{ original2.title }}"{%- else -%}""{%- endif -%};{%- if original2.url -%}{{ original2.url | absolute_url }}{%- else -%}""{%- endif -%};{%- if t2.lang -%}{{ t2.lang }}{%- else -%}""{%- endif -%};{%- if t2.title -%}"{{ t2.title }}"{%- else -%}""{%- endif -%};"{{ t2.url | absolute_url }}";
{%- if t2.lang != 'en' and t2-date < en2-date -%}
"Needs update"
{%- elsif t2.lang != 'en' and t2-date >= en2-date -%}
"Up-to-date"
{%- else-%}
""
{%- endif -%};&#13;
{%- endfor -%}
{%- for subsubpage in subpage.pages -%}
{%- assign original3=alldocs | where_exp:"item", "item.lang == 'en' or item.lang == nil" | where_exp:"item", "item.ref == subsubpage.url or item.url == subsubpage.url" | first %}
{%- assign versions3=alldocs | where_exp:"item", "item.ref == subsubpage.url" -%}
{%- capture en3-date %}{{original3.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
{% for t3 in versions3 %}
{%- capture t3-date %}{{t3.last_updated | date: '%s' | plus: 0 }}{% endcapture -%}
Level 3;
{%- if section.name.en -%}"{{ section.name.en }}"{%- elsif section.name -%}"{{ section.name }}"{%- else -%}""{%- endif -%};{%- if original3.title -%}"{{ original3.title }}"{%- else -%}""{%- endif -%};{%- if original3.url -%}{{ original3.url | absolute_url }}{%- else -%}""{%- endif -%};{%- if t3.lang -%}{{ t3.lang }}{%- else -%}""{%- endif -%};{%- if t3.title -%}"{{ t3.title }}"{%- else -%}""{%- endif -%};"{{ t3.url | absolute_url }}";
{%- if t3.lang != 'en' and t3-date < en3-date -%}
"Needs update"
{%- elsif t3.lang != 'en' and t3-date >= en3-date -%}
"Up-to-date"
{%- else-%}
""
{%- endif -%};&#13;
{%- endfor -%}
{%- endfor -%}
{%- endfor -%}
{%- endfor -%}
{%- endfor -%}
</textarea>


