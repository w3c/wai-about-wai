---
title: "Reviewing a Translation"
nav_title: Reviewing a translation
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/review-translation.md'
permalink: /about/translating/guides/review-translation/
ref: /about/translating/guides/review-translation/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a first draft documentation to guide volunteer translators. **It welcomes feedbacks.**
last_updated: 2023-09-13
translators:
  - name: Translator 1
  - name: Translator 2
contributors:
  - name: Contributor 1
  - name: Contributor 2
description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 14 September 2023.</p>
  <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>, Rémi Bétin.</p>
---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

Here are some guidance to review a translation.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::options toc_levels="2,3" /}
{::nomarkdown}
{% include toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include toc.html type="end" %}
{:/}

## How to add comments to a draft translation in GitHub

A <6 minute video:
* on [YouTube {% include_cached external.html %}](https://www.youtube.com/watch?v=oP0PZtHlhiU)
* on [Zoom (unedited captions) {% include_cached external.html %}](https://mit.zoom.us/rec/share/ED-utGMCqDnP3fmECnhd5mFYTekeTa4WOEohnxEd8MFaZ0GVZszNtdN52sLHm8Me.ksOapg8FA6jvXJp1)

## Initial things to check

{::nomarkdown}
<ol>
  <li>
{:/}

The language codes are correct, per [frontmatter](/about/translating/guides/new-translation/#specific-inline-instructions-for-front-matter).

{::nomarkdown}
  </li>
  <li>
{:/}

The information in the "About this translation" box is correct.

{::nomarkdown}
{% include box.html type="start" title='There should be 5 lines, for example:' %}
{:/}
 <section class="doc-note-box doc-note-translation">
   <h2 class="visuallyhidden">{% include t.html t="About this Translation" %}</h2>
   <p>{% assign replacepattern = page.url | relative_url | prepend: "$1|"  %}{% include t.html t='This volunteer translation might not accurately reflect the intentions of the <a href="$1">English original</a>.' replace=replacepattern %}</p>
   <p>{% include_cached icon.html name="check-circle" %} {% include t.html t='Translation up-to-date with the English version.' %}
     <br>{% include t.html t='Translation updated:' %} <span dir="auto">{{page.last_updated | date: "%Y-%m-%d"}}</span>. {% include t.html t='English updated:' %} <span dir="auto">{{page.last_updated | date: "%Y-%m-%d"}}</span>.
    </p>
   <p>
     {%- capture translatorslabel %}<strong>{% include t.html t='Translators:' %}</strong>{%- endcapture %}
     {% include peoplelist.html label=translatorslabel people=page.translators %}
     {%- capture contributorslabel %}{% include t.html t='Contributors:' %}{%- endcapture %}
     {% include peoplelist.html label=contributorslabel people=page.contributors %}
     {%- assign replacepattern = "/about/translating/" | relative_url | prepend: "$1|" -%}
     <br>{% include t.html t='WAI thanks translators, and welcomes other <a href="$1">translations</a>.' replace=replacepattern %}</p>
 </section>
 {::nomarkdown}
 {% include box.html type="end" %}
 {:/}

- If translator or contributor names are missing, it's because they are still commented out.\
Delete the hashmark and space (`# `) before the lines.
- Check the dates: one is the date of the translation; the other should usually match the date in the footer.

{::nomarkdown}
  </li>
  <li>
{:/}

In the footer, the dates are the same in the English version and the translated version.

{::nomarkdown}
  </li>
  <li>
{:/}

There is no code showing in the rendered page.

{::nomarkdown}
  </li>
  <li>
{:/}

All of the text that should be translated, is actually translated.

{::nomarkdown}
  </li>
  <li>
{:/}

The links work.

{::nomarkdown}
  </li>
  <li>
{:/}

Check the raw file to see if all alternative texts and other not-visible content are translated.

{::nomarkdown}
  </li>
  <li>
{:/}

In the "Help improve this page" box near the bottom, the "Fork and Edit" button works.

If not, the fix is probably adding "content/" to the path in the front matter.

For example:

{::nomarkdown}
{% include box.html type="start" %}
{:/}
```yaml
  path: content/index.es.md
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
  </li>
  <li>
{:/}

For any videos on the page, the `[CC]` defaults to the translated language.

If not, some [video subtitles steps]({{ "/about/translating/guides/video-subtitles/" | relative_url }}) are probably missing.

{::nomarkdown}
  </li>
</ol>
{:/}

## For people who know the translated language

The most important thing for review is helping accurately convey the meaning from the English version in the translated language. For that, you will need to read the English version and compare it to the translation. Often is best to have them open in side-by-side windows.

A technique for proof-reading is to listen to the translation being read aloud, for example with a screen reader or text-to-speech in the operating system.

**Specific wording:**
- Consider different dialects. Where possible, the translation should use words and phrases that will be best understood across different areas.
- The translator and reviewer(s) might want to work together to consider different options for some wording. If you have any questions about the wording, please e-mail them to [public-wai-translations@w3.org](mailto:public-wai-translations@w3.org).\
We are happy to help you decide on the best translated wording by sharing the considerations and nuances that went into choosing the wording for the English page.
- When you decide on translation of unclear words and phrases that will likely be in other resources, feel free to add them to the [Glossary for your language]({{ "/about/translating/glossaries/" | relative_url }}).

## For people who do _not_ know the translated language

You can still help with reviews by looking for things like: 
- English text that is not translated (like alt text)
- Link accuracy,
- Formatting issues,
- and other things listed [at the top of this section](#initial-things-to-check).

You can also help find missing content or potential issues with the specific wording.

**Suggestion: Compare three versions side-by-side:**
- The English original
- The translation for review
- A machine translation of the translation back into English (of course, this will be very inaccurate, yet sometimes it still works to spot issues)