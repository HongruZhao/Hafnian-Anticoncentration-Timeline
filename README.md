# Hafnian Anticoncentration Timeline

**Hongru Zhao · Updated September 30, 2026**

A chronology of my complex-Gaussian hafnian anticoncentration work, its Lean releases, and its companion papers, with links to the earlier moment literature and the exact independent-complex-Gaussian lower-tail problem.

**The September 20, 2026 manuscript resolves the polynomial lower-tail statement for independent circular complex symmetric Gaussian hafnians.** [Theorem 2.2 and Corollary 2.4](https://zenodo.org/records/22856033/files/main.pdf#page=5) give the explicit polynomial $p(n,1/\delta)=2n/\delta$.

[Read the full chronology](CONCURRENT_TIMELINE.md) · [Browse the source index](SOURCES.md) · [Manuscript archive](https://zenodo.org/records/22856033) · [Lean archive](https://zenodo.org/records/22554594)

## The result and the exact problem

Let $S=S^{\mathsf T}\in\mathbb C^{2n\times2n}$ have zero diagonal and independent entries above the diagonal, each with density $\pi^{-1}e^{-|z|^2}$. Write

$$
h_n=(2n-1)!!,\qquad H_n=\operatorname{haf}(S),
\qquad \mathbb E|H_n|^2=h_n.
$$

For every $n\ge1$, center $z\in\mathbb C$, and $\varepsilon\ge0$, Theorem 2.2 gives

$$
\Pr\!\left[|H_n-z|\le\varepsilon\sqrt{h_n}\right]
\le \min\{1,b_n\varepsilon^2\},
\qquad
b_n=\frac{2\Gamma(n+1/2)}{\sqrt{\pi}\,\Gamma(n)}
\le 2\sqrt{n/\pi}.
$$

The paper uses independent variance-two Gaussian diagonal entries; changing those entries to zero leaves the ordinary hafnian unchanged. Thus its theorem applies to the ensemble in [QIQCOP problem op_55be40726cdf7304](https://qiqc-op.com/problem/op_55be40726cdf7304/).

Set $z=0$ and $\varepsilon=\delta/(2n)$. Since $b_n\le2n$, for every $0<\delta<1$,

$$
\Pr\!\left[
|H_n|<\frac{\sqrt{h_n}}{p(n,1/\delta)}
\right]
\le \frac{\delta^2}{2n}<\delta,
\qquad p(n,u)=2nu.
$$

This supplies one polynomial, positive on $[1,\infty)^2$, for all $n$ and $\delta$, including the strict inequality required by the catalog. See [Corollary 2.4, page 6](https://zenodo.org/records/22856033/files/main.pdf#page=6).

## From finite transpose-Gram matrices to the independent ensemble

The proof first establishes a bound for $\operatorname{haf}(X^{\mathsf T}X)$, where $X\in\mathbb C^{k\times2n}$ has independent standard circular complex Gaussian entries. The finite theorem assumes $n\ge1$ and $k\ge4n$; its explicit coefficient is polynomial in the regime $n^2/k=O(\log n)$.

For the independent symmetric theorem, the paper fixes $n$ and lets $k\to\infty$. The matrix $k^{-1/2}X^{\mathsf T}X$ converges in distribution to the symmetric Gaussian model. Hafnian homogeneity scales the amplitude by $k^{-n/2}$; the exact second moment fixes the limiting normalization. The coefficient and normalized disk estimates then pass to the limit. [Supplementary Section S9.1, page S24](https://zenodo.org/records/22856033/files/supplement.pdf#page=24) gives this argument.

These are local small-ball bounds at every center and radius. They control lower tails beyond the weak-anticoncentration conclusions obtained from moments.

## Chronology at a glance

| Date | Event |
| --- | --- |
| 2017 | Hamilton et al. discuss hafnian anticoncentration after Eq. (11) of *Gaussian Boson Sampling*. |
| December 2023 / March 2024 | Ehrenberg, Iosue, Deshpande, Hangleiter, and Gorshkov submit the transition and second-moment papers; both appear in journals on April 8, 2025. |
| August 17, 2026 | My weak-anticoncentration moment paper, arXiv:2608.17065, is submitted. |
| August 25–26 | I complete Lean v1.0.0 on August 25 and initially submit the complex manuscript on August 26 as 7994335. |
| August 27 | Shou, Ehrenberg, Wang, Iosue, and Gorshkov submit the closed-form moment paper; its Note added acknowledges my independent weak-threshold work. |
| September 1 | Updated complex submission 7994335; public Lean v1.0.0 release; hiding v1 cites the complex companion on page 22, reference [13]. |
| September 4 | I request removal of 7994335 and 7994183 to reorganize the work. |
| September 6 | Real-Gaussian paper submitted; complex Lean v1.1.0 released. |
| September 8–9 | Removal confirmed September 8; new complex submission 8055779 acknowledged September 9. |
| September 10–11 | QIQCOP creates its entry; hiding v2 cites the *Local Anticoncentration* title on page 48, reference [12], and develops two relative-accuracy routes. |
| September 17–20 | arXiv confirms 8055779 is on hold; I publicly release the manuscript on Zenodo September 20. |
| September 30 | I post the correction comment; my dashboard still shows 8055779 on hold. |

The [full chronology](CONCURRENT_TIMELINE.md) gives the UTC timestamps, manuscript titles, and sources. My submission and administrative dates come from my retained arXiv records. I completed Lean v1.0.0 on August 25, the date listed in Zenodo's publication field, and publicly released it on September 1.

## Lean verification materials

The [ComplexGramHafnians repository](https://github.com/HongruZhao/ComplexGramHafnians) provides the Gaussian-model specifications and proofs, and the Zenodo releases preserve versioned verification materials.

| September 20 main article | Revised Lean declaration |
| --- | --- |
| Theorem 2.1: finite complex transpose-Gram bound | `ComplexGramHafnians.theorem2_1` |
| Theorem 2.2: independent complex symmetric bound | `ComplexGramHafnians.theorem2_3` |

The recorded September 6 build succeeded, and the two public declarations' recorded dependency audit lists exactly `propext`, `Classical.choice`, and `Quot.sound`. The [verification record](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md) and [paper-to-code comparison](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/docs/PAPER_COMPARISON.md) provide the details.

## Companion application and catalog record

[Section 3 of hiding v2](https://arxiv.org/pdf/2609.01008v2#page=4) combines finite-Gram or independent-symmetric small-ball bounds with hiding. Theorem 3.1 transfers lower tails to finite interferometers; Theorem 3.2 combines them with an assumed additive-estimation guarantee for two routes to relative accuracy. Local anticoncentration is the Gaussian input to those routes. Additive estimation and average-case computational hardness remain separate inputs to a full GBS hardness argument.

As of September 30, the [QIQCOP entry](https://qiqc-op.com/problem/op_55be40726cdf7304/) still displays “Unsolved” and cites my real-Gaussian paper. My [September 30 correction comment](https://github.com/Naixu-Guo/quantum-open-problems/issues/92#issuecomment-5917023518) points to the complex theorem and corollary. Issue #92 is another candidate report in that discussion.
