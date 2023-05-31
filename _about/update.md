---
title: "What We're Working On"
title_html: "What We're Working On<br><span style='font-style: italic; font-size: 0.625em;'> Accessibility Activities and Publications, May 2023</span>"
# nav_title: "Short Title" # NEW: (I think not used yet, but in place for possible future use.)

lang: en

github:
  repository: w3c/wai-about-wai
  path: _about/update.md    # Add the language shortcode to the middle of the filename, for example: content/index.fr.md
permalink: /update/   # Add the language shortcode to the end, with no slash at end, for example: /link/to/page/fr

ref: /update/   # Translators, do not change this
# changelog: /@@/changelog/
# acknowledgements: /@@/acknowledgements/  # NEW: delete if don"t have a separate acknowledgements page. And delete it in the footer below.

description: Find out what we're doing now at the W3C Web Accessibility Initiative (WAI). Get news and learn about upcoming publications and contribution opportunities.   # translate the description
image: /content-images/wai-about-wai/update_social.png
feedbackmail: wai@w3.org

# In the footer below:
# Do not translate or change CHANGELOG or ACKNOWLEDGEMENTS.
# Translate the other words below, including "Date:" and "Editor:"
# Translate the Working Group name. Leave the Working Group acronym in English.
# Do not change the dates in the footer below.
footer: >
   <p><strong>Date:</strong> Updated 28 April 2023. First published March 2022.<!-- CHANGELOG. --></p>
   <p><strong>Editor:</strong> <a href="https://www.w3.org/People/Shawn">Shawn Lawton Henry</a>. Contributors: <a href="https://www.w3.org/groups/wg/eowg/participants">Participants of the EOWG</a> and others working on accessibility at W3C.</p>
   <p>Developed with the Accessibility Education and Outreach Working Group (<a href="http://www.w3.org/WAI/EO/">EOWG</a>).</p>

inline_css: |
  h1 {
    line-height:1;
  }
  
---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

