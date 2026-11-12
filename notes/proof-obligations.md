# Proof audit — working draft

Status categories: **PROVED IN DRAFT** means the argument is written here but awaits independent checking; **FROM LITERATURE** means the cited hypotheses must be verified against the exact primary statement; **OPEN** means the manuscript must not claim this conclusion unconditionally.

| Obligation | Status | Location / precise check |
| --- | --- | --- |
| Common invariant \(\pi\) for each Gaussian random-walk kernel | FROM LITERATURE | A&M Section 6 and MH detailed balance |
| Condition (M) implies uniform minorization/drift on covariance compacts | FROM LITERATURE | A&M Proposition 12 |
| Lipschitz continuity of Gaussian proposal kernels | FROM LITERATURE | A&M Lemma 13, check scaling by \(\ell^2\) |
| Local \(V^\beta\) regularity of enlarged \(H\) | PROVED IN DRAFT | Lemma in Section 4, polynomial expansion |
| Poisson existence and Lipschitz regularity | FROM LITERATURE | A&M Proposition 3, hypotheses A1 AND A2 for Lipschitz conclusion |
| Polar retraction has a global quadratic remainder | PROVED IN DRAFT | Section 5, proof split into small and large tangent increments |
| Summability of geometric perturbations | PROVED IN DRAFT | Stopped moment estimates + square-summable steps |
| Weighted cumulative Markov noise convergence | PROVED IN DRAFT | Section 5, Appendix A; verify localization indicators, endpoint indexing and initial moments by hand |
| Euclidean ODE tracking for full recursion | PROVED IN DRAFT | Section 5, standard discrete Grönwall / APT theorem |
| A&M Lyapunov drift identity | PROVED IN DRAFT | Section 6; rederive from (52), do not mechanically rely on printed expanded (53) |
| Compact sublevels, uniform eigenvalue bounds | PROVED IN DRAFT | Section 6, eigenvalue transform and Rayleigh--Ritz |
| Composite Lyapunov strictness for sample-driven Oja | PROVED IN DRAFT | Section 6; perturbation is \(vv^\top\), not \(\Gamma-C\) |
| Finite Lyapunov critical values and ICT theorem | FROM LITERATURE | Benaïm 1999 Theorem 5.7 and Proposition 6.4 |
| Conditional almost-sure convergence to invariant-subspace set | PROVED IN DRAFT | Section 7; verify the localized path argument under chosen filtration |
| Finite number of reinitializations for the enlarged algorithm | OPEN | Requires manifold-compatible A&M Theorem 11 proof and exact reinitialization map |
| Unconditional convergence of untruncated algorithm | OPEN | Needs stochastic stability/eventual compactness |
| Almost-sure selection of dominant principal subspace | OPEN | Needs avoidance of unstable equilibria/non-degenerate noise assumptions |
| ArXiv readiness | OPEN | Independent proof and citation audit; source build and review of claims |

## Hand-check order

1. Reproduce Section 6's gradient calculation without reference to this draft.
2. Check the stopped weighted Poisson decomposition term by term in Appendix A.
3. Verify hypotheses and exact theorem numbering in A&M and Benaïm.
4. Decide whether the first posted manuscript should present a localized result or incorporate a full random-truncation stability extension.
5. Review the final rendered PDF and compare mathematical line breaks with the source.
