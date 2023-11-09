---
title: "Creating a New Translation"
nav_title: New translation
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/new-translation.md'
permalink: /about/translating/guides/new-translation/
ref: /about/translating/guides/new-translation/
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

{::options toc_levels="2,3" /}
{::nomarkdown}
{% include toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include toc.html type="end" %}
{:/}

## Initial steps

Before starting:
- Find the language short code "subtag" from [Language Subtag Registry {% include_cached external.html %}](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry). You will use it at multiple times during the translation.

## Step 1: Create a new file {#create-file}

Duplicate the file used by the original version, with the language shortcode added to the middle of the filename, as follows:

{::nomarkdown}
{% include box.html type="start" title="Example" %}
{:/}

- Original English file: `index.md`
- New Korean file: `index.ko.md`

{::nomarkdown}
{% include box.html type="end" %}
{:/}

## Step 2: Update "front matter" metadata {#frontmatter}

{::nomarkdown}
{% include box.html type="start" class="highlighted" %}
{:/}

From now on, only edit the newly created translation file.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

At the top of WAI website files are some metadata, also known as "front matter".

Your first step into the file is to update this section.

{::nomarkdown}
{% include box.html type="start" title="Example of front matter (this may differ on your file)" %}
{:/}
```yaml
---
title: Evaluation Tools Overview
lang: en
last_updated: 2020-04-28

github:
  repository: w3c/wai-eval-tools-overview
  path: "content/index.md"

permalink: /test-evaluate/tools/
ref: /test-evaluate/tools/

footer: >
   <p><strong>Date:</strong> Updated 28 April 2020.</p>
   <p><strong>Editor:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>.</p>
   <p>Video developed by the Education and Outreach Working Group (<a href="http://www.w3.org/WAI/EO/">EOWG</a>) with support from the <a href="https://www.w3.org/WAI/about/projects/wai-guide/">WAI-Guide</a> project funded by the European Commission (EC) under the Horizon 2020 program (Grant Agreement 822245). <a href="./acknowledgements/">Acknowledgements</a>.</p>
---
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

### General instructions for front matter

#### 2.1. Update the following front matter values:

`lang`
- Replace the original value (`en`) with the language shortcode of your translation.  

`last_updated`
- Change `last_updated: 2000-00-00` to the date you finish the translation.  
  Use the format: YYYY-MM-DD (with month in the middle).

`path` (below `github`)
- Add the language shortcode at the middle of the filename.

`permalink`
- Add the language shortcode at the end of the permalink, with no `/` at the end.

`footer` (not always present)
- If this attribute is present, translate its content.
- Do not change the dates in this section. Those dates should be the same in your translation as in the English version.

#### 2.2. Add translators & contributors names.

After `last_updated`, add these lines, depending on how many translators there are and if there are contributors.  

Policy for names and links is introduced in [Translating WAI Resources]({{ "/about/translating" | relative_url }}#links).

{::nomarkdown}
{% include box.html type="start" %}
{:/}
```yaml
translators:
  - name: "Your Name"
contributors:
  - name: "Other Name"
  - name: "Other Name"
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

Or, if the lines are there with "`#`" before them to comment them out: delete the # and the space.

#### Updated Example

{::nomarkdown}
{% include box.html type="start" title="Updated front matter for a translation into French" %}
{:/}
{% include excol.html type="start" id="optional-id" %}

Show example

{% include excol.html type="middle" %}

```yaml
---
title: Evaluation Tools Overview
lang: fr
last_updated: 2023-09-13

translators:
  - name: "Your Name"
contributors:
  - name: "Other Name"
  - name: "Other Name"

github:
  repository: w3c/wai-eval-tools-overview
  path: "content/index.fr.md"

permalink: /test-evaluate/tools/fr
ref: /test-evaluate/tools/

footer: >
  <p><strong>Date :</strong> Mise à jour : 28 avril 2020.</p>
  <p><strong>Rédactrice :</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>.</p>
  <p>Vidéo créée par le groupe de travail Éducation et Promotion (<a href="http://www.w3.org/WAI/EO/">EOWG</a>) avec le soutien du projet <a href="https://www.w3.org/WAI/about/projects/wai-guide/">WAI-Guide</a> financé par la Commission européenne (CE) dans le cadre du programme Horizon 2020 (convention de subvention n°822245) <a href="./acknowledgements/">Remerciements</a>.</p>
---
```

{% include excol.html type="end" %}
{::nomarkdown}
{% include box.html type="end" %}
{:/}

### Follow additional inline instructions

Many resources have inline instructions in the front matter (after the "`#`" character). 

Please follow these instructions. It will help you know what to translate/update and what to not change.

## Step 3: Translate main content

Follow [Translation guidance]({{ "/about/translating/guides/translation-guidance/" | relative_url }}) to translate the main content of the page.
