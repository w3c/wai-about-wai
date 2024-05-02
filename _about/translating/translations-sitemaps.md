---
title: "Translations Sitemaps"
nav_title: Translations Sitemaps
lang: en
last_updated: 2024-05-02
description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.

github:
  repository: w3c/wai-about-wai
  path: '_about/translating/translations-sitemaps.md'

permalink: /about/translating/sitemaps/
ref: /about/translating/sitemaps/

image: /content-images/wai-about-wai/social-translations.png
feedbackmail: group-wai-translations@w3.org

footer: |
  <p><strong>Date:</strong> Updated 2 May 2024.</p>
  <p><strong>Editors:</strong> Rémi Bétin and <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>.</p>
  <p>Developed as part of the <a href="https://www.w3.org/WAI/about/projects/wai-coop/">WAI-CooP project</a>, co-funded by the European Commission.</p>
---

Translation sitemaps display the structure of WAI website, and indicate for each page:
- If a translation has been published for this language + its current status ({% include_cached icon.html name="check-circle" %} Up-to-date / {% include_cached icon.html name="warning" %} Needs update).
- If a page has no translation available in this language, and therefore welcomes a volunteer translation.

## Current Translations Sitemaps

_Languages are listed alphabetically by their English names._

{::nomarkdown}
<ul>
  {% for sitemap in site.translations-sitemaps %}
    {% assign langname=site.data.lang[sitemap.tlang].name %}
    {% assign langnativename=site.data.lang[sitemap.tlang].nativeName %}
    <li><a href="{{ sitemap.permalink | relative_url }}"><span lang="sitemap.tlang" style="text-transform: capitalize;">{{ langnativename }}</span> ({{ langname }})</a></li>
  {% endfor %}
</ul>
{:/}