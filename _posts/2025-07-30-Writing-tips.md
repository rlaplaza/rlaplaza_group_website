---
title: Writing tips and tricks
image: images/post-tutorial.jpg
author: rlaplaza
tags: tutorial, guidelines
---

# Scientific Paper Writing Guidelines

## About

This document provides a structured guide to help you write a clear, rigorous, and publishable **scientific manuscript**, especially in the **chemical sciences**. It is tailored to those using **[Overleaf](https://www.overleaf.com/)** with **[ACS](https://www.overleaf.com/latex/templates/acs-publishing-template/jngpwwcvzjtv)** or **[RSC](https://www.overleaf.com/latex/templates/rsc-article-template/fhxhhrxcqzvm)** LaTeX templates, but the core principles apply universally.

---

## Getting Started

### Choose the Right Journal

Before writing, define your **target journal**. This influences structure, style, and reference format. Consider:

- Scope of the journal
- Impact factor and audience
- Recent articles similar to your work

Links:
- [ACS Journals List](https://pubs.acs.org/page/journals)
- [RSC Journals List](https://www.rsc.org/journals-books-databases/about-journals/)
- [Journal Finder (Elsevier)](https://journalfinder.elsevier.com/)

### Use the Official Template

Overleaf templates ensure correct formatting and metadata setup.

Here are some useful ones, but for most journals we will probably have a previous example. For others, you may have to look for the template yourself (if it exists!):

- **ACS Template:** [Link](https://www.overleaf.com/latex/templates/latex-template-for-american-chemical-society-acs-journal-submissions/nzngbcrcptmm)
- **RSC Template:** [Link](https://www.overleaf.com/latex/templates/tagged/rsc)

Follow the structure provided and don’t override style commands unless necessary.

- In general, I prefer using [Overleaf](https://www.overleaf.com/) for all manuscripts (unless a journal prohibits LaTeX). Use group-maintained Overleaf templates where possible (cover letters, SI, latexdiff, etc.). If you are not sure if there is one, ask me!
- Use cross-references (`\ref{}`) for figures, tables, sections—**never hard-code numbers**.
- For versioning: Continue working in one Overleaf project. Backup older versions by copying to separate `.tex` files every now and then, specially before major changes.
- For reviewer responses: Use `latexdiff` to highlight changes (e.g., for reviewer responses). For the actual answers, we may use [Google docs](https://docs.google.com/) instead.

### Outline First

Before writing, prepare an outline for discussion with your advisor (i.e., me). The outline should include:

- **Abstract**: 4–8 sentences summarizing the entire paper's message and contributions.
- **Introduction**: A paragraph-level sketch of background, open questions, and this paper’s specific goals. End with a clear list of 2–4 main contributions.
- **Figure 1**: Often a schematic or conceptual diagram—draft this early.
- **Results**: Describe key experiments, figures, and tables. Write draft captions early on—they should be mostly self-contained.
- **Discussion**: Draft sections for analysis and interpretation, including an explicit **limitations** paragraph if applicable.

---

## General Structure of a Scientific Paper

### 1. Title

- Concise, descriptive, and specific
- Avoid jargon or overly broad titles
- Include keywords if relevant

### 2. Abstract

- 150–250 words
- Summarize the problem, key methods, major results, and conclusions
- Write it **last**, even though it appears first

### 3. Introduction

- Context and motivation
- Review of relevant work (with citations)
- Clearly state the **research question or hypothesis**
- End with a summary of **your contribution**

### 4. Results and Discussion

- Present results in **logical order**, not necessarily chronological
- Use **figures and tables** to highlight key findings
- Discuss implications, limitations, and comparisons with prior work
- Include **control experiments** or computational benchmarks if relevant

### 5. Methods / Experimental Section

- Describe methods with enough detail to allow replication
- Separate subsections for synthesis, measurements, and simulations
- Include software versions, parameters, and tools used
- Use SI units and standard nomenclature

### 6. Conclusions

- Recap major findings, make sure message is clear even if its repetitive
- Emphasize scientific impact
- Optionally outline future directions

### 7. References

- Use a **consistent and journal-appropriate** style (ACS, RSC, etc.)
- Use BibTeX with a reference manager like:
  - [Zotero](https://www.zotero.org/)
  - [Mendeley](https://www.mendeley.com/)
  - [JabRef](https://www.jabref.org/)

To generate BibTeX entries from DOIs, use:
- [DOI2Bib](https://www.doi2bib.org/)

To clean up `.bib` files, use:
- [betterbib (GitHub)](https://github.com/texworld/betterbib)

---

## Writing Tips

### Be Clear and Concise

- Prefer short, direct sentences
- Avoid unnecessary jargon
- Eliminate filler phrases (e.g., "it is worth mentioning that")

### Be Scientific

- Support all claims with **data or references**
- Use error bars, confidence intervals, and statistical significance where applicable
- Avoid overclaiming or hyping results

### Be Structured

- Use informative section headers
- Use logical transitions between paragraphs
- Ensure each paragraph has one core idea

### Be Visual

- Use well-labeled figures and tables
- Avoid clutter in graphs (no rainbow plots, overly small fonts)
- Refer to **every** figure/table in the main text

Recommended tools for figure-making are:
- [ChemDraw](https://www.perkinelmer.com/category/chemdraw), always with ACS style
- [Matplotlib](https://matplotlib.org/) / [Plotly](https://plotly.com/)

---

## Overleaf and LaTeX Tips

- Use `\cite{}` with a `.bib` file to manage references
- Use `\autoref{}` or `\ref{}` for cross-referencing
- Define custom commands for repeated symbols or equations
- Add `% TODO:` comments to mark unfinished areas
- Use `[draft]` option in `\documentclass` for fast compilation during writing

---

## Final Checklist

- Never submit any version (poster, abstract, manuscript) without advisor approval.
- If deadlines are involved, plan ahead for:
  - Internal review. It takes me time to review a paper critically and several rounds may (probably will) be necessary.
  - External collaborator approval — **allow ≥30 days** if needed.

Before submission or feedback, ensure:

### ✅ Scientific Rigor

- All claims supported with data or references
- All figures readable and reproducible
- All abbreviations defined at first use

### ✅ Formatting

- Correct journal style (template, references, headings)
- Figures and tables placed appropriately
- Units and nomenclature are consistent and SI-compliant when possible (for energies, we like kcal/mol or eV)

### ✅ Language and Clarity

- Spell-checked and grammar-checked
- No overly long or vague sentences
- Clear and engaging abstract

### ✅ Metadata

- Author names and affiliations are correct
- ORCID and email info included
- Proper keywords provided (if required)

---

## Bonus Tools

- [Grammarly](https://www.grammarly.com/) – grammar and style check
- [Writefull](https://writefull.com/) – language correction for scientific writing
- [LaTeX table converter](https://tableconvert.com/) – for tables
- [LaTeX equation writer](https://latexeditor.lagrida.com/) – for equations
- [Overleaf LaTeX Tutorials](https://www.overleaf.com/learn)
- [Data Visualization: A Practical Introduction](https://serialmentor.com/dataviz/)
- [Multipanel figures](https://stackoverflow.com/questions/44970010/axes-class-set-explicitly-size-width-height-of-axes-in-given-units)

---

