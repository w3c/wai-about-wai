---
# NEW: Comments for new repos start with "NEW". Please delete the NEW comments. Leave the other comments for translators. Also, search for @@s to replace. For multi-page resources and other frontmatter info, see: https://wai-website-theme.netlify.app/writing/frontmatter/

# Translation instructions are after the "#" character in this first section. They are comments that do not show up in the web page. You do not need to translate the instructions after #.
# In this first section, do not translate the words before a colon. For example, do not translate "title:". Do translate the text after "title:".

doc-note-type: draft
title: "[EARLY DRAFT] Accessibility Work at W3C"
# title_html: "Main Title:<br>Other Part" # NEW: only needed if you need <br> or other in title. Otherwise, delete.
# nav_title: "Short Title" # NEW: (I think not used yet, but in place for possible future use.)

lang: en   # Change "en" to the translated-language shortcode from https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry
# last_updated: 2022-02-22   # Put the date of this translation YYYY-MM-DD (with month in the middle)

# translators:    # remove from the beginning of this line and the lines below: "# " (the hash sign and the space)
# - name: "Jan Doe"   # Replace Jan Doe with translator name
# - name: "Jan Doe"   # Replace Jan Doe with name, or delete this line if not multiple translators
# contributors:
# - name: "Jan Doe"   # Replace Jan Doe with contributor name, or delete this line if none
# - name: "Jan Doe"   # Replace Jan Doe with name, or delete this line if not multiple contributors

github:
  repository: w3c/wai-about-wai
  path: _about/new-work.md    # Add the language shortcode to the middle of the filename, for example: content/index.fr.md
permalink: /about/new-work/   # Add the language shortcode to the end, with no slash at end, for example: /link/to/page/fr

# NEW: 3 navigation lines below are only needed for multi-page resources where you have previous and next at the bottom. If so, un-comment them; otherwise delete these lines.
# navigation:
  # previous: /path/to/previous/file/
  # next: /path/to/next/file/
# @@SLH To Do: figure out if need to add lang here, too, and if this replaces "order" from older resources?

ref: /about/new-work/   # Translators, do not change this
# changelog: /@@/changelog/
# acknowledgements: /@@/acknowledgements/  # NEW: delete if don"t have a separate acknowledgements page. And delete it in the footer below.
# license: creative-commons   # NEW: delete if not creative-commons

# description:  # NEW: add a 150ish-character-description for social media   # translate the description
# image: /content-images/wai-@@repo/social.png  # NEW: image for social media
feedbackmail: wai@w3.org  # NEW: delete this line if it’s an EOWG resource (the default is wai-eo-editors@w3.org)

# NEW: Footer below has several options, and not all will be relevant for specific pages. (Ask Shawn if questions.)

# In the footer below:
# Do not translate or change CHANGELOG or ACKNOWLEDGEMENTS.
# Translate the other words below, including "Date:" and "Editor:"
# Translate the Working Group name. Leave the Working Group acronym in English.
# Do not change the dates in the footer below.
footer: >
   <p><strong>Date:</strong> EARLY DRAFT Updated @@ March 2022. First published March 2022.<!-- CHANGELOG.--></p>
   <p><strong>Editor:</strong> <a href="https://www.w3.org/People/Shawn">Shawn Lawton Henry</a> Contributors: @@name, @@name, and <a href="https://www.w3.org/groups/wg/eowg/participants">participants of the EOWG</a>.</p>
   <p>Developed with the Accessibility Education and Outreach Working Group (<a href="http://www.w3.org/WAI/EO/">EOWG</a>).</p>

---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

This page highlights some of the work you can contribute to at the Web Accessibility Iniaitive (WAI) W3C to make the Web more accessible to people with disabilities. _{draft wording}_

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

This page highlights some of the current accessibility work in the Web Accessibility Iniaitive (WAI) and other groups in the W3C. It includes links to the group responsible for the work, so you can learn more about contributing to specific projects.

Get related information:
* To learn more about contributing to this work generally, see [[Participating in WAI]](/about/participating/).
* To get updates on this and other accessibility work, see [[Get WAI News]](/news/subscribe/).
* To learn about existing resources, see [[WAI Resources]](/resources/).

## Web Accessibility Guidelines and other Standards

