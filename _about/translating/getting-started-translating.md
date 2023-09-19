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

## What can I do to help?

There are several opportunities to contribute to WAI Resources translation efforts:

- [Translating new pages](#translating-resources)
- <mark>TO DO</mark> Updating existing translations
- [Reviewing translations](#reviewing-translations)

## GitHub

We encourage you to use GitHub, especially if you intend to become a regular translator. 

Discussions, collaboration with reviewers and progress tracking are more easily managed in GitHub.

- If you do not already have a GitHub Account, [sign up {% include_cached external.html %}](https://github.com/signup) for an account;
- If you are new to GitHub, we recommend that you follow this interactive free course:\
[Introduction to GitHub {% include_cached external.html %}](https://github.com/skills/introduction-to-github).
- Then, for more specific guidance during the translation process, you can deep dive with our [Using Github]({{ "/about/translating/guides/using-github/" | relative_url }}) guide.

If you are not comfortable with GitHub, tell us by email and we will send you a zipped package containing a subset of the files.

{::nomarkdown}
{% include box.html type="start" title="Important note" class="simple" %}
{:/}

We hope you find benefits in using GitHub to contribute. That said, we do not expect translators to be or become GitHub experts. 

If you are unsure how to proceed and need guidance, we are happy to help.\
Please send e-mail to [public-wai-translations@w3.org](mailto:public-wai-translations@w3.org) (publicly archived).

{::nomarkdown}
{% include box.html type="end" %}
{:/}


## Translating resources

{% include excol.html type="all" %}

{% include excol.html type="start" %}

### Step 1: Find a resource to translate

{% include excol.html type="middle" %}

#### Have a look at our priorities

For suggestions on which to translate first, see Priorities for Translations.

<mark>TO DO: Detail this part</mark>

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

To begin your journey, send an email to the publicly-archived [WAI translations list](public-wai-translations@w3.org) <mark>or staff-archived group-wai-translations@w3.org ?</mark> to express your interest in joining the WAI translator volunteers community.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

When you have found a resource to translate, you must indicate your interest, and wait for a reply from WAI staff. We'll check that the file isn't currently being translated by someone else, and that it isn't about to be updated. 

Please wait for reply from WAI staff before starting a translation.

#### Recommended / quickest way

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
Near the bottom of each page on the WAI website, there is a "Help improve this page" box. The middle button is "Fork & Edit in GitHub". That gets you to the repository. 
- Fork the repository.
- Create a new branch.
{:.checkbox}

#### Translate the resource

- Refer to [Creating a Translation]({{ "/about/translating/guides/new-translation/" | relative_url }}) guide
- If the page you are translating has videos, also refer to [Creating Video Subtitles/Descriptions]({{ "/about/translating/guides/video-subtitles/" | relative_url }})
- Read the [Translating Guidance]({{ "/about/translating/guides/translation-guidance/" | relative_url }}).
{:.checkbox}

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 4: Preview and check your translation

{% include excol.html type="middle" %}

- Open a Pull Request in the GitHub repository of the resource, with `[IN-PROGRESS]` at the beginning of the title.

- Check the Netlify preview from GitHub.
  - Check everything listed in [Reviewer Guidance]({{ "/about/translating/guides/review-translation/" | relative_url }}#initial-things-to-check)
  - Eventually, commit some fixes.
  - At this point, if you encounter some technical problems, ask for help from WAI staff.

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

WAI staff is responsible for publishing translations.

{% include excol.html type="end" %}


## Reviewing Translations

Translations are reviewed by volunteers and WAI staff before they are published.

{% include excol.html type="all" %}

{% include excol.html type="start" %}

### Step 1: Find translations ready for review

{% include excol.html type="middle" %}

{::nomarkdown}
{% include box.html type="start" title="New volunteer?" class="highlighted" %}
{:/}
Thank you so much for your interest in reviewing W3C WAI Resources!

First and foremost, send an email to the publicly-archived [WAI translations list](public-wai-translations@w3.org) <mark>or staff-archived group-wai-translations@w3.org ?</mark> to express your interest in joining the WAI translator volunteers community.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

1. Explore the [WAI Translations GitHub project {% include_cached external.html %}](https://github.com/orgs/w3c/projects/46/views/2)
  - Look into the "Ready for review" column to find translations ready for review.
  - You can filter the view by clicking on your language in the "Language" column on your left.
  - If you have trouble using this _board_ view, you can look at the [equivalent table view {% include_cached external.html %}](https://github.com/orgs/w3c/projects/46/views/3)

2. Communicate you are volunteering to review, by leaving a comment in the corresponding issue.

{% include excol.html type="end" %}

{% include excol.html type="start" %}

### Step 2: Review the translation

{% include excol.html type="middle" %}

Follow [Reviewing translations]({{ "/about/translating/guides/review-translation/" | relative_url }}) step-by-step guide.

{% include excol.html type="end" %}
