---
title: "Getting started with translating WAI Resources"
nav_title: Getting started
github:
  repository: w3c/wai-about-wai
  path: '_about/getting-started-translating.md'
permalink: /about/translating/getting-started/
ref: /about/translating/getting-started/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a first draft documentation to guide volunteer translators. **It welcomes feedbacks**, even if steps 4 & 5 need updates and step-by-step instructions (to be added to Using Github guide).

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 14 September 2023.</p>
  <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>, Rémi Bétin.</p>

translations_priorities:
- url: "/videos/standards-and-benefits/"
- url: "/fundamentals/accessibility-intro/"
- url: "/perspective-videos/"
  pages:
    - url: "/perspective-videos/keyboard/"
    - url: "/perspective-videos/contrast/"
    - url: "/perspective-videos/layout/"
    - url: "/perspective-videos/speech/"
    - url: "/perspective-videos/controls/"
    - url: "/perspective-videos/captions/"
    - url: "/perspective-videos/customizable/"
    - url: "/perspective-videos/voice/"
    - url: "/perspective-videos/understandable/"
    - url: "/perspective-videos/notifications/"
- url: "/tips/writing/"
- url: "/tips/designing/"
- url: "/tips/developing/"
- url: "/tutorials/images/decision-tree/"
- url: "/fundamentals/accessibility-principles/"
- url: "/about/participating/"  #For testing only
- url: "/about/sponsoring/"  #For testing only
- url: "/about/contacting/"  #For testing only

---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

This page provides step-by-step guidance on translating WAI resources.

For more general information, see [Translating WAI Resources]({{ "/about/translating/" | relative_url }})

To get announcements related to WAI translations, subscribe to the WAI Translations mailing list by sending e-mail to <a href="mailto:public-wai-translations-request@w3.org?subject=subscribe">public-wai-translations-request@w3.org with subject: &ldquo;subscribe&rdquo;</a>

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::options toc_levels="2,3" /}
{::nomarkdown}
{% include_cached toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}

## GitHub

We encourage you to use GitHub, especially if you intend to become a regular translator. 

Discussions, collaboration with reviewers and progress tracking are more easily managed in GitHub.

