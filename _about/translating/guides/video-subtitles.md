---
title: "Translating Video Subtitles and Descriptions"
nav_title: Video Subtitles/Descriptions
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/video-subtitles.md'
permalink: /about/translating/guides/video-subtitles/
ref: /about/translating/guides/video-subtitles/
lang: en
last_updated: 2023-12-06

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 6 December 2023.</p>
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

## Step 1: Find the related video identifier {#find-video-id}

If you want to create new subtitles/translated descriptions for a video, you have probably seen the video in a W3C WAI resource.

You now need to find the video identifier. 

Look for the embedded video player **in the code of the English version of the page**. It looks similar to this:

{::nomarkdown}
{% include box.html type="start" title='Video player example' %}
{:/}

```liquid
{% raw %}{% include video-player-data.html
   yt-id="20SHvU2PKsM"
   video-id="keyboard"
%}{% endraw %}
```

{::nomarkdown}
{% include box.html type="end" %}
{:/}

**The value of `video-id` is the video identifier you need.**


## Step 2: Edit video-metadata.yml {#video-metadata}

WAI videos captions, subtitles and descriptions metadata are stored in "video-metadata.yml" in ["wai-website-data" repository {% include_cached external.html %}](https://github.com/w3c/wai-website-data/)

{::nomarkdown}
{% include box.html type="start" title="Video-metadata.yml example" %}
{:/}
{% include excol.html type="start" id="optional-id" %}

Show example

{% include excol.html type="middle" %}

```yaml
- id: keyboard
  name:
    en: "Web Accessibility Perspectives: Keyboard Compatibility"
    fr: "L'accessibilité Web illustrée : Compatibilité avec le clavier"
  main-page: /perspective-videos/keyboard/
  path: perspective-videos
  lang-folder: true
  captions:
    - en
  captions-ad:
    - en
  subtitles:
    - fr
    - zh-hans
  subtitles-ad:
    - fr
    - zh-hans
  descriptions-ad:
    - en
    - fr
    - zh-hans
```
{% include excol.html type="end" %}
{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
<ol>
  <li>
{:/}
Navigate to the [wai-website-data repository {% include_cached external.html %}](https://github.com/w3c/wai-website-data/).
{::nomarkdown}
    </li>
    <li>
{:/}
  In "video-metadata.yml", look for the `id` that matches the `video-id` found in previous step.
{::nomarkdown}
    </li>
    <li>
{:/}
Update the following video attributes
  
- `name`: name of the video.\
Add your translated version to the list.
  
- `subtitles`: available subtitles languages.\
Add your language subtag to the list.
  
- `subtitles-ad`: available subtitles languages for the audio-described version of the video.\
Add your language subtag to the list.
  
- `descriptions-ad`: available descriptions languages for the audio-described version of the video.\
Add your language subtag to the list.

{::nomarkdown}
  </li>
  <li>
{:/}

Do not change the following attributes
  
- `main-page`
- `path`
- `lang-folder`
- `captions`
- `captions-ad`

{::nomarkdown}
  </li>
</ol>
{:/}

## Step 3: Create the subtitles/descriptions file(s) {#create-vtt}

Captions, subtitles and descriptions are stored in WebVTT (`.vtt`) files. VTT files are located in "wai-videos" folder, in ["wai-website-data" repository {% include_cached external.html %}](https://github.com/w3c/wai-website-data/).

{::nomarkdown}
<ol>
  <li>
{:/}
To find the path to the VTT files to translate, look at `path` and `lang-folder` attributes in ["video-metadata.yml"](#video-metadata).

- `path`: path to VTT files, from "wai-videos" folder.
- `lang-folder` (not always present): when set to `true`, means VTT files for a language are located in a subfolder named after the language shortcode.

{::nomarkdown}
{% include box.html type="start" title="Example" %}
{:/}
In this example, English VTT files are located into "/wai-folders/perspective-videos/en/"

```yaml
- id: keyboard
  (...)
  path: perspective-videos
  lang-folder: true
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
</li>
<li>
{:/}
Duplicate the English VTT file, with language shortcode added to the middle of the filename.

{::nomarkdown}
{% include box.html type="start" title="Example for a translation into Arabic" %}
{:/}

- Original English files:
  - Captions: `keyboard.en.vtt`
  - Captions (audio-described version): `keyboard_ad.en.vtt`
  - Description (audio-described version): `keyboard_ad_desc.en.vtt`

- New files translated into Arabic:
  - Subtitles: `keyboard.ar.vtt`
  - Subtitles (audio-described version): `keyboard_ad.ar.vtt`
  - Description (audio-described version): `keyboard_ad_desc.ar.vtt`

{::nomarkdown}
{% include box.html type="end" %}
{:/}

If files are stored into lang subfolders, create a subfolder for your language.
{::nomarkdown}
  </li>
</ol>
{:/}

## Step 3: Translate the VTT file(s) {#translate-vtt}

1. Translate all text segments
2. Keep the first line (`WEBVTT`)
3. Do not edit time-intervals

{::nomarkdown}
{% include box.html type="start" title='VTT file example' %}
{:/}

```text
WEBVTT

00:00:01.000 --> 00:00:04.340
Tools for evaluating web accessibility.

00:00:04.640 --> 00:00:10.880
There are software programs and online services
to help you identify accessibility barriers.

00:00:11.340 --> 00:00:14.380
They can save you lots of time and effort
on evauation,

00:00:14.540 --> 00:00:18.120
and can help you avoid creating
new accessibility barriers.
```
{::nomarkdown}
{% include box.html type="end" %}
{:/}

## Step 4: Commit your changes {#commit-changes}

Include the updated "video-metadata.yml" and the new translated VTT files.