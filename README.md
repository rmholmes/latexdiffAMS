# latexdiff AMS tool

This script creates a pdf with the differences between two AMS latex
.tex articles marked up. The main work is done by
[latexdiff](https://github.com/ftilmann/latexdiff). However, latexdiff
does not mark-up changes in the abstract of AMS articles because they
are contained in the latex header inside a separate `\abstract`
command/environment.

**usage:** `./latexdiffAMS old_article.tex new_article.tex diff.pdf`

**dependencies:** pdflatex, bibtex, latexdiff, pdftk, sed

**Not yet implemented:**

- The formatting of the abstract doesn't quite match the AMS style
  (yet - should be easy).
- Currently the script assumes that the abstract pdf takes up only one
  page. Potentially fixable by looking for almost empty pdf pages?
- This script will only work if there is nothing between the end of
  the abstract and the `\begin{document}` command.

**testing:**

`./latexdiffAMS test_old.tex test_new.tex test_diff.pdf`

