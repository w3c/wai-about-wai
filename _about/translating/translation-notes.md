---
title: "Translation Notes"
nav_title: Translation Notes
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/translation-notes.md'
permalink: /about/translating/translation-notes/
ref: /about/translating/translation-notes/
lang: en
last_updated: 2023-11-09
description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 9 November 2023.</p>
  <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a> and Rémi Bétin.</p>
  <p>Developed as part of the <a href="https://www.w3.org/WAI/about/projects/wai-coop/">WAI-CooP project</a>, co-funded by the European Commission.</p>
---

{::options toc_levels="2" /}
{::nomarkdown}
{% include toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include toc.html type="end" %}
{:/}

{::nomarkdown}
{% include excol.html type="all" %}
{:/}

{::nomarkdown}
{% include excol.html type="start" id="wcag-glance" %}
{:/}
## WCAG 2 at a Glance
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}

Please consider the wording in the WCAG 2.2 success criteria. If there is a translation of WCAG 2 in your language, review it thoughtfully. This text is not the same as the success criteria wording &mdash; it is a paraphrased summary that is intended to be easier to understand and accurate - yet it does not need to be comprehensive.

Please collaborate with others who are familiar with WCAG to refine this wording in your language. Thank you!

{::nomarkdown}
{% include excol.html type="end" %}
{:/}

{::nomarkdown}
{% include excol.html type="start" id="people-use-web" %}
{:/}
## How People with Disabilities Use the Web
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}

The title "How People with Disabilities Use the Web" is a statement. The title is **not a question**. For translation, it might help to think of the title "How People with Disabilities Use the Web" as **a shorter version of** "An Introduction to How People with Disabilities Use the Web" or "Description of How People with Disabilities Use the Web".

{::nomarkdown}
{% include excol.html type="end" %}
{:/}



{::nomarkdown}
{% include excol.html type="start" id="perspective-videos" %}
{:/}
## Web Accessibility Perspectives Videos
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}

### Changelog/Acknowledgements

Do not translate `changelog.md` and `acknowledgements.md`.

### Links with images in index page

In `index.[lang].md`: add the language shortcode of your translation at the end of the URLs listed in "Perspectives Videos"

Example (French translation):
```markdown
- [![](img/thumbnails/keyboard.jpg)<br>Compatibilité avec le clavier]({{ "/perspective-videos/keyboard/fr" | relative_url }})
```

### Subtitles & descriptions

Follow [Translating Video Subtitles and Descriptions](/translating/guides/video-subtitles/) guidance.

{::nomarkdown}
{% include excol.html type="end" %}
{:/}


{::nomarkdown}
{% include excol.html type="start" id="standards-overview" %}
{:/}
## Standards Overview
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}


### Links to WCAG standards

The page contains links to WCAG 2.0, 2.1 and 2.2.

If an Authorized Translation of a WCAG standard has been published in your language, please point to the translated version.

Example:

```
- [Le standard WCAG 2.0](https://www.w3.org/Translations/WCAG20-fr/)
- [Le standard WCAG 2.1](https://www.w3.org/Translations/WCAG21-fr/)
```

If not, translate the link text but keep the link to the English version.

Example:

```
- [Le standard WCAG 2.2](https://www.w3.org/TR/WCAG22//)
```

### [Image at the bottom](https://www.w3.org/WAI/content-images/wai-std-gl-overview/specs.png)

For now, it is OK to leave the image in English. (It only illustrates the information above, and does not provided substantial additional information.) We are working on an SVG version of that image, with support for translation. We will update this section and notify existing translators when it is ready.

{::nomarkdown}
{% include excol.html type="end" %}
{:/}

{::nomarkdown}
{% include excol.html type="start" id="tutorials" %}
{:/}
## Tutorials
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}

Tutorials resources use a dynamic footer, using specific metadata set in the "front matter" of each page.

Example:
```yaml
metafooter: true
editors:
  - Eric Eggert: "https://www.w3.org/People/yatil/"
  - Shadi Abou-Zahra: "https://www.w3.org/People/shadi/"
update_editors:
  - Brian Elton
contributing_participants:
  - see <a href="/WAI/tutorials/acknowledgements/">Acknowledgements</a>
support: Developed by the Education and Outreach Working Group (<a href="https://www.w3.org/groups/wg/eowg">EOWG</a>). Developed with support from the <a href="https://www.w3.org/WAI/ACT/">WAI-ACT project</a>, co-funded by the <strong>European Commission <abbr title="Information Society Technologies">IST</abbr> Programme</strong>.
```

1. Translate content in `editors`, `update_editors`, `contributing_participants` and `support`.\
   Note: Translate the Working Group name and leave the Working Group acronym in English.
2. Add translations for the following terms, used by the footer, in [translations.yml file](https://github.com/w3c/wai-website-data/blob/master/translations.yml) located in [wai-website-data repository](https://github.com/w3c/wai-website-data/):
- "Editors:"
- "Update Editor:"
- "Status"
- "Updated"
- "first published"

{::nomarkdown}
{% include excol.html type="end" %}
{:/}


{::nomarkdown}
{% include excol.html type="start" id="video-introduction" %}
{:/}
## Video Introduction to Web Accessibility and W3C Standards
{::nomarkdown}
{% include excol.html type="middle" %}
{:/}

1. Check if the [player is available in your translated language](https://github.com/ableplayer/ableplayer/blob/master/README.md#user-content-supported-languages).

2. Translate the "Translations" section of the page accordingly:

* **If the player _is_ available in the translated language**:
  * Translate the following words from the video player interface:
    * "Captions"
    * "Show transcript"
    * "Language"
  * Please also update the image per the instructions below.<br>_If you are not able to update the image, let us know._
    * Make a new image to replace [show-language.png](https://www.w3.org/WAI/content-images/wai-video-standards-and-benefits/show-language.png). The circle is 7px #eed009 / rgb(238,208,9).
    * Name it `show-language.[language shortcode].png`\
      For example: `show-language.fr.png`
    * Upload it to the [content-images folder](https://github.com/w3c/wai-video-standards-and-benefits/tree/master/content-images/wai-video-standards-and-benefits)
      * Select "Upload files"
      * Drag or choose the file
      * Select "Commit changes"
    * In your translation, add the language shortcode to the image path.
* **If the player is _not_ available in the translated language**:
  * Do not translate the following words from the video player interface; leave them in English:
    * "Captions"
    * "Show transcript"
    * "Language"
  * Mark up the English words with the lang attribute:\
    `<span lang="en">Captions</span>`.

{::nomarkdown}
{% include excol.html type="end" %}
{:/}



