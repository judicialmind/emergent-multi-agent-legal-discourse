Submission Package
=========================

Title: Emergent Specialization in Autonomous Multi-Agent Legal Discourse
       Six Empirical Findings from a 150-Turn Conversation Among Five Frontier Models

Author: Surya Saka
Affiliation: JudicialMind, India
Email: hello@judicialmind.ai

Files:
  main.tex         - LaTeX source (acmart sigconf, nonacm=true)
  main.bbl         - Compiled bibliography
  references.bib   - BibTeX database (17 entries)
  figures/         - All 34 figures (PDF + PNG)

Compilation:
  pdflatex main.tex
  bibtex main
  pdflatex main.tex
  pdflatex main.tex

Dependencies:
  acmart (document class)
  booktabs, amsmath, amssymb, graphicx, hyperref, url, xcolor,
  microtype, enumitem, multirow

Notes:
  - All fonts are embedded (Type 1 and CID TrueType)
  - No external dependencies beyond standard TeX Live
  - Figures are in PDF format (vector graphics)
  - Bootstrap statistics computed with B=10,000, seed 0
