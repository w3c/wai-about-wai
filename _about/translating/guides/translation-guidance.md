---
title: "Translation guidance"
nav_title: Translation guidance
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/translation-guidance.md'
permalink: /about/translating/guides/translation-guidance/
ref: /about/translating/guides/translation-guidance/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a draft documentation to guide volunteer translators. **It welcomes feebacks.**
last_updated: 2023-09-18
description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 18 September 2023.</p>
  <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>, Rémi Bétin.</p>
---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

Here are some general guidance for translators.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

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

- Please leave the code, HTML, and markdown as is without changing it.

Make sure to:
- Translate titles in the markdown such as "Summary" in <br />  {% raw %}`{% include box.html type="start" title="Summary" class="" %}`{% endraw %}
- Translate image alternative text. For example, "mouse crossed out"<br />
  - in Markdown: ```![mouse crossed out](`https://www.w3.org/WAI/intro/no-mouse.png`)```<br />
  - in HTML: ```<img src="`https://www.w3.org/WAI/intro/no-mouse.png`" alt="mouse crossed out" />```

- Make sure that the quote marks stay as is, and are not converted to "smart quotes" by word processing software.

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

Make sure to:
- Keep these together, with no space between the closing `]` and the opening `(`.
- Keep double `[[` or single brackets `[` as they are.
- Translate the text in the links, including document titles.

If the link text is exactly the same as the linked-to page title, then the link should use `[[double brackets]]`.
- When a linked-to page is translated, the system will use the translated page's title.
- If the linked-to page is not translated, the system will add `(in English)` in the translated language at the end of the link.

## Text Editor

The markdown files are very sensitive to indentation, commas, quotes, and special characters. We recommend that you use a markdown editor or a simple text editor — and not a document editor like Microsoft Word that often changes quotes and indentation.

## Glossaries

- Read the [General Translation Glossary]({{ "/about/translating/glossaries/general/" | relative_url }}).
- See if there is a [glossary for your language]({{ "/about/translating/glossaries/" | relative_url }}).

## Resource-Specific Information

Some resources have specific Translations notes. 

{::nomarkdown}
<ul>
<li>
{:/}

At the top of the resource file (in the ["front matter" metadata]({{ "/about/translating/guides/new-translation" | relative_url }}#frontmatter)), see if there is a comment like this one:

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

If you wish to translate the [WCAG-EM Report Tool](https://www.w3.org/WAI/eval/report-tool/), please read the [specific guidance in its repository](https://github.com/w3c/wai-wcag-em-report-tool/wiki/How-to-add-a-language), as different steps have to be followed.

{::nomarkdown}
</li>
</ul>
{:/}

## We are here to help

If you have any questions about the translation, please send e-mail to [mailto:public-wai-translations@w3.org](public-wai-translations@w3.org) (publicly archived). We are happy to help you decide on the best translated wording by sharing the considerations and nuances that went into choosing the wording for the English page.

