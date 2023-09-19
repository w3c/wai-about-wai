---
title: "Using GitHub"
nav_title: Using GitHub
github:
  repository: w3c/wai-about-wai
  path: '_about/translating/guides/using-github.md'
permalink: /about/translating/guides/using-github/
ref: /about/translating/guides/using-github/
lang: en
doc-note-type: draft
doc-note-message-md: This page is a **work-in-progress draft needing extensive edits.**

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 13 September 2023.</p>
   <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>, Rémi Bétin.</p>
---

{::nomarkdown}
{% include box.html type="start" title="Summary" class="" %}
{:/}

Here are some guidance to use GitHub.

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

We encourage you to use GitHub.
If you are not comfortable with it, we can work with text files.

## Getting to the repository: 

Near the bottom of each page on the WAI website, there is a "Help improve this page" box. The middle button is "Fork & Edit in GitHub". That gets you to the repository.

You can fork and edit from the main repository.

## Translations Ready for Review


## Pull Request Status & Title

To help us keep track of the pull requests and status, please use this for your Pull Request Titles:

`[status] Language - Resource Title`

with status of `IN-PROGRESS` or `Ready for Review` or `Ready to Publish` (after it is reviewed and ready for publication)

For example:

~~~
[IN-PROGRESS] Spanish - Accessibility Principles
[Ready for Review] Spanish - Accessibility Principles
[Ready to Publish] Spanish - Accessibility Principles
~~~

To let others know that your translation is ready for review, please send e-mail to public-wai-translations@w3.org with subject:

[Language] Request for Review – [resource title]
If you're using GitHub, include:
link to the preview
link to the pull request
If you are not using GitHub, attach your translation to the e-mail.
Include:

When published, it will be available at: [uri/language-code]
The URI is the same as the English page + the language code at the end. For example:
https://www.w3.org/WAI/standards-guidelines/ko (This is for later readers of the list archives. After we close the pull request, the preview won't be available and we want readers to find your published version. :-)

If you know people who might review the resource (for example, other translators in your language):

It is usually best to also send the e-mail directly to other translators in your language so they don't miss it on the list. :-)
And/or mention them in the GitHub pull request so they get notification.
If others have already reviewed your translation (and are OK being listed as a reviewer), include their names in the GitHub pull request "Conversation", or in the e-mail.
When it's Ready for Publication
When your translation has been sufficiently reviewed and you have addressed comments, let us know that it is done.
Please send e-mail to public-wai-translations@w3.org with subject:

Completed Translation – [language code] – [resource title]
If you're using GitHub, include a link to the pull request.
If you are not using GitHub, attach your translation to the e-mail.
Include:

When published, it will be available at: [uri/language-code]
The URI is the same as the English page + the language code at the end. For example:
https://www.w3.org/WAI/standards-guidelines/ko (This is for later readers of the list archives. After we close the pull request, the preview won't be available and we want readers to find your published version. :-)

If you want to include a link to information about you, per the policy at https://www.w3.org/WAI/about/translating/#links, include the link in the e-mail.

Remember to let us know about reviewers per above.

## Preview

We have enabled a preview with Netlify so you can check your file and make edits. To see the preview, you need to submit a pull request. Please start the pull request title with "[IN-PROGRESS]" so we know it's not ready for review yet. Make it a draft pull request while you are working on it.

To set it as a draft pull request:

1. In the "Create pull request" button, select the drop-down arrow.

2. In the drop-down options, select "Create draft pull request".
   GitHub-draft-PR-1.png
   The button changes to "Draft pull request".

3. Select the "Draft pull request" button.
   GitHub-draft-PR-2.png

After you submit the pull request, it will create a preview. At first it will say "Some checks haven't completed yet.".
Preview-waiting.png

After a few minutes, the box will say "All checks have passed"
The last line is "deploy/netlify — Deploy preview ready!"
At the end of that line, click the "Details" link to see your preview.
Preview ready.png

If you get a message that the checks have failed, it is probably because there is a problem in the markup.

Click on that last "Details" link.
It will open up a "Deploy log".
Skim through the log until you see information about what failed (in red text).
If you're not able to fix the issue, let us know, and we can help. :-)
