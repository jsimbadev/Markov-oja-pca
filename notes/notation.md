# Internal notation ledger

The publishable notation page is Section 2 of the manuscript.  This ledger records a few distinctions to preserve while editing:

- \(\pi\) means target distribution, while \(m=\pi(x)\) and \(C\) denote target mean and covariance.
- \(\Gamma\) is the adaptive covariance, not the target covariance.
- \(V\) is the Markov drift function, never an EMA or a covariance.
- \(H\) is the ambient observable, \(h=\pi H\) the averaged field, and \(G\) its Oja component.
- \(u_\theta\) solves the Poisson equation; \(v_\theta=P_\theta u_\theta\).  Lowercase \(v=\mu-m\) is the mean error (distinguished by whether there is a subscript).
- \(B_C(W)=(I-WW^\top)CW\), and \(\mathcal E_C=\{W:B_C(W)=0\}\).
- The principal theorem concerns **sample-driven** Oja, not an iteration driven by \(\Gamma_n W_n\).
