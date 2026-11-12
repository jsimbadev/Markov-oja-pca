# Online principal-subspace estimation with adaptive MCMC

This repository is a standalone mathematical research note on **Oja's online principal-subspace iteration driven by an adaptive Markov chain**.  It is based on the reusable [quarto-math-note](https://github.com/jsimbadev/quarto-math-note) workflow and is independent of other research projects.

**Manuscript status: first research draft.**  The main theorem proves convergence on **eventually compact** adaptive-parameter trajectories.  Extension to unconditional convergence requires proving finite reinitialization/stability for the enlarged mean--covariance--Stiefel recursion.  Leading-eigenspace selection is not claimed.  The complete verification checklist is in [notes/proof-obligations.md](notes/proof-obligations.md).

## Read the note

After GitHub Actions renders the manuscript, the current branch contains:

- [Rendered PDF](_output/index.pdf) — easiest to read on mobile.
- [Rendered HTML](_output/index.html).
- [Manuscript entrypoint](index.qmd), assembling the following sections:

1. Introduction and research question
2. Notation and conventions (separate PDF page)
3. Coupled adaptive MCMC--Oja recursion and mean field
4. Markov assumptions and Poisson regularity
5. Retraction and stochastic error accumulation
6. Lyapunov structure and composite energy
7. Localized convergence theorem
8. Interpretation and limitations

Appendix A details all four Poisson remainder estimates; Appendix B records the geometry and the invariant-subspace calculations.

## Working on the note

Requires Quarto CLI >=1.6, Python >=3.10, GNU Make and LuaLaTeX, or Docker Compose.  The source is Quarto and each section is independently editable.

~~~sh
make check-source
make preview
make pdf
make check
make arxiv
# Or use Docker without a host Quarto/TeX installation:
make USE_DOCKER=1 preview
~~~

The bibliography is in [references.bib](references.bib) and can be maintained with Zotero Better BibTeX auto-export.  Math macros live in [macros.tex](macros.tex); [mathjax-macros.html](mathjax-macros.html) is generated from them.

GitHub Actions renders and commits HTML and PDF after pushes to the manuscript branch.  The PDF is not presented as a peer-reviewed result or a ready-to-submit preprint until the audit is completed.
