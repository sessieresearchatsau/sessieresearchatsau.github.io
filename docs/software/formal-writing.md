# Formal Writing Tools
**LaTeX, Overleaf, and JabRef** are standard tools for academic and technical writing. LaTeX handles structured typesetting for text, math, and references. Overleaf provides an online editor with real-time collaboration and version control. JabRef manages bibliographies in BibTeX format, keeping citations organized and consistent. Together, they provide a reliable workflow for producing publication-ready documents.

## LaTeX
LaTeX is a **document preparation system** widely used in academia, especially for scientific and technical writing. Unlike word processors (e.g., Microsoft Word), LaTeX focuses on **content and structure**, leaving formatting to predefined styles. It excels at typesetting **mathematics, bibliographies, and large documents** like theses or research papers.

- **Key Features:**
    - Professional-quality typesetting
    - Mathematical formulas and symbols
    - Automated numbering (sections, figures, tables, equations)
    - Bibliography and citation management
    - Cross-references and indexing

For instance,
```latex
\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}
```
will render
$$
\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}
$$

> NOTE: You can, of course, also include such LaTeX **expressions in markdown** using `$expression$` for inline expressions and `$$expression$$` for expression blocks. It is also helpful to know that Mathematica and RuleFlow support **exporting expressions as LaTeX** so that you can easily include such expressions in papers or documentation.

## Overleaf
Overleaf is a **cloud-based LaTeX editor** that allows you to write, edit, and collaborate on LaTeX documents directly in your browser. It removes the need to install LaTeX locally and provides real-time collaboration (like Google Docs for LaTeX).

- **Key Features:**
    - No installation required
    - Real-time collaboration
    - Rich template library (CVs, theses, journal submissions)
    - Integrated version control
    - Direct submission to some publishers

When you create a new project in Overleaf, simply focus on writing LaTeX and Overleaf will automatically compile it into a PDF (or other formats) for you. It is one of the de facto ways to write academic papers.

---

## JabRef
JabRef is an **open-source reference manager** that uses **BibTeX** as its native format. It integrates seamlessly with LaTeX, making it easy to manage bibliographies and citations.

- **Key Features:**
    - Import references from databases (DOI, ISBN, PubMed, arXiv)
    - Organize references with tags, keywords, and groups
    - Automatic metadata retrieval
    - Integration with LaTeX editors
    - File management (rename PDFs, link to entries)

This is what a citation looks like.
```bibtex
@article{einstein1905,
  author  = {Albert Einstein},
  title   = {On the Electrodynamics of Moving Bodies},
  journal = {Annalen der Physik},
  year    = {1905},
  volume  = {17},
  pages   = {891--921}
}
```

Each citation (like the above) is contained as plaintext in a `.bib` file that is managed by JabRef. In your LaTeX document you simply cite the name of the citation using `\cite{}` or `\footnote{}` and `\bibliography{references.bib}` at the end of the document.
```latex
\documentclass{article}
\usepackage{cite}

\begin{document}
Einstein’s work on relativity was groundbreaking \cite{einstein1905}.

\bibliographystyle{plain}
\bibliography{references} % references.bib file
\end{document}
```
This will result in a references page being automatically generated at the end of the document.

> NOTE: Using JabRef to log relevant research is the preferred way of keeping track of research/papers. Adding relevant work here on the docs site is also important (or links to `.bib` files).

## Additional Resources
- [Overleaf Learn Portal](https://www.overleaf.com/learn)
- [Overleaf Documentation](https://docs.overleaf.com/)
- [Learn LaTeX in 30 Minutes (Overleaf)](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)
- [JabRef Official Website](https://www.jabref.org/)
