---
layout: post
title: "GSoC Final Report"
description: Summary of the entire work done on 'Lesson translation dashboard' for Oppia Foundation during GSoC 2018.
headline: Google Summer of Code 2018
category: GSoC-Report
tags: [GSoC, report, translation-tab, Oppia-Foundation]
imagefeature: gsoc_1.svg
comments: true
share: true
featured: true
published: true
---
As Google Summer of Code 2018 draws to a close, I'd like to summarize my work  for Oppia Foundation on the project - 'Lesson translation dashboard'. I had an awesome experience working with the Oppia Foundation community, under the mentorship of two amazing people - **Tony Jiang** and **Anmol Shukla**.

This post aims at linking and listing out all the feature milestones developed during my project and the relevant pull requests, along with the work to be done in the future.

<h1>Milestones Achieved</h1>
<ol>
  <li>
    <b>Milestone 1</b> - This Milstone was mostly focousing on the backend part of the project and the blog post describing the feature can be seen <a href="/sidebar-documentation/Milestone-1-post" target="_blank"><i>here</i></a>.
    <h4>Pull requests merged</h4>
    <ul>
      <li>
        <a href="https://github.com/oppia/oppia/pull/4959" target="_blank">PR#4959: Milestone 1.1: Add translator role for the exploration.</a>
        <ul>
          <li> Added “translator” role for the exploration.</li>
          <li> Added new entity translator_ids in ExplorationSummary and ActivityRights object.</li>
          <li> Added `translator_ids` in ExplorationSummaryModel and ExplorationRightsModel.</li>
          <li> Wrote @acl_decorators for can_translate_exploration.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5007" target="_blank">PR#5007: Milestone 1.2: Refactor exploration state structure.</a>
        <ul>
          <li> Replaces audio_translations to content_id in SubtitledHtml.</li>
          <li> Adds Content_ids_to _audio_translation to connect audio translations with SubtitledHtml.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5099" target="_blank">PR#5099: Milestone 1.3: </a>
        <ul>
          <li> Allowed an exploration owner to assign translator for their exploration.</li>
          <li> Made editor page accesible to translators.</li>
          <li> Allowed translators to upload, delte and mark need updates translated audio.</li>
        </ul>
      </li>
    </ul>
  </li>
  <br>
  <li>
    <b>Milestone 2</b> - In this milestone a simple version of translation tab was built and the blog post describing the feature can be seen <a href="/sidebar-documentation/Milestone-2-post" target="_blank"><i>here</i></a>.
    <h4>Pull requests merged</h4>
    <ul>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5122" target="_blank">PR#4959: Milestone 2.1 & 2.2: Translation overview directive.</a>
        <ul>
          <li> Created TranslationLanguageService (and Spec).</li>
          <li> Made navbar functional for audioTranslation tab.</li>
          <li> Added translation-tab directive.</li>
          <li> Added translation-overview directive.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5163" target="_blank">PR#5007: Milestone 2.3: Translation status graph directive.</a>
        <ul>
          <li> Adds graph to translation tab.</li>
          <li> Connected graph with translation overview directive.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5210" target="_blank">PR#5099: Milestone 2.4: State translation directive</a>
        <ul>
          <li> Added state content in the translation tab.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5279" target="_blank">PR#5279: Milestone 2.5: Audio translation bar for translation tab.</a>
        <ul>
          <li> Added recording functionality in translation tab.</li>
          <li> Allowed translators to record and save the translated audio.</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>
    <b>Milestone 3</b> - In this milestone the complete version of translation tab was built and the blog post describing the feature can be seen <a href="/sidebar-documentation/Milestone-2-post" target="_blank"><i>here</i></a>.
    <h4>Pull requests merged</h4>
    <ul>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5378" target="_blank">PR#5378: Milestone 3.1 & 3.2: Translation Status color.</a>
        <ul>
          <li> Created TranslationStatusService.</li>
          <li> Added colors for graph node to show the translation status of the state.</li>
          <li> Added status color for translation nav bar.</li>
          <li> Added exploration translation progress slider in translation-overview directive.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5413" target="_blank">PR#5413: Milestone 3.3: Removing audio translation bar from editor page.</a>
        <ul>
          <li> Removed audio translation bar from editor tab.</li>
        </ul>
      </li>
      <li>
        <a href="https://github.com/oppia/oppia/pull/5483" target="_blank">PR#5483: Milestone 3.4: Added drag and drop files functionality</a>
        <ul>
          <li> Added funcionality to drag and drop files in the new translation tab.</li>
        </ul>
      </li>
    </ul>
</li>
</ol>


<h1>Future work:</h1>
<ol>
    <li>
        <b>Will add soon!</b>
    </li>
</ol>
<br>
You may find all my github pull requests <a href="https://github.com/oppia/oppia/pulls?q=is%3Apr+author%3ADubeySandeep+is%3Aclosed" target="_blank"><i>here</i></a> in one go.

Overall, a summer well spent. I'll be contributing to Oppia Foundation even after the completion of GSoC, aiming to fix the rest of the Sidebar issues. Happy Hacking!
