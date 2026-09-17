# risheekkumar.in

Source code for my personal technical blog: **[risheekkumar.in](https://risheekkumar.in)**.

The site is built with [Quarto](https://quarto.org/) and is used for writing about machine learning, LLMs, recommender systems, foundation models, and ML systems.

## Design

The visual design is inspired by [Astro Theme Pure](https://astro-pure.js.org/).

I recreated and adapted the theme in Quarto using custom CSS, HTML partials, and templates while keeping Quarto's notebook-first writing workflow.

## Stack

- [Quarto](https://quarto.org/)
- Python
- Jupyter notebooks
- Custom CSS and HTML partials
- GitHub Pages
- `uv` for Python dependency management

## Repository structure

```text
.
├── index.qmd
├── about.qmd
├── archive.qmd
├── projects.qmd
├── _quarto.yml
├── styles.css
│
├── posts/
│   ├── HNSW/
│   ├── KNN/
│   ├── bitcoin_from_scratch/
│   ├── gepa-deepdive/
│   ├── gepa-impact/
│   ├── micrograd-karpathy/
│   └── naive-bayes/
│
├── partials/
├── fonts/
└── docs/
```

`posts/` contains the source for individual articles, while `docs/` contains the rendered website served through GitHub Pages.

## Local development

Clone the repository:

```bash
git clone https://github.com/risheekkumarb/myblog.git
cd myblog
```

Install Python dependencies:

```bash
uv sync
```

Start the Quarto development server:

```bash
quarto preview
```

## Build

Render the full site with:

```bash
quarto render
```

The generated site is written to:

```text
docs/
```

## Writing workflow

Most posts begin as notebooks or small experiments.

```text
idea / question
      ↓
experiment
      ↓
notebook / implementation
      ↓
understand the concept
      ↓
write the article
      ↓
publish with Quarto
```

Quarto lets me keep code, outputs, equations, figures, and long-form explanations together instead of maintaining a separate blogging workflow.

## Acknowledgements

The design of this site is inspired by [Astro Theme Pure](https://astro-pure.js.org/).

The implementation in this repository is a Quarto adaptation with custom styling and components for notebook-based technical writing.

## Author

**Risheekkumar Baskaran**

- Website: [risheekkumar.in](https://risheekkumar.in)
- GitHub: [@risheekkumarb](https://github.com/risheekkumarb)
- LinkedIn: [Risheekkumar Baskaran](https://www.linkedin.com/in/risheekkumar-baskaran-748115120/)