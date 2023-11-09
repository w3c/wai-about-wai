---
title: "Translating Video Subtitles and Descriptions"
nav_title: Video Subtitles/Descriptions
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/video-subtitles.md'
permalink: /about/translating/guides/video-subtitles/
ref: /about/translating/guides/video-subtitles/
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

## Step 1: Create the subtitles file

Captions, subtitles and descriptions of WAI videos are stored in WebVTT (`.vtt`) files.

To create the subtitles file, duplicate the English captions file, with language shortcode added to the middle of the filename, as follows:

{::nomarkdown}
{% include box.html type="start" title="Example for a translation into Arabic" %}
{:/}

- Original English file: `VTT_FILE_NAME.vtt`
- New Arabic file: `VTT_FILE_NAME.ar.vtt`

{::nomarkdown}
{% include box.html type="end" %}
{:/}

## Step 2: Translate the file

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

## Step 3: Add the new subtitles to the video player

In the English version of the page, the embedded video player looks similar to this:

{::nomarkdown}
{% include box.html type="start" title='Video player example' %}
{:/}

```liquid
{% raw %}{% include video-player.html
   yt-id="20SHvU2PKsM"
   path="/path/to/vtt/files/"
   captions="VTT_FILE_NAME.vtt|en|default"
   subtitles="VTT_FILE_NAME.es.vtt|es"
%}{% endraw %}
```

{::nomarkdown}
{% include box.html type="end" %}
{:/}

### Actions needed in the translated page

1. Delete `|default` from: `captions="VTT_FILE_NAME.vtt|en|default"` <br />so it's:
   `captions="VTT_FILE_NAME.vtt|en"`

2. Add your subtitles file name in `subtitles` parameter, along with the translated language shortcode.\
Add `|default`, so that subtitle will be the default selected one when opening the translated page.

If no subtitles have been added yet, you may have to create the `subtitles` parameter.

{::nomarkdown}
{% include box.html type="start" title='Example (snippet): Arabic translation added' %}
{:/}

```liquid
   captions="VTT_FILE_NAME.vtt|en"
   subtitles="VTT_FILE_NAME.es.vtt|es,VTT_FILE_NAME.ar.vtt|ar|default"
```

{::nomarkdown}
{% include box.html type="end" %}
{:/}


#### More information

The video player may contain additional parameters:

- `subtitles-ad` \
  Audio described version of the subtitles.

- `descriptions-ad` \
  Text of the audio description.

In that case, apply the same logic as described above:
- Delete `|default` when specified next to the English version.
- Add your translated file in the parameter, along with the translated language shortcode and `|default`.

{::nomarkdown}
{% include box.html type="start" title='Example (snippet): Arabic translation added' %}
{:/}

```liquid
   captions="VTT_FILE_NAME.vtt|en"
   subtitles="VTT_FILE_NAME.ar.vtt|ar|default"
   subtitles-ad="VTT_FILE_NAME_ad.en.vtt|en,VTT_FILE_NAME_ad.ar.vtt|ar|default"
   descriptions-ad="VTT_FILE_NAME_ad_desc.en|en,TT_FILE_NAME_ad_desc.ar.vtt|ar|default"
```

{::nomarkdown}
{% include box.html type="end" %}
{:/}
