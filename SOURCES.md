# Source Index

**Hongru Zhao · Updated October 1, 2026 (UTC)**

Primary sources for the [research narrative](README.md) and [dated chronology](CONCURRENT_TIMELINE.md). PDF locators refer to the specified versions.

## Complex-Gaussian result and verification

| Source | Date / version | Locator and purpose |
| --- | --- | --- |
| Zhao, [Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry — arXiv:2610.00112](https://arxiv.org/abs/2610.00112) | v1 submitted **September 9, 2026, 07:19:22 UTC**; publicly available **October 1, 2026 (US Eastern)** | Public title, sole author Hongru Zhao, 39 pages, math.PR / quant-ph, and original v1 submission history. Public access was checked October 2 UTC, still October 1 in US Eastern. The exact announcement timestamp is not separately displayed on the abstract page. |
| [arXiv availability and announcement schedule](https://info.arxiv.org/help/availability.html) | Current guidance checked October 2, 2026 (UTC) | Announcement times use US Eastern: October 1 at 20:00 EDT corresponds to October 2 at 00:00 UTC. Identifiers are assigned in the month of first announcement; submission dates can precede announcement dates. |
| [Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry](https://zenodo.org/records/22856033) | September 20, 2026; manuscript v1.0.0 | [Main article](https://zenodo.org/records/22856033/files/main.pdf): Theorem 2.1, p. 4; Theorem 2.2, p. 5; Corollary 2.4, p. 6. |
| [Supplementary proofs](https://zenodo.org/records/22856033/files/supplement.pdf#page=24) | Same deposit | Section S9.1, p. S24: fixed-$n$ symmetric Gaussian limit, normalization, and disk-probability transfer. |
| [Manuscript metadata](https://zenodo.org/records/22856033) | Publication September 20; record created 09:41:35 UTC | Separate manuscript release from the Lean release dates. |
| [Lean verification v1.0.0](https://zenodo.org/records/22102635) | Publication field August 25; public release September 1 | Earlier *Shifted Anticoncentration* title; [metadata](https://zenodo.org/records/22102635) records creation September 1 at 06:30:38 UTC. |
| [Lean verification v1.1.0](https://zenodo.org/records/22554594) | September 6, 2026 | Successor under the *Local Anticoncentration* title; [metadata](https://zenodo.org/records/22554594) records creation at 23:29:30 UTC. |
| [ComplexGramHafnians](https://github.com/HongruZhao/ComplexGramHafnians) | Development repository; archive snapshot `95ab10d` | [Specification](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/Challenge.lean), [comparison](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/docs/PAPER_COMPARISON.md), and [recorded build and axiom audit](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md). Revised `theorem2_3` corresponds to deposited Theorem 2.2. |

## Submission policy — separate from the manuscript chronology

| Source | Effective date | Locator and purpose |
| --- | --- | --- |
| [arXiv: Fair Moderation, Equitable Access, and AI: arXiv's Updated Rate Limit Policy](https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/) | **October 1, 2026** | Announcement and full FAQ: two submissions per calendar month per submitter, across all categories; three total active submissions at any time, a limit in place since 2024; coauthors may coordinate submissions, with only the submitting account affected. |
| [arXiv moderation: submission rate](https://info.arxiv.org/help/moderation/index.html#submission-rate) | Current policy checked October 2, 2026 (UTC) | States the monthly and active limits and links the announcement. arXiv may also require a particular author to further limit their submission rate. |

The October 1 policy update is recorded for context. It does not establish the cause of the manuscript's September moderation hold.

## Companion papers and historical background

| Source | Submission / publication | Locator and purpose |
| --- | --- | --- |
| Hamilton, Kruse, Sansoni, Barkhofen, Silberhorn, and Jex, [Gaussian Boson Sampling](https://doi.org/10.1103/PhysRevLett.119.170501) | PRL **119**, 170501 (2017); [arXiv v1 December 4, 2016](https://arxiv.org/abs/1612.01199) | [v2 PDF, p. 3](https://arxiv.org/pdf/1612.01199v2#page=3): “Approximate GBS” discussion after Eq. (11). Historical motivation for the question. |
| Ehrenberg, Iosue, Deshpande, Hangleiter, and Gorshkov, [Transition of Anticoncentration in Gaussian Boson Sampling](https://arxiv.org/abs/2312.08433) | v1 December 13, 2023, 19:00:00 UTC; [PRL **134**, 140601, April 8, 2025](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.134.140601) | [Supplement §S5.B, pp. 16–17](https://arxiv.org/pdf/2312.08433#page=16): Eqs. (S61)–(S62), weak-anticoncentration transfer and quantitative hiding conjecture. |
| Same authors, [The Second Moment of Hafnians in Gaussian Boson Sampling](https://arxiv.org/abs/2403.13878) | v1 March 20, 2024, 18:00:00 UTC; [PRA **111**, 042412, April 8, 2025](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.111.042412) | Moment recursion; [Conjecture 2, PDF p. 12](https://arxiv.org/pdf/2403.13878#page=12), weak anticoncentration in the conjectured hiding regime. |
| Gorshkov, [IMSI talk: Anticoncentration and Entanglement in Gaussian Boson Sampling](https://www.imsi.institute/videos/anticoncentration-and-entanglement-in-gaussian-boson-sampling/) | September 16, 2024 | Talk and linked slides; my inspiration for the moment problem. |
| Koehler and Leung, [Anticoncentration of the Permanent in Ginibre Ensembles](https://arxiv.org/abs/2607.20329) | v1 July 22, 2026, 16:15:28 UTC | [Theorem 1.1, p. 2](https://arxiv.org/pdf/2607.20329v1#page=2), and comparison method; methodological source acknowledged in my complex manuscript. |
| Zhao, [Exact Moments of Gaussian Gram Hafnians Reveal an n²/log n Threshold for Weak Anticoncentration](https://arxiv.org/abs/2608.17065) | v1 August 17, 2026, 19:12:22 UTC | Earlier complex-Gram moment and weak-threshold result. |
| Shou, Ehrenberg, Wang, Iosue, and Gorshkov, [Anticoncentration and entanglement in Gaussian boson sampling](https://arxiv.org/abs/2609.01241) | v1 August 27, 2026, 17:55:00 UTC | [p. 2, Theorem 2.1](https://arxiv.org/pdf/2609.01241v1#page=2); [p. 14, AI acknowledgments](https://arxiv.org/pdf/2609.01241v1#page=14); [p. 15, Note added](https://arxiv.org/pdf/2609.01241v1#page=15), independent Zhao moment result. |
| Zhao, [Uniform Hiding of Haar Block Transpose Gram Matrices](https://arxiv.org/abs/2609.01008v1) | v1 September 1, 2026, 09:55:29 UTC | [Actual v1 PDF p. 22, reference [13]](https://arxiv.org/pdf/2609.01008v1#page=22): *Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry*. |
| Zhao, [Two Routes from Additive to Relative Accuracy in Gaussian Boson Sampling](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf) | Separate September 1, 2026 submission **7994183**; author-supplied five-page copy | **Eq. (4), p. 1**: finite complex Gram bound. **Eq. (8), p. 2**: independent circular complex symmetric bound, citing **Theorem I.3 of ref. [8]**, proof Appendix D. **Refs. [7]–[8], p. 4**: hiding and complex-anticoncentration companions. |
| [Two Routes Lean verification archive](https://zenodo.org/records/22102501) | v1.0.0; record created **September 1, 2026, 05:02:29 UTC** | `EQUATION_LEAN_CROSSWALK.md`, row 8, `eq:symmetric-anticoncentration`; bundled independent symmetric package, `VERIFICATION/public_axioms.log`: `symmetricHafnian_shifted_smallBall`, standard Lean foundations only. The combined archive preserves two separately verified packages. |
| Zhao, [Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling](https://arxiv.org/abs/2609.01008v2) | v2 September 11, 2026, 07:30:07 UTC; combines hiding v1 with the separate September 1 Two Routes manuscript | [Theorem 2.1 and Corollary 2.2, p. 3](https://arxiv.org/pdf/2609.01008v2#page=3), resolve the quantitative product-hiding conjecture in Supplemental Eq. (S62). [§3.1, p. 4](https://arxiv.org/pdf/2609.01008v2#page=4), Eqs. (3.2), (3.4); [Theorem 3.1, p. 5](https://arxiv.org/pdf/2609.01008v2#page=5), finite-Haar small-ball transfer; Theorem 3.2, p. 6; [p. 48, ref. [12]](https://arxiv.org/pdf/2609.01008v2#page=48), complex companion. Eq. (3.4) carries forward Two Routes Eq. (8). |
| Zhao, [Shifted Anticoncentration for Real Gram Hafnians and Symmetric Gaussian Hafnians](https://arxiv.org/abs/2609.06526) | v1 September 6, 2026, 10:47:33 UTC | Later real-Gaussian paper cited by the catalog. |
| [RealGramHafnians](https://github.com/HongruZhao/RealGramHafnians) and [real Lean archive](https://zenodo.org/records/22498111) | v1.1.0, September 6, 2026 | Verification materials for the real Gram and real symmetric theorems. |

## Later complex papers

| Source | Date | Locator and purpose |
| --- | --- | --- |
| Zhang, [Anticoncentration of Independent Complex Gaussian Hafnians](https://yuxuanzhang1995.github.io/agentic-research/complex-gaussian-hafnian/) | Prepared September 20, 2026 | Credits Koehler–Leung, Zhao real and weak Gram papers; target links the QIQCOP entry. |
| [Original Zhang site commit](https://github.com/yuxuanzhang1995/yuxuanzhang1995.github.io/commit/9ba4cd37740c3ec9e88895a0e994dd3087b0d5ac) | September 21, 00:50:33 UTC; September 20 in Chicago | First committed page; front matter dates preparation September 20. |
| Pant, [Anticoncentration of Complex Gaussian Hafnians](https://arxiv.org/abs/2609.35019) | v1 September 28, 2026, 12:18:39 UTC | [p. 2, Theorem 1.1](https://arxiv.org/pdf/2609.35019v1#page=2); [p. 3, concurrent-work acknowledgment](https://arxiv.org/pdf/2609.35019v1#page=3); [p. 15, ref. [9]](https://arxiv.org/pdf/2609.35019v1#page=15), Zhao's combined hiding paper. Citation chain: [hiding v2 Eq. (3.4)](https://arxiv.org/pdf/2609.01008v2#page=4) → complex companion [Theorem 2.2 / Corollary 2.4](https://zenodo.org/records/22856033). |

## Established terminology

| Source | Locator and scope |
| --- | --- |
| Quesada, Arrazola, and Killoran, [Gaussian Boson Sampling Using Threshold Detectors](https://doi.org/10.1103/PhysRevA.98.062322) (2018) | [§IV, PDF p. 3](https://arxiv.org/pdf/1807.01639#page=3), explicitly names the Hafnian-anti-concentration conjecture. |
| Deshpande et al., [Quantum Computational Advantage via High-Dimensional Gaussian Boson Sampling](https://doi.org/10.1126/sciadv.abi7894) (2022) | Discussion, point 2; [arXiv PDF p. 11](https://arxiv.org/pdf/2102.12474#page=11), GBS anticoncentration and additive-to-multiplicative approximation. |
| Li et al., [A Complexity Transition in Displaced Gaussian Boson Sampling](https://doi.org/10.1038/s41534-025-01062-5) (2025) | Conjecture 5, Eq. (24), loop-hafnian anticoncentration with displacement; a different ensemble. |

## Catalog and public correction

| Source | Date | Purpose |
| --- | --- | --- |
| [QIQCOP: Anticoncentration of independent complex Gaussian hafnians](https://qiqc-op.com/problem/op_55be40726cdf7304/) | Created September 10, 2026; latest displayed edit September 25 | Exact ensemble, root-mean-square normalization, and quantified lower-tail statement; displays “Unsolved” as of September 30. |
| [Quantum-open-problems issue #92](https://github.com/Naixu-Guo/quantum-open-problems/issues/92) | Created September 21, 2026 | Another candidate report concerning the independent-complex problem. |
| [My correction comment](https://github.com/Naixu-Guo/quantum-open-problems/issues/92#issuecomment-5917023518) | September 30, 2026, 18:12:56 UTC | Complex manuscript, Theorem 2.2 / Corollary 2.4, polynomial, and revised Lean numbering. |

My arXiv submission and administrative events are recorded in the [chronology](CONCURRENT_TIMELINE.md). The numbered receipts describe the August 26 / September 1 stage under 7994335 and the new September 9 stage under 8055779.

Receipt images in this repository: [September 1, 7994335](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-01-7994335.png) · [September 9, 8055779](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-09-8055779.png).

Additional retained records for *Two Routes*: the **7994183** acknowledgment prints **September 1, 2026, 00:39:01 EST**, identifies **five pages and one figure**, and names the independent complex symmetric reference in its abstract. The Overleaf history screenshot shows the titled project on **September 1**, with a **6:28 am** entry adding `main.tex`, `references.bib`, and the figure. These are displayed times from my records, distinct from the linked public archive's UTC timestamp.
