# R Markdown for Scientists — NIEHS Training

A 3-hour hands-on workshop on creating reproducible reports with R Markdown,
designed for scientists at the National Institute of Environmental Health
Sciences (NIEHS).

## Platform

This training is designed to run on **[Posit Cloud](https://posit.cloud)** 
(formerly RStudio Cloud). No local software installation is required.

## Workshop Structure (3 Hours)

| File | Module | Time |
|------|--------|------|
| `00_welcome_and_setup.Rmd` | Welcome, setup, and package installation | 10 min |
| `01_rmarkdown_basics.Rmd` | YAML headers, Markdown syntax, and knitting | 25 min |
| `02_code_chunks.Rmd` | Code chunks, chunk options, inline code | 30 min |
| `03_tables_and_data.Rmd` | Tables with kable, kableExtra, and DT | 25 min |
| — | **Break** | 10 min |
| `04_visualizations.Rmd` | ggplot2 figures, sizing, captions, plotly | 25 min |
| `05_scientific_writing.Rmd` | Equations, citations, parameters | 20 min |
| `06_output_formats.Rmd` | HTML themes, Word, PDF, custom CSS | 15 min |
| `07_capstone_exercise.Rmd` | Build a complete analysis report | 20 min |

## Prerequisites

- A free **Posit Cloud** account ([posit.cloud](https://posit.cloud))
- A free **GitHub** account ([github.com](https://github.com)) — recommended
- A modern web browser (Chrome, Firefox, or Edge)
- No prior R Markdown experience required (basic R familiarity helpful)

## Getting Started

### Option A: From GitHub (recommended)
1. Log in to Posit Cloud
2. Click **New Project → New Project from Git Repository**
3. Paste the GitHub repository URL
4. Open `00_welcome_and_setup.Rmd` and click **Knit**

### Option B: Upload manually
1. Log in to Posit Cloud and create a new project
2. Upload all `.Rmd` files to the project
3. Open `00_welcome_and_setup.Rmd` and click **Knit**

## Required Packages

Run this in the R console if packages aren't installed:

```r
install.packages(c(
  "rmarkdown", "knitr", "tidyverse", "kableExtra",
  "DT", "plotly", "broom", "patchwork", "here"
))
```

## Key Learning Outcomes

By the end of this workshop, participants will be able to:

1. Create R Markdown documents with proper YAML configuration
2. Write narrative text using Markdown formatting
3. Use code chunks with appropriate options for different audiences
4. Report statistics dynamically with inline R code
5. Create publication-quality tables and figures
6. Add equations, citations, and cross-references
7. Produce output in HTML, Word, and PDF formats
8. Build parameterized reports that scale across sites or chemicals

## Presentation Slides (for instructors)

The `slides/` folder contains **ioslides presentation** versions of each
module that you can present directly from RStudio or Posit Cloud.

| File | Covers | Approx. Time |
|------|--------|-------------|
| `slides/slides_01_welcome_and_basics.Rmd` | Welcome + Module 1 (YAML, Markdown, Knitting) | 35 min |
| `slides/slides_02_code_chunks.Rmd` | Module 2 (Chunk options, Inline code) | 30 min |
| `slides/slides_03_tables.Rmd` | Module 3 (kable, kableExtra, DT, broom) | 25 min |
| `slides/slides_04_visualizations.Rmd` | Module 4 (ggplot2, sizing, patchwork, plotly) | 25 min |
| `slides/slides_05_scientific_writing.Rmd` | Module 5 (Equations, Parameters, Citations) | 20 min |
| `slides/slides_06_formats_capstone_closing.Rmd` | Modules 6–7 (Formats, Capstone, Resources) | 35 min |
| `slides/rmd_slides_style.css` | Custom theme (navy/blue color scheme) | — |

### How to present

1. Open any `slides/slides_*.Rmd` in RStudio / Posit Cloud
2. Click **Knit** → HTML slides render in the Viewer pane
3. Click **"Show in new window"** for full-screen presentation
4. Arrow keys or click to advance; press **P** for presenter notes
5. No extra packages needed — uses `ioslides_presentation` built into `rmarkdown`

### Features

- Live R code output on slides (tables, plots render during knitting)
- `{.segue}` section dividers with navy backgrounds
- `{.build}` for incremental bullet reveal
- Presenter notes via `<div class="notes">` blocks
- `self_contained: true` — standalone HTML files you can email
7. Produce output in HTML, Word, and PDF formats
8. Build parameterized reports that scale across sites or chemicals

## Resources

- [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)
- [R Markdown Cookbook](https://bookdown.org/yihui/rmarkdown-cookbook/)
- [R Markdown Cheat Sheet](https://www.rstudio.com/resources/cheatsheets/)
- [Posit Cloud Documentation](https://docs.posit.co/cloud/)

## License

These training materials are provided for educational use at NIEHS.
