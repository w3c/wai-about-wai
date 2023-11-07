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
doc-note-message-md: This page is a draft. **It welcomes feedbacks.**

description: Help make the Web accessible to people with disabilities around the world. We appreciate your contributions to translating W3C WAI accessibility resources.
image: /content-images/wai-about-wai/social-translations.png

feedbackmail: wai@w3.org
footer: |
  <p><strong>Date:</strong> Updated 28 September 2023.</p>
   <p><strong>Editors:</strong> <a href="https://www.w3.org/People/Shawn/">Shawn Lawton Henry</a>, Rémi Bétin.</p>

inline_css: |
   figure.screenshot {
      margin-block-start: 1em;   
   }
   
   figure.screenshot img {
      box-shadow: 3px 3px 3px #ddd;
   }

---

{::options toc_levels="2,3" /}
{::nomarkdown}
{% include toc.html type="start" title="Page Contents" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include toc.html type="end" %}
{:/}

## Creating a translation in GitHub - A step by step guide

{% include showhidebutton.html showtext="Show all screenshots" hidetext="Hide all screenshots" target=".screenshot" %}

### Create the translation file

<ol>
   <li>
   Near the bottom of each page on the WAI website, there is a "Help improve this page" box.<br />
   The middle button is "Fork & Edit in GitHub". That gets you to the GitHub repository.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".fork-edit-link" %}
   <figure class="fork-edit-link screenshot">
      {% include image.html src="translating/fork-edit-link.jpg" alt="Screenshot of the “Help improve this page” box. The “Fork & Edit in Github” middle button is outlined in dark orange." %}
   </figure>
   </li>
   <li>
   From there, you will be asked to “Fork the repository” – that is, creating a copy of the repository so you can make changes without affecting the original one.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".fork-repo" %}
   <figure class="fork-repo screenshot">
      {% include image.html src="translating/fork-repo.jpg" alt="TBD" %}
   </figure>
   </li>
   <li>
   On the next screen, select all the original file code and copy it to your clipboard (<kbd><kbd>Ctrl</kbd>+<kbd>C</kbd></kbd> or <kbd><kbd>⌘</kbd>+<kbd>C</kbd></kbd>).
   </li>
   <li>
   Click on the expand icon, next to the editor breadcrumb, to show the repository file tree.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".expand-file-tree" %}
   <figure class="expand-file-tree screenshot">
      {% include image.html src="translating/expand-file-tree.jpg" alt="Screenshot of the edit view in GitHub: the Expand icon is outlined in dark orange next to the secondary breadcrumb." %}
   </figure>
   </li>
   <li>
   Click on the "+" icon to create a new file.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".new-file" %}
   <figure class="new-file screenshot">
      {% include image.html src="translating/new-file.jpg" alt="Screenshot of the edit view in GitHub, with the file tree expanded. The “+” icon with a “Add file” label on hover is outlined in dark orange." %}
   </figure>
   </li>
   <li>Name the new file according to instructions on <a href="/wai-about-wai/about/translating/guides/new-translation/#create-file">Creating a New Translation</a> page.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".name-new-file" %}
   <figure class="name-new-file screenshot">
      {% include image.html src="translating/name-new-file.jpg" alt="Screenshot of the edit view in GitHub. The “File name” field, at the end of the secondary breadcrumb, is outlined in dark orange." %}
   </figure>
   </li>
   <li>
   <p>Paste the original content that you copied in step 2 into the editor (<kbd><kbd>Ctrl</kbd>+<kbd>V</kbd></kbd> or <kbd><kbd>⌘</kbd>+<kbd>V</kbd></kbd>).</p>
   <p>&#127881; <strong>Congrats! You have now created the translation file to work with.</strong></p>
   </li>
</ol>

### Work on your translation

