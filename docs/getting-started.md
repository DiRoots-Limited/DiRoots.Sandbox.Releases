---
layout: default
title: Getting started
nav_order: 2
permalink: /docs/getting-started/
---

# Getting started
{: .no_toc }

Use this site to learn the documentation flow and check a change before adopting the workflows in a product repository.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## How the site is published

The documentation lives on the `gh-pages` branch of `DiRoots.Sandbox.Releases`. GitHub Pages reads that branch and uses Jekyll to turn the Markdown pages into a website.

The `develop` branch is the repository's default branch. It will hold the trusted publishing caller when the preview workflows are installed. The website's files and the preview build caller belong in the documentation branch.

## Propose a documentation change

1. Start a new branch from `gh-pages`.
2. Edit a sample page, such as the sample sentence on the homepage.
3. Open a pull request targeting `gh-pages`.
4. Review the text and formatting before merging it.

When the PR merges, GitHub Pages rebuilds the sandbox website. A temporary PR preview is a separate feature that will become available after the shared workflows are connected.

## Write a sample help page

A documentation page starts with settings between two lines of three dashes. These settings tell the theme which layout, sidebar title and position to use.

```markdown
---
layout: default
title: Example help page
nav_order: 5
---

# Example help page

Explain one task in a short paragraph.

1. Describe the first step.
2. Describe the expected result.
```

## Check the result

Use the sidebar to switch pages, try the search box and follow an internal link. The [preview checklist]({{ '/docs/preview-checklist/' | relative_url }}) lists the checks to repeat when automatic previews are enabled.