- If you do not already have a GitHub Account, [sign up {% include_cached external.html %}](https://github.com/signup) for an account;
- If you are new to GitHub, we recommend that you follow this interactive free course:\
[Introduction to GitHub {% include_cached external.html %}](https://github.com/skills/introduction-to-github).
- Then, for more specific guidance during the translation process, you can deep dive with our [Using Github]({{ "/about/translating/guides/using-github/" | relative_url }}) guide.


{::nomarkdown}
{% include box.html type="start" title="Important note" class="simple" %}
{:/}

We hope you find benefits in using GitHub to contribute. That said, we do not expect translators to be or become GitHub experts. 

If you are unsure how to proceed and need guidance; or if you are not comfortable with GitHub at all: please send e-mail to [group-wai-translations@w3.org](mailto:group-wai-translations@w3.org) [^1].

We will be happy to guide you through GitHub or look for alternatives more suitable for you.

{::nomarkdown}
{% include box.html type="end" %}
{:/}


## Translating resources {#translating}

{% include excol.html type="all" %}

{% include excol.html type="start" %}

### Step 1: Find a resource to translate

{% include excol.html type="middle" %}

#### Have a look at our priorities

For suggestions on which to translate first, see [Priorities for Translations](#priorities).

#### Or pick a resource according to your preference

You are welcome to translate any current WAI resource that you think would be useful in your language.

The easiest way to find a resource to translate is to head over to the dedicated translation sitemap for your language.

Translation sitemaps display the structure of WAI website, and indicate for each page:
- If a translation has been published for this language + its current status ({% include_cached icon.html name="check-circle" %} Up-to-date / {% include_cached icon.html name="warning" %} Needs update).
- If a page has no translation available in this language, and therefore welcomes a volunteer translation.

##### List of current translations sitemaps:

- [French translations sitemap]({{ "/about/translating/sitemaps/sitemap-fr/" | relative_url }})

{::nomarkdown}
{% include box.html type="start" title="Note" class="simple" %}
{:/}

If there is no sitemap for your language, it generally means no resources have been translated in this language.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 2: Inform us of your intent to translate a resource

{% include excol.html type="middle" %}

{::nomarkdown}
{% include box.html type="start" title="New volunteer?" class="highlighted" %}
{:/}
 Thank you so much for your interest in translating W3C WAI Resources! 

To begin your journey, send an email to [group-wai-translations@w3.org](group-wai-translations@w3.org) (not publicly archived&nbsp;[^1]) to express your interest in joining the WAI translator volunteers community.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

When you have found a resource to translate, you must indicate your interest, and wait for a reply from WAI team. We'll check that the file isn't currently being translated by someone else, and that it isn't about to be updated. 

Please wait for reply from WAI team before starting a translation.

#### Recommended / quickest way {#translation-issue}

From the translations sitemap in your language, click on the `"Volunteer to translate this page"` link, displayed next to the resource you intend to translate.
  - It will automatically pre-fill a GitHub issue with some useful information.

#### Alternatives:
  - You can directly create an Issue in our GitHub translations repository. See [Creating a GitHub issue]()
  - If you are not comfortable with GitHub, send e-mail to the WAI translations list using [this e-mail template](mailto:public-wai-translations@w3.org?subject=%5Blang%5D%20Intent%20to%20Translate%3A%20%5Btitle%5D&body=I%20would%20like%20to%20translate%20into%20%5Blanguage%5D%20the%20following%20resource%3A%0A%5BEnglish%20title%5D%0A%5BURI%5D%0A%0AI%20have%20read%20the%20information%20on%20Translating%20WAI%20Documents%20at%20https%3A%2F%2Fwww.w3.org%2FWAI%2Fabout%2Ftranslating%2F%0A%0AI%20will%20wait%20for%20confirmation%20that%20the%20resource%20is%20ready%20for%20translation.). 

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 3: Start translating

{% include excol.html type="middle" %}

#### Initial setup

- Log in to your existing GitHub account, or create one. [See GitHub section](#github)
- Get to the repository of the resource you will translate. 
  - Near the bottom of each page on the WAI website, there is a "Help improve this page" box. The middle button is "Fork & Edit in GitHub". That gets you to the repository. 
  - If you have followed the [recommended way](#translation-issue) to declare your intent, you can directly see that info in the GitHub issue.
- You can directly work from there. When committing changes, a [forked repository {% include_cached external.html %}](https://docs.github.com/get-started/quickstart/fork-a-repo) will automatically be created. Alternatively, you can fork the repository first.

#### Translate the resource

- Refer to [Creating a Translation]({{ "/about/translating/guides/new-translation/" | relative_url }}) guide
- If the page you are translating has videos, also refer to [Creating Video Subtitles/Descriptions]({{ "/about/translating/guides/video-subtitles/" | relative_url }})
- Read the [Translating Guidance]({{ "/about/translating/guides/translation-guidance/" | relative_url }}).

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 4: Preview and check your translation

{% include excol.html type="middle" %}

We have enabled a preview with Netlify so you can check your file and make edits.

- Open a [draft Pull Request {% include_cached external.html %}](https://docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) in the GitHub repository of the resource, with `[IN-PROGRESS]` at the beginning of the title.

- After you submit the pull request, a preview will be generated. At first it will say "Some checks haven't completed yet.".
  - Check everything listed in [Reviewer Guidance]({{ "/about/translating/guides/review-translation/" | relative_url }}#initial-things-to-check)
  - Eventually, commit some fixes.
  - At this point, if you encounter some technical problems, ask for help from WAI team.

- When your auto-review is done, go to the next step.

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 5: Ask for reviews

{% include excol.html type="middle" %}

Translations are reviewed before they are published.

- Change the beginning of your PR title to `[READY FOR REVIEW]`
- Communicate your PR is ready for review in the GitHub issue created at step 2.
- Discussions take place directly in the GitHub Pull Request.

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 6: Wait for publication

{% include excol.html type="middle" %}

WAI team is responsible for publishing translations.

{% include excol.html type="end" %}


## Priorities for Translating WAI Resources {#priorities}

{% include ednote.html note="Pages listed below are examples + translated pages need to be deleted before final publication" %}

{% assign alldocs=site.documents | concat: site.pages %}
{%- if page.translations_priorities -%}
  <ul>
  {%- for prio in page.translations_priorities -%}
    {% assign original=alldocs | where_exp:"item", "item.lang == 'en' or item.lang == nil" | where_exp:"item", "item.ref == prio.url or item.url == prio.url" | first %}
    {% assign allt=alldocs | where_exp:"item", "item.lang != 'en' and item.lang != nil" | where_exp:"item", "item.ref == prio.url" %}
    {%- if original -%}
      <li>
      {%- if original.title -%}
        <a href="{{ original.url | relative_url }}">{{ original.title }}</a>
      {%- endif -%}
      {%- if allt.size > 0 -%}
        <br />
        Completed translations:
        {%- for t in allt -%}
          {%- capture url -%}{{ t.url | relative_url }}{%- endcapture -%}
          {% include resource-link.html noicon="true" label=t.lang href=url %}
        {%- endfor -%}
      {%- endif -%}
      </li>
    {%- endif -%}
  {%- endfor -%}
  </ul>
{%- endif -%}

## Reviewing Translations  {#reviewing}

Translations are reviewed by volunteers and WAI team before they are published.

{% include excol.html type="all" %}

{% include excol.html type="start" %}

### Step 1: Find translations ready for review

{% include excol.html type="middle" %}

{::nomarkdown}
{% include box.html type="start" title="New volunteer?" class="highlighted" %}
{:/}
Thank you so much for your interest in reviewing W3C WAI Resources!

First and foremost, send an email to [group-wai-translations@w3.org](group-wai-translations@w3.org) (not publicly archived&nbsp;[^1]) to express your interest in joining the WAI translator volunteers community.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

1. Explore the [WAI Translations GitHub project {% include_cached external.html %}](https://github.com/orgs/w3c/projects/46/views/2)
  - Look into the "Ready for review" column to find translations ready for review.
  - You can filter the view by clicking on your language in the "Language" column.
  - If you have trouble using this _board_ view, you can look at the [equivalent table view {% include_cached external.html %}](https://github.com/orgs/w3c/projects/46/views/3)

2. Communicate you are volunteering to review, by leaving a comment in the corresponding issue.

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 2: Review the translation

{% include excol.html type="middle" %}

Follow [Reviewing translations]({{ "/about/translating/guides/review-translation/" | relative_url }}) step-by-step guide.

{% include excol.html type="end" %}

[^1]: Emails sent to `group-wai-translations@w3.org` are not publicly visible.