* **Web Content Accessibility Guidelines (WCAG) 2.2** is in progress. The current plan is to publish the final version by June 2022. Note that these links have information that will change: [What's New in WCAG 2.2 Working Draft](/standards-guidelines/wcag/new-in-22/), [WCAG 2.2 Editor's Draft ](https://w3c.github.io/wcag/guidelines/22/).

* **W3C Accessibility Guidelines (WCAG) 3.0** an early draft of a few aspects of a potential new standard. It is years away from being finalized. [[WCAG 3 Introduction]](/standards-guidelines/wcag/wcag3-intro/), [About Accessibility Guidelesines Working Group](https://www.w3.org/groups/wg/ag)

* **Personalization** (renaming in progress, maybe _Personalized Adaptation_) involves tailoring the user experience to meet the needs and preferences of the individual user. [[Personalization Overview]](/personalization/), [Personalization Task Force](https://www.w3.org/groups/tf/personalization-tf)

* **Spoken Pronunciation** technical standards are being developed to enable screen readers and voice assistants to pronounce words correctly. [[Pronunciation Overview]](/pronunciation/), [Spoken Pronunciation Task Force](https://www.w3.org/groups/tf/pronunciation-tf)

* **ARIA**

## Guidance for Cognitive, Low Vision, Mobile

* **Cognitive** &mdash; There are several documents being updated to better address the needs of people with cognitive and learning disabilities. See [[Cognitive Accessibility at W3C]](/cognitive/). [About COGA TF](https://www.w3.org/groups/tf/cognitive-a11y-tf)

* **Low Vision**  &mdash; We are writing guidance that goes beyong the minimums required by WCAG. It is called "supplementla guidance". Current topics cover proximity, printing, and alternative themes such as high contrast and dark mode. [About Low Vision TF](https://www.w3.org/groups/tf/low-vision-a11y-tf)

* [[Mobile Accessibility at W3C]](/standards-guidelines/mobile/)

## Accessibility User Requirements (AUR) and Emerging Technologies

Documenting the user needs of people with disabilities helps develop standards to meet those needs. It also helps designers, developers, and others better understand and meet user needs in order to support accessibility.

* **Natural Language Interface Accessibility User Requirements ("NAUR")** is a Working Draft. A natural language interface is a user interface in which the user and the system communicate via a natural (human) language. The user provides input as sentences via speech or other input, and the system generates responses as sentences delivered by speech, text, or another modality. [About  NAUR](https://www.w3.org/blog/2021/10/natural-language-interface-accessibility-user-requirements-call-for-review/), [NAUR Draft](https://www.w3.org/TR/naur), [About the APA Working Group](https://www.w3.org/WAI/APA/)

* **XR Accessibility User Requirements (XAUR)** is a Working Draft. XAUR describes the needs of people with disabilities in virtual or immersive environments (XR). It includes requirements for XR to be accessible. XAUR is for designers and developers who are involved in creating XR experiences. [XAUR Draft](https://www.w3.org/TR/xaur/), [About the APA Working Group](https://www.w3.org/WAI/APA/)

* **Synchronization Accessibility User Requirements (SAUR)** is a Working Draft. Synchronization of multimedia content, especially audio and video, is essential for accessible web-based communication and cooperation. To be understandable, media needs to be synchronized to very specific limits. [SAUR Draft](https://www.w3.org/TR/saur/)

* **How People with Disabilities Use the Web** helps you understand user needs broadly. We are updating this resrouce and creating videos to go along with it. [[How People with Disabilities Use the Web]](/people-use-web/), [About EOWG](/EO/)

* **Cognitive accessibility user requirements** &mdash; Updating documentation on the user needs of people with cognitive and learning disabilities is happening through the [Cognitive and Learning Disabilities Accessibility Task Force (COGA)](https://www.w3.org/WAI/GL/task-forces/coga/#about).

## Teaching Accessibility

**Curricula on Web Accessibility** is a framework to build your own courses. It currently includes modules for foundations for everyone, for developers, and for designers. We are currently working on modules for content authors. [[Existing Curricula]](/curricula/), [Content Authors rough draft outline](https://github.com/w3c/wai-curricula/wiki/content-author-modules-outline), [About EOWG](/EO/)

## Testing Accessibility

**WCAG 2 Test Rules** (also known as ACT Rules) describe how to test conformance to WCAG success criteria. They are primarily for developers of evaluation tools and test methodologies. [[About WCAG 2 Test Rules]](/standards-guidelines/act/rules/about/), [Accessibility Conformance Testing (ACT) Task Force](https://www.w3.org/groups/tf/wcag-act)

<br><br><hr>

@@ END DRAFT - below are internal notes @@ ==================================

**current projects not listed &mdash; why (see [Scope in the Requirement Analysis](https://github.com/w3c/wai-about-wai/wiki/What-WAI-is-Working-On-Requirements-Analysis#scope))**
* Eval Tools list redesign (EOWG) &mdash; we're not seeking additional contributions right now, and it's not a new things
* Course list (EOWG) &mdash; we're not seeking additional contributions right now
* Authoring Tools list (EOWG) &mdash; we're not seeking additional contributions right now
* Easy Checks – A First Review of Web Accessibility (EOWG) &mdash; we're not going to get to it for a few months and we have out hands full with other things. (drafted: We hope to do a significant update of this in late 2022. We welcome contributions from user interface designers and coders.)
* Accessibility of Remote Meetings &mdash; we're not seeking additional contributions right now
* @@...

**for AUR page -- also:**

* **Media Accessibility User Requirements (MAUR)** is a published Working Group Note. This document presents the accessibility requirements users with disabilities have with respect to audio and video on the web.  [About MAUR](https://www.w3.org/blog/2015/12/media-accessibility-user-requirements-is-a-w3c-note/), [MAUR Note](https://www.w3.org/TR/media-accessibility-reqs/)

* **RTC Accessibility User Requirements (RAUR)** is a published Working Group Note. Real-time communication (RTC) provides real-time peer to peer audio, video, and data exchange directly between supported user agents. This enables instantaneous applications for video and audio calls, text chat, file exchange, screen sharing, and gaming. [RAUR Note](https://www.w3.org/TR/raur/)

**Link markdown template in markdown**:
* [[Exact Title of Page on WAI website]](/permalink/to/page/)
* [WAI website but not exact title](/permalink/to/page/)
* [link off WAI website, including W3C pages](https://example.com)
