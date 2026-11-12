---
layout: default
title: Preview checklist
nav_order: 3
permalink: /docs/preview-checklist/
---

# Preview checklist
{: .no_toc }

Use these sample changes to check the documentation preview flow once the shared workflows are connected.
{: .fs-6 .fw-300 }

## Before previews are enabled

Check the published sandbox site after this initial setup merges:

- The homepage and all three help pages load.
- The sidebar highlights the current page.
- Search finds the phrase **sandbox example** from the homepage.
- Internal links stay inside the sandbox website.
- The pages remain readable in a narrow browser window.

## Open and update a preview

1. Create a branch from `gh-pages` and change the homepage's sample sentence.
2. Open a pull request targeting `gh-pages`.
3. Wait for the build and publication workflows to succeed.
4. Open the preview link posted by the workflow on the PR.
5. Confirm the preview contains the changed sentence while the main sandbox site still shows the merged version.
6. Push another edit to the same branch and confirm the preview and its existing comment update.

These preview steps require the workflows and GitHub App access to be configured first.

## Expected lifecycle

| Action | Expected result after previews are enabled |
| --- | --- |
| Open a same-repository documentation PR | A temporary website and one preview comment appear. |
| Update the PR | The preview shows the latest eligible build. |
| Close the PR without merging | The preview is removed; the main site keeps its existing content. |
| Merge the PR | The main site receives the changes and the temporary preview is removed. |
| Introduce a build error | The workflow reports a failure and does not publish a new preview. |

## Check formatting

This page includes headings, an ordered list, a bullet list and a table so reviewers can compare their appearance in the published site and a preview.

Return to [Getting started]({{ '/docs/getting-started/' | relative_url }}) or the [homepage]({{ '/' | relative_url }}).