<ol start="8">
   <li>
   Edit the content to translate the file, following guidance from <a href="/wai-about-wai/about/translating/guides/new-translation/">Creating a New Translation</a> page.
   </li>
   <li>
   When you are happy with your work, click on "Commit changes..." to save the changes.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".commit-changes" %}
   <figure class="commit-changes screenshot">
      {% include image.html src="translating/commit-changes.jpg" alt="Screenshot of the edit view in GitHub. The “Commit changes...” button, next to the “Cancel changes” button, is outlined in dark orange." %}
   </figure>
   </li>
   <li>
   <p>In the appearing "Propose changes" modal window, you can rename your commit message to better reflect what you have changed. Then, click on "Propose changes".
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".propose-changes" %}</p>
   <figure class="propose-changes screenshot">
      {% include image.html src="translating/propose-changes.jpg" alt="Screenshot of the “Propose changes” modal window in GitHub. The “Commit message” field says “Create french translation for Tips in Designing page”. The “Propose changes” button, next to the “Cancel” button, is outlined in dark orange." %}
   </figure>
   <p>&#127881; <strong>Congrats! You have now commited your changes!</strong></p>
   </li>
</ol>

### Prepare your draft Pull Request

<ol start="11">
   <li>
   <p>You are now in the "Comparing changes" view, between the "base" repository (the original W3C repository, beginning with w3c) and the "head" repository (your forked repository, beginning with your username).</p>
   <p>Click on "Create pull request", meaning that you propose to apply your changes to the official repository. If the button does not appear, you may need to refresh the page.    {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".compare-changes" %}</p>
   <figure class="compare-changes screenshot">
      {% include image.html src="translating/compare-changes.jpg" alt="TBD" %}
   </figure>
   </li>
   <li><p>Set the title of the Pull request using the following format: <strong>[IN-PROGRESS] Language - Resource Title.</strong></p>
   <p>Then, in the "Create pull request" button, select the drop-down arrow and select "Create draft pull request in the drop-down options. {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".create-draft-pull-request" %}
</p>
   <figure class="create-draft-pull-request screenshot">
      {% include image.html src="translating/create-draft-pull-request.jpg" alt="TBD" %}
   </figure>
   </li>
   <li><p>Click on the "Draft pull request" button to confirm the submission of the pull request.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".draft-button" %}</p>
   <figure class="draft-button screenshot">
      {% include image.html src="translating/draft-button.jpg" alt="TBD" %}
   </figure>
   <p>&#127881; <strong>Congrats! Your draft pull request is now created!</strong></p>
   </li>
</ol>

### Preview your changes

<ol start="14">
   <li>After you submit the pull request, it will create a preview so you can check your file and make edits. At first, a notification comment will say <strong>"👷 Deploy Preview for <em>wai-repo-name</em> processing."</strong>
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".preview-processing" %}
   <figure class="preview-processing screenshot">
      {% include image.html src="translating/preview-processing.jpg" alt="TBD" %}
   </figure>
   </li>
   <li><p>After a few minutes, the notification comment will change to <strong>“✅ Deploy Preview for <em>wai-repo-name</em> ready!”</strong>.</p>
   <p>To see your preview, click on the "Deploy Preview" link. {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".preview-ready" %}</p>
   <figure class="preview-ready screenshot">
      {% include image.html src="translating/preview-ready.jpg" alt="TBD" %}
   </figure>
   </li>
</ol>

### Mark your Pull request as ready for review

<ol start="16">
<li><p>When you have done all your checks and edits, click on the "Edit" button at the top of the Pull request view, to change the title prefix "[IN-PROGRESS]" to <strong>"[Ready for Review]"</strong></p>
   <p>Then, click on the "Ready for review" button, at the bottom of the Pull request view. {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".ready-for-review-button" %}</p>
   <figure class="ready-for-review-button screenshot">
      {% include image.html src="translating/ready-for-review-button.jpg" alt="TBD" %}
   </figure>
   </li>
   <li><p>&#127881; <strong>Congratulations, your pull request is now ready for review!</strong></p>
   <p>You can see it is marked as "Open" with a green label at the top of the Pull request view.
   {% include showhidebutton.html showtext="Show screenshot" hidetext="Hide screenshot" target=".ready-for-review-state" %}</p>
   <figure class="ready-for-review-state screenshot">
      {% include image.html src="translating/ready-for-review-state.jpg" alt="TBD" %}
   </figure>
   </li>
</ol>