This page highlights some current work at the [W3C](https://www.w3.org/Consortium/) Web Accessibility Initiative ([WAI](https://www.w3.org/WAI/about/)). It points out how you can contribute to making digital technology more accessible to people with disabilities.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
{% include toc.html type="start" title="Page Contents" %}
{:/}

- This will be replaced by an automatically generated TOC when using Markdown formatting.
{:toc}
{::nomarkdown}
{% include toc.html type="end" %}
{:/}

## Introduction

We hope you'll find accessibility work on this page that you are interested in contributing to through W3C WAI. After each item is the acronym of the responsible Working Group (WG) and some Task Forces (TF). Information about the groups is later in this page &mdash; first, let's look at some of the work itself.

## Current Work Highlights

### Updating Core Guidelines and Other Standards

* **Web Content Accessibility Guidelines (WCAG) 2.2 Draft** is available for final review. We plan to publish the completed standard in 2023. Get the latest up-to-date information from [What's New in WCAG 2.2 Working Draft](/standards-guidelines/wcag/new-in-22/).  _[AG WG]_

* **W3C Accessibility Guidelines (WCAG) 3** is an early draft of a few aspects of a potential new standard. We're exploring different approaches. It's years away from being finalized. [[WCAG 3 Introduction]](/standards-guidelines/wcag/wcag3-intro/) _[AG WG]_

* **ARIA 1.3** &mdash; We're working on additional support for Braille and other [new features for ARIA 1.3](https://w3c.github.io/aria/#substantive-changes-targeted-for-the-1-3-release).  _[ARIA WG]_

### Developing New Standards

* **WAI-Adapt** enables users to adapt (or ‘personalize’) how content is presented to meet their needs and preferences. [[WAI-Adapt Overview]](/adapt/) _[APA WG, WAI-Adapt TF]_

* **Spoken Pronunciation** technical standards will enable screen readers and voice assistants to pronounce words correctly. [[Pronunciation Overview]](/pronunciation/) _[APA WG, Spoken Pronunciation TF]_

### Documenting Additional Guidance for People with Cognitive Disabilities, Low Vision, and Mobile Devices

* **Cognitive Accessibility** &mdash; We're updating several documents to better address the needs of people with cognitive and learning disabilities. A current topic is mental health. [[Cognitive Accessibility at W3C]](/cognitive/). _[AG WG, COGA TF]_

<!--
* **Low Vision Accessibility** &mdash; We're writing guidance that goes beyond the minimums required by WCAG. It is called "supplemental guidance". Current topics cover proximity, printing, and alternative themes such as high contrast and dark mode. _[AG WG, Low Vision TF]_
* -->

* **Mobile Accessibility** work includes supporting on-going standards development, including supporting WCAG 3 exploration. [[Mobile Accessibility at W3C]](/standards-guidelines/mobile/) _[AG WG, Mobile TF]_

### Updating Guidance on EPUB Accessibility and on Applying WCAG to ICT

* **EPUB Fixed Layout Accessibility** aims to help publishers address challenges for people with cognitive disabilities and low vision. [EPUB Fixed Layout Accessibility Editor's Draft](https://w3c.github.io/epub-specs/epub33/fxl-a11y/) _[EPUB3 WG, FXL A11y TF]_

* **WCAG2ICT** describes how Web Content Accessibility Guidelines (WCAG) 2 can be applied to non-web information and communications technologies (ICT). We are updating it to include WCAG 2.1 and WCAG 2.2. [[WCAG2ICT Overview]](/standards-guidelines/wcag/non-web-ict/) _[AG WG, WCAG2ICT TF]_

### Defining User Requirements (AUR) and Emerging Technologies

Documenting the user needs of people with disabilities helps develop standards to meet those needs. It also helps designers, developers, and others better understand and meet user needs in order to support accessibility.

* **Natural Language Interface Accessibility User Requirements ("NAUR")** is a Working Draft. A natural language interface is a user interface in which the user and the system communicate via a natural (human) language. The user provides input as sentences via speech or other input, and the system generates responses as sentences delivered by speech, text, or another modality. [About NAUR](https://www.w3.org/blog/2021/10/natural-language-interface-accessibility-user-requirements-call-for-review/), [NAUR Draft](https://www.w3.org/TR/naur)  _[APA WG, Research TF]_

* **How People with Disabilities Use the Web** helps you understand user needs broadly. We're updating this resource and publishing new videos to go along with it. Previous version: [[How People with Disabilities Use the Web]](/people-use-web/) _[EOWG]_

### Testing Accessibility, Evaluation Tools

* **ACT Rules** (Accessibility Conformance Testing (ACT), also known as "WCAG 2 Test Rules") describe ways to test conformance to WCAG success criteria. They are primarily for developers of evaluation tools and test methodologies. We're documenting more. [[About WCAG 2 Test Rules]](/standards-guidelines/act/rules/about/) _[AG WG, ACT TF]_
* ACT Rules implementation reports list which ACT Rules the evaluation tool or methodology addresses. We invite evaluation tool developers to [submit implementation reports](https://act-rules.github.io/pages/implementations/reporting/). _[AG WG, ACT TF]_

## Upcoming Publications

We plan to publish the following documents in "Q2", which is April, May, June. To learn about "Candidate Recommendation" (**CR**), "Proposed Recommendation" (**PR**), and other stages, see [How WAI Develops Accessibility Standards through the W3C Process: **Milestones** and Opportunities to Contribute](https://www.w3.org/WAI/standards-guidelines/w3c-process/).

* [WCAG 2.2](https://www.w3.org/WAI/standards-guidelines/wcag/new-in-22/) to CR and PR
* [ARIA 1.2](https://www.w3.org/TR/wai-aria-1.2/) to Recommendation
* [EPUB Accessibility 1.1](https://www.w3.org/TR/epub-a11y-11/) to Recommendation
* [Digital Publishing WAI-ARIA Module 1.1](https://www.w3.org/TR/dpub-aria-1.1/) and [Digital Publishing Accessibility API Mappings 1.1](https://www.w3.org/TR/dpub-aam-1.1/) to CR
* [WCAG 3 Working Draft](https://www.w3.org/WAI/standards-guidelines/wcag/wcag3-intro/) update

Recent publications and other announcements are listed on the **[News page](/news/)**.

### Get Updated

To get news via e-mail, Twitter, or Atom/RSS feed when these and other accessibility documents are _ready for review_ or _published as final_, see **[[Get WAI News]](/news/subscribe/)**.

## Wait, Wait, There's More

This page _only lists about half_ of the active work on accessibility at W3C. Much of the work happens in the accessibility groups that are introduced in the [W3C Working Groups page](https://www.w3.org/groups/wg/#wg-list).

To learn more about what that the Working Groups are working on right now, see:

* [EOWG Current Work](https://www.w3.org/WAI/EO/wiki/EOWG_Current_Projects) - lists over 20 current and upcoming projects of the Accessibility Education and Outreach (EO) Working Group
* [APA Current Work](https://www.w3.org/WAI/APA/#work) - Accessible Platform Architectures (APA) Working Group
* ARIA - Accessible Rich Internet Applications (ARIA) Working Group
  * [ARIA Working Drafts](https://www.w3.org/groups/wg/aria/publications#WD)
  * [ARIA Authoring Practices Guide (APG)](https://www.w3.org/WAI/ARIA/apg/)
* [AG WG Current Work](https://www.w3.org/WAI/GL/#work) - Accessibility Guidelines (AG) Working Group
  * [COGA Current Work](https://www.w3.org/WAI/GL/task-forces/coga/wiki/Main_Page) - Cognitive and Learning Disabilities Accessibility Task Force (COGA)
  * [LVTF Current Work](https://www.w3.org/WAI/GL/low-vision-a11y-tf/wiki/Main_Page) -  Low Vision Accessibility Task Force (LVTF)
  * [Mobile Current Work](https://www.w3.org/WAI/GL/mobile-a11y-tf/wiki/Main_Page) - Mobile Accessibility Task Force
* [EPUB 3 Working Group document publication status and milestones](https://www.w3.org/publishing/groups/epub-wg/PublStatus)

### Surprise! We already have a resource for that

Did you know the WAI website has: **videos, tips, tutorials, tools** (for generating reports and accessibility statements), **translations** (over 35 languages), **training** (a free online course), and so much more. There are [resources for](https://www.w3.org/WAI/roles/) content authors, designers, developers, evaluators, testers, managers, policy makers, trainers, educators, web users, advocates, and people with disabilities.

**Discover** accessibility resources that _you didn't even know existed_ from the annotated list of **[[WAI Resources]](/resources/).** When you find helpful information, would you **share it with others**.

## How to Get Involved {#participate}

To learn about contributing to W3C WAI accessibility work generally, **see [[Participating in WAI]](/about/participating/)**.

Links to each Working Group's "How to Participate" page are in the [Participating in Working Groups section](/about/participating/#WGs). If you are interested in a Task Force, see participation information for the parent Working Group.

We also offer ideas for [Promoting and Implementing Web Accessibility](https://www.w3.org/WAI/about/participating/#promoting-and-implementing-web-accessibility).

**We look forward to your contributions to making the web more accessible to people with disabilities!**

### Specific Invitations

We are particularly seeking the following contributions:
* EOWG (Accessibilty Education and Outreach Working Group) welcomes contributions on the next iteration of thre following resources.<br> **To comment on current work, please see [EOWG Work for this Week](https://www.w3.org/WAI/EO/wiki/EOWG_Meetings#Work_for_this_week)**.
  * [How People with Disabilities use the Web (draft in progress)](https://deploy-preview-113--wai-people-use-web.netlify.app/people-use-web/) &mdash; complete drafts for review
  * [Easy Checks – A First Review of Web Accessibility (old version)](https://www.w3.org/WAI/test-evaluate/preliminary/) &mdash; in-progress
  * [Digital Accessibility Foundations / Introduction to Web Accessibility](https://www.w3.org/WAI/courses/foundations-course/) free online course &mdash; later in 2023
* Framework for Accessible Specification of Technologies (FAST) Task Force &mdash; FAST advises technical specification creators how to ensure their technology meets the needs of users with disabilities. The newly-forming FAST Task Force will collect user and functional needs, develop guidance to meet those needs in technologies, and work with other groups to develop this guidance for content developers. To participate in the FAST Task Force, see [FAST TF, How to Comment, Contribute, and Participate](https://www.w3.org/WAI/APA/task-forces/fast/#contribute).
* _(more coming, please check back)_

### Who is We

"We" is:

* [W3C](https://www.w3.org/Consortium/) Web Accessibility Initiative ([WAI](https://www.w3.org/WAI/about/))
* W3C WAI Staff: [Kevin White](https://www.w3.org/People#kevin) (Accessibility Development and Operations Lead), [Michael Cooper](https://www.w3.org/People#cooper) (Accessibility Strategy and Technical Lead), [Ruoxi Ran](https://www.w3.org/People#ran) (Accessibility Engineer), [Daniel Montalvo](https://www.w3.org/People#dmontalvo) (Accessibility Harmonization and Testing Specialist), and [Shawn Lawton Henry](https://www.w3.org/People#shawn) (Accessibility Education and Communications Lead)
* Participants of: [AG](https://www.w3.org/groups/wg/ag/participants), [APA](https://www.w3.org/groups/wg/apa/participants), [ARIA](https://www.w3.org/groups/wg/aria/participants), [EPUB](https://www.w3.org/groups/wg/epub/participants), [EO](https://www.w3.org/groups/wg/eowg/participants), and other [W3C groups](https://www.w3.org/groups/)

<section class="default-grid teaser making-web-accessible" aria-labelledby="mwa-title" style="border: 1px solid var(--line-grey);">
  <header class="inner teaser-h">
    <h2 id="mwa-title">
      <span class="title">Making the Web Accessible</span>
    </h2>
    <p class="subtitle">Strategies, standards, and supporting resources to help you make the Web more accessible to people with disabilities.</p>
  </header>
  <div class="inner grid-3">
    <div class="col1 making-web-accessible-box">
      <h3>{%- include_cached icon.html name="hp-book" class="mwa-icon mwa-icon-book" -%} W3C</h3>
      <p>The World Wide Web Consortium (W3C) develops international standards for the Web: HTML, CSS, and many more.</p>
    </div>
    <div class="col2 making-web-accessible-box">
      <h3>{%- include_cached icon.html name="hp-tools" class="mwa-icon" -%} WAI</h3>
      <p>The W3C Web Accessibility Initiative (WAI) develops standards and support materials to help you understand and implement accessibility.</p>
    </div>
    <div class="col3 making-web-accessible-box">
      <h3>{%- include_cached icon.html name="hp-computer" class="mwa-icon mwa-icon-computer" -%} You</h3>
      <p>You can use W3C WAI resources to make your websites, applications, and other digital creations more accessible and usable to everyone.</p>
    </div>
  </div>
</section>

## Updates to this page (changelog)

* 28 April 2023
  * Updated W3C WAI staff roles under [Who is We](https://www.w3.org/WAI/update/#who-is-we): [Kevin White](https://www.w3.org/People#kevin) (Accessibility Development and Operations Lead), [Michael Cooper](https://www.w3.org/People#cooper) (Accessibility Strategy and Technical Lead), [Ruoxi Ran](https://www.w3.org/People#ran) (Accessibility Engineer), [Daniel Montalvo](https://www.w3.org/People#dmontalvo) (Accessibility Harmonization and Testing Specialist), and [Shawn Lawton Henry](https://www.w3.org/People#shawn) (Accessibility Education and Communications Lead)
  * Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
  * Minor update to WCAG 2.2 current work highlights bullet.
  * Deleted Low Vision Task Force work, since it's on hold for a while.
* 31 March 2023 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications) and minor update to WCAG 2.2 current work highlights bullet.
* 28 February 2023 &mdash; No substantive updates.
* 31 January 2023 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 21 December 2022
  * Updated [Testing Accessibility, Evaluation Tools section](https://www.w3.org/WAI/update/#testing-accessibility-evaluation-tools): updated ACT Rules wording and added invitation for evaluation tool vendors to submit implementation reports.
  * Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 1 December 2022 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 9 November 2022 &mdash; We're in the process of updating our <a rel="me" href="https://w3c.social/@wai">Mastodon account w3c.social/@wai</a>.
* 1 November 2022 &mdash; Updated WCAG 2.2 final publication to early 2023.
* 19 October 2022 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 29 September 2022
  * Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
  * Under Current Work Highlights section, deleted "Teaching Accessibility. Curricula on Web Accessibility...", since we published it today
* 12 September 2022
  * Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
  * Updated WCAG 2.2 bullet under Current Work Highlights.
  * Deleted "ARIA 1.2..." from Current Work Highlights because we completed documenting immplementations and are ready to go from CR to PR.
  * [GitHub diff 12 Sept](https://github.com/w3c/wai-about-wai/pull/156/files), [rich text diff 12 Sept](https://github.com/w3c/wai-about-wai/pull/156/files?short_path=a0b7030#diff-a0b70304b865682a8845dbdca495ffbbc8198d8e7fc20066ce55181ffe0d461c)
* 31 August 2022 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 24 August 2022 &mdash; Added [ARIA Authoring Practices Guide (APG)](https://www.w3.org/WAI/ARIA/apg/). Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications). [GitHub diff 24 Aug](https://github.com/w3c/wai-about-wai/pull/154/files), [rich text diff 24 Aug](https://github.com/w3c/wai-about-wai/pull/154/files?short_path=a0b7030#diff-a0b70304b865682a8845dbdca495ffbbc8198d8e7fc20066ce55181ffe0d461c)
* 1 August 2022 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications).
* 12 July 2022 &mdash; added: **WCAG2ICT** describes how Web Content Accessibility Guidelines (WCAG) 2 can be applied to non-web information and communications technologies (ICT). We are updating it to include WCAG 2.1 and WCAG 2.2. [[WCAG2ICT Overview]](/standards-guidelines/wcag/non-web-ict/) _[AG WG, WCAG2ICT TF]_
* 30 June 2022 &mdash; Updated [Upcoming Publications list](https://www.w3.org/WAI/update/#upcoming-publications). Updated 'Personalization' to 'WAI-Adapt'.
* 5 May 2022 &mdash; Just a few little language edits.
* 30 April 2022 &mdash; Minor updates shown in [GitHub diff 30 Apr](https://github.com/w3c/wai-about-wai/pull/141/files), [rich text diff 30 Apr](https://github.com/w3c/wai-about-wai/pull/141/files?short_path=a0b7030#diff-a0b70304b865682a8845dbdca495ffbbc8198d8e7fc20066ce55181ffe0d461c)
