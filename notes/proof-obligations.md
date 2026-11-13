# Proof audit — working draft

Status categories: **PROVED IN DRAFT** means the argument is written here but awaits independent checking; **FROM LITERATURE** means the cited hypotheses must be verified against the exact primary statement; **OPEN** means the manuscript must not claim this conclusion unconditionally.

| Obligation | Status | Location / precise check |
| --- | --- | --- |
| Common invariant \(\pi\) for each subspace-dependent Gaussian random-walk kernel | FROM LITERATURE | Symmetric MH and \(\Sigma(\Gamma,W)\) |
| Condition (M) implies uniform minorization/drift on compact covariance-map images | FROM LITERATURE | A&M Proposition 12; verify compact image of \(\Sigma(\Gamma,W)\) |
| Lipschitz continuity of Gaussian proposal kernels in both \(\Gamma\) and \(W\) | FROM LITERATURE | A&M Lemma 13 composed with the smooth covariance map; check weighted norm and scale |
| Local \(V^\beta\) regularity of enlarged \(H\) | PROVED IN DRAFT | Lemma in Section 4, polynomial expansion |
| Poisson existence and Lipschitz regularity | FROM LITERATURE | A&M Proposition 3, hypotheses A1 AND A2 for Lipschitz conclusion |
| Polar retraction has a global quadratic remainder | PROVED IN DRAFT | Section 5, proof split into small and large tangent increments |
| Summability of geometric perturbations | PROVED IN DRAFT | Stopped moment estimates + square-summable steps |
| Weighted cumulative Markov noise convergence | PROVED IN DRAFT | Section 5, Appendix A; verify localization indicators, endpoint indexing and initial moments by hand |
| Euclidean ODE tracking for full recursion | PROVED IN DRAFT | Section 5, standard discrete Grönwall / APT theorem |
| A&M Lyapunov drift identity | PROVED IN DRAFT | Section 6; rederive from (52), do not mechanically rely on printed expanded (53) |
| Compact sublevels, uniform eigenvalue bounds | PROVED IN DRAFT | Section 6, eigenvalue transform and Rayleigh--Ritz |
| Joint reconstruction-error Lyapunov identity | PROVED IN DRAFT | Section 6; differentiate \(\mathcal R(\mu,W)=\tfrac12\pi[\|P_W(X-\mu)\|^2]\) in both \(\mu\) and \(W\), and verify global strictness for any \(\lambda>0\) |
| Finite Lyapunov critical values and ICT theorem | FROM LITERATURE | Benaïm 1999 Theorem 5.7 and Proposition 6.4 |
| Conditional almost-sure convergence to invariant-subspace set | PROVED IN DRAFT | Section 7; verify the localized path argument under chosen filtration |
| Finite number of reinitializations for the feedback-coupled algorithm | OPEN | Requires manifold-compatible A&M random truncation, W-dependent kernel control and exact reset map |
| Unconditional convergence of untruncated algorithm | OPEN | Needs stochastic stability/eventual compactness |
| Almost-sure selection of dominant principal subspace | OPEN | Needs avoidance of unstable equilibria/non-degenerate noise assumptions |
| ArXiv readiness | OPEN | Independent proof and citation audit; source build and review of claims |

## Hand-check order

1. Reproduce both gradients of the reconstruction-error functional and the exact three-square dissipation identity in Section 6 without reference to this draft.
2. Check the stopped weighted Poisson decomposition term by term in Appendix A.
3. Verify hypotheses and exact theorem numbering in A&M and Benaïm.
4. Check the feedback-coupled kernel estimates and decide whether to close the random-truncation stability argument before posting.
5. Review the final rendered PDF and compare mathematical line breaks with the source.
