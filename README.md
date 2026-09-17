Risheekkumar’s Blog

Source code for my personal technical blog: risheekkumar.in.

I write about machine learning, foundation models, recommender systems, LLMs, and the software systems behind them. The blog is primarily a place for me to learn things deeply by implementing, experimenting, and then explaining what I understood.

Design

The site is built with Quarto.

Its visual design is heavily inspired by Astro Theme Pure. I liked Pure’s minimal typography, navigation, article layout, dark mode, and overall focus on long-form writing, and recreated that style within Quarto while adapting it for notebook-driven technical posts.

So the stack is roughly:

Pure-inspired design → Quarto implementation → notebooks/code as articles → GitHub Pages

What I write about

Most posts sit somewhere around the intersection of machine learning and software:

* Machine learning from first principles
* Foundation models and sequence modeling
* Recommender and retrieval systems
* LLM optimization and evaluation
* ML systems, performance, and memory
* Implementations of papers and algorithms
* Experiments that help me understand how things actually work

Some posts are conventional technical deep dives. Others use code, diagrams, analogies, or stories to build intuition before getting into the implementation.

Philosophy

I don’t want this to become a collection of summaries of things I already know.

The idea is closer to:

Learn something deeply enough that I can rebuild it, experiment with it, and explain why it works.

A post might therefore begin as a notebook, an implementation, a paper I’m trying to understand, or a problem I run into while building something.

Writing the article is part of the learning process.

Repository structure

.
├── index.qmd          # Homepage
├── about.qmd          # About
├── archive.qmd        # Posts archive
├── projects.qmd       # Projects
│
├── posts/             # Articles and notebooks
│   ├── HNSW/
│   ├── KNN/
│   ├── bitcoin_from_scratch/
│   ├── gepa-deepdive/
│   ├── gepa-impact/
│   ├── micrograd-karpathy/
│   └── naive-bayes/
│
├── partials/          # Custom Quarto/HTML components
├── fonts/
├── styles.css         # Site styling
├── _quarto.yml        # Quarto configuration
└── docs/              # Rendered site

Running locally

Install Quarto and clone the repository:

git clone https://github.com/risheekkumarb/myblog.git
cd myblog

The Python environment is managed with uv:

uv sync

Then start Quarto:

quarto preview

To render the complete website:

quarto render

The generated site is written to docs/ and served using GitHub Pages.

Writing workflow

Most technical posts start as notebooks or code-heavy experiments.

I prefer keeping the implementation and the explanation close together:

question
   ↓
experiment / notebook
   ↓
understand the implementation
   ↓
write the explanation
   ↓
Quarto article

Quarto works particularly well for this because executable notebooks, Markdown, equations, code, figures, and long-form writing can all live in the same project.

Acknowledgements

The site’s design is inspired by Astro Theme Pure.

The website itself is implemented in Quarto, with custom CSS, templates, and components to reproduce and adapt that design for my technical-writing workflow.

About

I’m Risheekkumar Baskaran, a data scientist interested in machine learning models and the systems used to train and deploy them.

I write here mostly to learn.

* Website
* GitHub
* LinkedIn