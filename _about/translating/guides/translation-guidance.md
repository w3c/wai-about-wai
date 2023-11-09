---
title: "Translation Guidance"
nav_title: Translation Guidance
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/translation-guidance.md'
permalink: /about/translating/guides/translation-guidance/
ref: /about/translating/guides/translation-guidance/
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

## General guidance

- Do not change or adapt or add to the meaning of the English version in your translation.
- If you have suggestions for changes to the English version, submit them via GitHub or e-mail using the links in the “Help improve this page” box near the bottom of the page.

## Markdown/Code

Please leave the code, HTML, and markdown as is without changing it.

Make sure to:

{::nomarkdown}
<ul>
<li>
{:/}

Translate titles in the markdown, such as "Summary" in:

{::nomarkdown}
{% include box.html type="start" %}
{:/}
```liquid
{% raw %}{% include box.html type="start" title="Summary" class="" %}{% endraw %}
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
</li>
<li>
{:/}

Translate image alternative text, such as “mouse crossed out” in:

{::nomarkdown}
{% include box.html type="start" %}
{:/}

- in Markdown: `![mouse crossed out](https://www.w3.org/WAI/intro/no-mouse.png)`
- in HTML: `<img src="https://www.w3.org/WAI/intro/no-mouse.png" alt="mouse crossed out" />`

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
</li>
<li>
{:/}

Make sure that the quote marks stay as is, and are not converted to "smart quotes" by word processing software.

{::nomarkdown}
</li>
</ul>
{:/}

### Links

Most links are formatted with single or double brackets and parentheses; for example:

{::nomarkdown}
{% include box.html type="start" %}
{:/}
```markdown
[Text that is linked]({%raw%}/{%endraw%}path/to/filename/)
[[Title of WAI Page]]({%raw%}/{%endraw%}path/to/filename/)
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

Just so you know:
- When we want the system to use the title of the linked-to page as link text, we use `[[double brackets]]`. 
  - That way, when the linked-to page is translated, the system will use the translated page's title.
  - If the linked-to page is not translated, the system will use your translated text between the brackets, and add `(in English)` in the translated language at the end of the link.
- When we want to use custom link text, we use `[single brackets]`.

Make sure to:
- Keep brackets and parentheses together, with no space between the closing `]` and the opening `(`.
- Keep double `[[` or single brackets `[` as they are.
- Translate the text in the links, including document titles.
- Do not manually add `(in English)`, even for external links.

## Text Editor

The markdown files are very sensitive to indentation, commas, quotes, and special characters. 

We recommend that you use a markdown editor or a simple text editor (including GitHub interface) — and not a document editor like Microsoft Word that often changes quotes and indentation.

## Glossaries

- Read the [General Translation Glossary {% include_cached external.html %}](https://github.com/w3c/translation-glossaries/blob/main/general.md).
- See if there is a [glossary for your language {% include_cached external.html %}](https://github.com/w3c/translation-glossaries#readme).

## Resource-Specific Information

Some resources have specific Translations notes. 

{::nomarkdown}
<ul>
<li>
{:/}

At the top of the resource file (in the ["front matter" metadata](/about/translating/guides/new-translation/#frontmatter)), see if there is a comment like this one:

{::nomarkdown}
{% include box.html type="start" %}
{:/}
```
# Read Translations Notes at https://github.com/w3c/path-to-repository#readme
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

In that case, follow the link and read the specific guidance.

{::nomarkdown}
</li>
<li>
{:/}

If you wish to translate the [WCAG-EM Report Tool](https://www.w3.org/WAI/eval/report-tool/), please read [this specific guidance {% include_cached external.html %}](https://github.com/w3c/wai-wcag-em-report-tool/wiki/How-to-add-a-language), as different steps have to be followed.

{::nomarkdown}
</li>
</ul>
{:/}

## We are here to help

If you have any questions about the translation, please report them in the related GitHub issue so that WAI team and other volunteers can help. Alternatively, send an e-mail to the publicly-archived [public-wai-translations@w3.org](mailto:public-wai-translations@w3.org) mailing-list.

We are happy to help you decide on the best translated wording by sharing the considerations and nuances that went into choosing the wording for the English page.