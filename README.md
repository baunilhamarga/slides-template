# Academic Slides Template

This repository contains a non-official LaTeX Beamer template for academic presentations, project defenses, research updates, seminars, and similar technical talks.

The template was made by Heitor Gama from a previous presentation style. It is not official material from USP, CentraleSupelec, Crossing, CNRS, or any course team. It does not guarantee compliance with any conference, school, instructor, jury, or event formatting requirement. Use it at your own risk and always check the rules for the specific presentation you are preparing.

✅ [Overleaf version available!](https://www.overleaf.com/read/mznfqyswnwtg#38a56f)  
✅ [PLMlatex version available!](https://plmlatex.math.cnrs.fr/read/xkxympztjqzy)

If this template saves you time, please leave a ⭐ on the repository.

## What Is Included

- `main.tex`: the self-contained presentation template source.
- `references.bib`: sample BibTeX bibliography entries.
- `figures/`: background, logos, portrait, and sample visual assets used by the template.

The template includes a title slide, about slide, section divider slides, figures, tables, equations, animated table highlighting, footnote-style citations, a references slide, a thank-you slide, and a backup section for extra material.

## How To Adapt

Edit the presentation metadata near the top of `main.tex`:

```tex
\title[Technical Presentation Title]{{\bf \Huge Technical Presentation Template}}
\author[Heitor Gama]{...}
\newcommand{\presentationcontext}{Course, project, seminar, supervisors or conference track}
\newcommand{\presenteremail}{heitor\_gama@usp.br}
\newcommand{\presenterwebsite}{https://www.heitor-gama.com}
```

Replace the sample slides with the content of your talk. Keep each slide focused on one claim, comparison, figure, table, or equation. Move detailed derivations, extra tables, implementation notes, and additional examples to the backup section after the thank-you slide.

Add all cited sources to `references.bib`. The template uses `biblatex` and redefines `\cite{...}` to produce a footnote citation on the slide:

```tex
\renewcommand{\cite}[1]{\texorpdfstring{\footfullcite{#1}}{}}
```

Keep bibliography entries in one consistent standard.

## Figures And Photos

Prefer vector figures such as PDF for diagrams, plots, graphs, and schematic figures. Use PNG or JPEG only for pixel-level image data or photos.

The portrait helper clips a rectangular image into a centered circular mask:

```tex
\circlephoto{figures/heitor.jpg}{1.8cm}
```

The second argument controls the circle radius. The image is centered and scaled so the shorter side fills the circle diameter.

## License And Reuse

See [LICENSE](LICENSE). Keep the source notice at the top of `main.tex` in every copy or derivative version. The template may be used, adapted, and distributed as long as that notice is kept.
