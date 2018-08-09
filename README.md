* latexdiff AMS tool

This script creates a pdf with the differences between two AMS latex
.tex articles marked up. The main work is done by
[latexdiff](https://github.com/ftilmann/latexdiff). However, latexdiff
does not mark-up changes in the abstract of AMS articles because they
are contained in the latex header inside a separate \abstract command.

usage: `./latexdiffAMS old_article.tex new_article.tex diff.pdf`

dependencies: pdflatex, bibtex, latexdiff, pdftk, sed



