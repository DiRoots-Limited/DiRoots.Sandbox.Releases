---
layout: default
title: Terms explained
nav_order: 4
permalink: /docs/terms/
---

# Terms explained
{: .no_toc }

A few terms used when working on the documentation website.
{: .fs-6 .fw-300 }

| Term | Meaning in this sandbox |
| --- | --- |
| Markdown | Plain text with simple formatting for headings, links, lists and tables. The help pages are Markdown files. |
| Jekyll | The tool that turns the source pages and settings into a website. |
| Just the Docs | The theme that provides the sidebar, search and page styling, also used by DiStem's documentation. |
| GitHub Pages | The GitHub service that builds and hosts the sandbox website. |
| `gh-pages` | The branch containing this site's documentation. It is a branch name rather than a separate service. |
| Pull request or PR | A proposed change that can be reviewed before it is merged into a branch. |
| Documentation preview | A temporary version of the website showing a PR's proposed changes. |
| Workflow | Automated instructions that build, publish, update or remove a site. |
| GitHub App | The integration that will give the publishing workflow permission to write preview files. |

## Website and preview

The main sandbox website shows the documentation merged into `gh-pages`. Once previews are enabled, a PR preview will show proposed changes before they are merged. Closing a PR will remove its temporary preview.

Start with [Getting started]({{ '/docs/getting-started/' | relative_url }}) to try a documentation change.
