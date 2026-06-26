# PREreview Champions' Handbook 

This repository contains the source files for [a Quarto site mock-up of the PREreview Champions' Handbook](https://xiuqili-xl.github.io/PREreview-Champions-Handbook-DEV/).

This repository is a fork of [`PREreview/champions-handbook`](https://github.com/PREreview/champions-handbook). It is being used to explore what the handbook could look like as a Quarto website, with reader-facing handbook content separated from source code for maintainers and contributors.

Note, this README is written for maintainers and contributors working on the website source.


## About this repository

The handbook is built with [Quarto](https://quarto.org/) as a static website.

Key files and directories:

- `_quarto.yml` controls the website structure, navigation, theme, and output settings
- `index.qmd` is the Home page of the published handbook
- `about-PREreview.qmd` and `how-to-contribute.qmd` are top-level website pages
- `subpages-champions-program/` contains subpages under the *About the Champions Program* menu
- `subpages-resources/` contains subpages under the *Resources* menu.
- `images/` contains images used throughout the site
- `.github/workflows/quarto-publishing.yml` publishes the rendered site to GitHub Pages


## Editing Content

Most handbook content is written in `.qmd` files using Markdown.

To make a content update:

1. Edit the relevant `.qmd` file
2. If adding a new page to the navigation bar, add it to `_quarto.yml` 
3. Preview the site locally when possible


## Previewing Locally

If you have Quarto installed, you can preview the website with:

```bash
quarto preview
```

To render the full site locally, use:

```bash
quarto render
```


## Publishing

The source files live on the `main` branch. When changes are pushed to `main`, the GitHub Actions workflow in `.github/workflows/quarto-publishing.yml` renders the Quarto site and publishes the built website to the `gh-pages` branch.

Maintainers should avoid editing the generated files on `gh-pages` directly. Content and configuration changes should be made on `main`.



## Gen AI usage

Generative AI (Codex, GPT-5.5, Medium Intelligence) was used to draft this `README.md file` and troubleshoot code. Content of this `README.md` file has been reviewed and edited to ensure accuracy.


