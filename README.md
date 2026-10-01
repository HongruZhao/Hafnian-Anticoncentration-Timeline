# Research and Submission Timeline for Hafnian Anticoncentration

**Hongru Zhao · September 30, 2026**

## 2017–2025: The question and the moment literature

In 2017, Hamilton et al. discussed hafnian anticoncentration after Eq. (11) of [*Gaussian Boson Sampling*](https://doi.org/10.1103/PhysRevLett.119.170501). Their discussion connects additive and multiplicative approximation of hafnians and is an early source of the problem that motivated my work. The historical question predates its September 2026 entry in an open-problem catalog. [Hamilton et al., PDF p. 3](https://arxiv.org/pdf/1612.01199v2#page=3).

Adam Ehrenberg, Joseph T. Iosue, Abhinav Deshpande, Dominik Hangleiter, and Alexey V. Gorshkov subsequently developed the moment approach in [*Transition of Anticoncentration in Gaussian Boson Sampling*](https://arxiv.org/abs/2312.08433), submitted December 13, 2023, and [*The Second Moment of Hafnians in Gaussian Boson Sampling*](https://arxiv.org/abs/2403.13878), submitted March 20, 2024. Both appeared in journals on **April 8, 2025**: [PRL **134**, 140601](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.134.140601) and [PRA **111**, 042412](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.111.042412).

These papers are central background for my research. They study moments, the transition in weak anticoncentration, and the role of hiding in transferring Gaussian conclusions to physical Haar interferometers. The transition paper's Supplement §S5.B, particularly [Eqs. (S61)–(S62)](https://arxiv.org/pdf/2312.08433#page=16), explains that transfer. Weak anticoncentration gives an inverse-polynomial probability of an amplitude above a specified scale; a shrinking small-ball estimate controls the probability of being arbitrarily close to zero or another center.

My [*Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling*](https://arxiv.org/abs/2609.01008v2) resolves the quantitative product-hiding conjecture in Eq. (S62): **[Theorem 2.1 and Corollary 2.2, p. 3](https://arxiv.org/pdf/2609.01008v2#page=3)** give the conjectured quadratic scaling, uniformly over the number of squeezed inputs. Combined with my companion's Gaussian small-ball theorem, this hiding estimate transfers local anticoncentration to finite Haar interferometers, with the stated hiding error. **[Theorem 3.1, p. 5](https://arxiv.org/pdf/2609.01008v2#page=5)** gives that transfer explicitly.

## My starting point: the IMSI talk and the weak threshold

I was inspired by Alexey Gorshkov's IMSI talk, [*Anticoncentration and Entanglement in Gaussian Boson Sampling*](https://www.imsi.institute/videos/anticoncentration-and-entanglement-in-gaussian-boson-sampling/), delivered on September 16, 2024. It drew my attention to the Gaussian Gram hafnian moment problem and its weak-anticoncentration transition.

With assistance from ChatGPT using **GPT 5.6 Sol**, I worked out the exact moments and the weak threshold. I submitted [*Exact Moments of Gaussian Gram Hafnians Reveal an n²/log n Threshold for Weak Anticoncentration*](https://arxiv.org/abs/2608.17065) on **August 17, 2026**. This was my solution of the weak Gaussian Gram problem, based on the second and fourth absolute moments.

I contacted Alexey Gorshkov by email and learned that a member of his group had independently obtained the same moment and weak-threshold solution. We agreed to acknowledge the work as independent. Laura Shou, Adam Ehrenberg, Yu-Xin Wang, Joseph T. Iosue, and Alexey V. Gorshkov submitted [*Anticoncentration and Entanglement in Gaussian Boson Sampling*](https://arxiv.org/abs/2609.01241) on **August 27, 2026**. Its [Note added, p. 15](https://arxiv.org/pdf/2609.01241v1#page=15), acknowledges my independent result. Their [acknowledgments, p. 14](https://arxiv.org/pdf/2609.01241v1#page=14), disclose assistance from GPT 5.5 Thinking and Pro. I have also added a reciprocal acknowledgment to the version of my paper submitted to a journal.

## July 2026: The methodological breakthrough

Frederic Koehler and Pui Kuen Leung's [*Anticoncentration of the Permanent in Ginibre Ensembles*](https://arxiv.org/abs/2607.20329), submitted July 22, 2026, was a decisive methodological breakthrough for this line of work. Their Fourier coordinate-compression and Gaussian comparison methods gave me a route beyond moment-based weak anticoncentration. I regard this paper as a foundational source for my subsequent hafnian small-ball proofs. [Theorem 1.1 and the comparison framework](https://arxiv.org/pdf/2607.20329v1#page=2).

## August–September: My complex Gaussian small-ball result

While working on the weak moment problem, I also developed a direct local anticoncentration proof for **complex Gaussian transpose-Gram hafnians**, with assistance from **GPT 5.6 Sol in Ultra mode**. Building on Koehler and Leung's method, I had to handle the additional dependence in the Gram ensemble. The conditional Wishart geometry controls the relevant variance while preserving the transpose-Gram matrix and its dependent hafnian cofactors. The manuscript credits this methodological starting point explicitly. [Methods, §4.2](https://zenodo.org/records/22856033/files/main.pdf#page=9).

The proof first treats $\mathrm{haf}(X^{\mathsf T}X)$ for an independent circular complex Gaussian matrix $X\in\mathbb C^{k\times2n}$. The finite theorem assumes $n\ge1$ and $k\ge4n$; its explicit coefficient is polynomial when $n^2/k=O(\log n)$. I then fix $n$ and let $k\to\infty$ after normalizing the matrix by $k^{-1/2}$. This yields the independent circular complex symmetric Gaussian theorem. [Theorem 2.1, p. 4](https://zenodo.org/records/22856033/files/main.pdf#page=4) · [Theorem 2.2, p. 5](https://zenodo.org/records/22856033/files/main.pdf#page=5) · [Supplement §S9.1, p. S24](https://zenodo.org/records/22856033/files/supplement.pdf#page=24).

For a zero-diagonal symmetric matrix $S$ with independent standard circular complex Gaussian entries above the diagonal, put $h_n=(2n-1)!!$. For every $n\ge1$, $z\in\mathbb C$, and $\varepsilon\ge0$:

```math
\Pr\left[|\mathrm{haf}(S)-z|\le\varepsilon\sqrt{h_n}\right]
\le\min\left\lbrace 1,b_n\varepsilon^2\right\rbrace.
```

Here

```math
b_n=\frac{2\Gamma(n+1/2)}{\sqrt{\pi}\Gamma(n)}
\le2\sqrt{\frac{n}{\pi}}.
```

Setting $z=0$ and $\varepsilon=\delta/(2n)$ gives the polynomial **$p(n,1/\delta)=2n/\delta$** and failure probability at most $\delta^2/(2n)<\delta$ for $0<\delta<1$. This resolves the precise independent circular complex Gaussian lower-tail statement later cataloged by QIQCOP. [Corollary 2.4, p. 6](https://zenodo.org/records/22856033).

### Lean completion, submission receipts, and public release

The first release is preserved in the [Lean v1.0.0 Zenodo archive](https://zenodo.org/records/22102635).

<table>
<thead><tr><th>Event</th><th>Date</th></tr></thead>
<tbody>
<tr><td>I completed the Lean code</td><td>August 25, 2026</td></tr>
<tr><td>I publicly released the archive</td><td>September 1, 2026</td></tr>
<tr><td>Zenodo created the archive record</td><td>September 1, 2026, at 06:30:38 UTC</td></tr>
</tbody>
</table>

Zenodo lists August 25 as the publication date, matching the code-completion date.

My complex manuscript went through two arXiv submission stages:

| Date in 2026 | Submission or release |
| --- | --- |
| August 26 | Initial receipt for **7994335**: *Shifted Anticoncentration of Complex Gaussian Transpose-Gram Hafnians via Conditional Wishart Geometry*, 18 pages. |
| September 1 | Updated complex receipt **7994335**, 22 pages; separate *Two Routes* receipt **7994183**, five pages; hiding **2609.01008v1**; public complex and Two Routes Lean archives. |
| September 4 / 8 | I requested removal of 7994335 to reorganize the work while the original submission was on hold; arXiv confirmed removal September 8. |
| September 6 | Complex Lean **v1.1.0** released, with verification records for the finite Gram and independent complex symmetric bounds. |
| September 9 | New receipt for **8055779**, *Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry*, 39 pages. Its abstract explicitly states the independent complex symmetric Gaussian limit. |
| September 17 / 20 | arXiv confirmed 8055779 was on hold; I released the manuscript on [Zenodo](https://zenodo.org/records/22856033) September 20 because of the prolonged delay. |
| September 30 | My dashboard still showed **8055779** on hold. |

The original receipt images are linked here: [September 1 — 7994335](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-01-7994335.png) · [September 9 — 8055779](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-09-8055779.png). The [detailed chronology](CONCURRENT_TIMELINE.md) retains the UTC timestamps and the separate submission identifiers.

By **September 6**, [Lean v1.1.0](https://zenodo.org/records/22554594) provided the recorded successful build and dependency audit for the two headline complex-Gaussian declarations. Their dependencies are exactly `propext`, `Classical.choice`, and `Quot.sound`. In the revised [ComplexGramHafnians](https://github.com/HongruZhao/ComplexGramHafnians) code, `theorem2_1` corresponds to the finite Gram bound and `theorem2_3` to **Theorem 2.2** of the September 20 manuscript. [Verification record](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md) · [Paper-to-code comparison](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/docs/PAPER_COMPARISON.md).

### September 1: Two Routes and the independent complex theorem

I also submitted **[*Two Routes from Additive to Relative Accuracy in Gaussian Boson Sampling*](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf)** to arXiv on **September 1**, under temporary submission number **7994183**. My receipt identifies a five-page manuscript with one figure. My retained Overleaf history also shows a September 1 version of the project, including `main.tex`, `references.bib`, and the figure file.

The manuscript explicitly uses **both** Gaussian small-ball results. **Eq. (4), p. 1**, gives the finite complex transpose-Gram bound. **Eq. (8), p. 2**, gives the independent circular complex symmetric Gaussian bound, with the same coefficient $b_n$ displayed above. It cites **Theorem I.3 of reference [8]**, with the proof in Appendix D of the earlier complex companion. Reference [8], on p. 4, names *Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry*; reference [7] names the separate hiding manuscript. [Author-supplied manuscript, pp. 1–2 and 4](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf).

There is also a dated public verification record: the [Two Routes Lean v1.0.0 archive](https://zenodo.org/records/22102501) was created on **September 1 at 05:02:29 UTC**. Its `EQUATION_LEAN_CROSSWALK.md`, row 8 (`eq:symmetric-anticoncentration`), records the independent complex symmetric Gaussian theorem and its exact normalization and coefficient. The bundled companion's `VERIFICATION/public_axioms.log` records `symmetricHafnian_shifted_smallBall` with only `propext`, `Classical.choice`, and `Quot.sound` as dependencies. The downstream Haar and relative-accuracy applications retain their stated hiding and estimator inputs.

These records document the independent complex result in my September 1 work, before the September 10 catalog entry and the later Zhang and Pant manuscripts.

### September 11: Combining hiding v1 with Two Routes

My [hiding paper v1](https://arxiv.org/abs/2609.01008v1), submitted September 1, cites the complex companion under its *Shifted Anticoncentration* title in the **actual PDF, p. 22, reference [13]**. [Version-specific citation](https://arxiv.org/pdf/2609.01008v1#page=22).

I combined the September 1 hiding manuscript and the separate September 1 *Two Routes* manuscript in the September 11 revision, [*Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling*](https://arxiv.org/abs/2609.01008v2). **September 1 is v1; September 11 is v2.** The combined paper cites the *Local Anticoncentration* title in **p. 48, reference [12]**. Its **Eq. (3.2)** states the finite complex Gram small-ball input, and **Eq. (3.4)** states the independent complex symmetric Gaussian input carried forward from *Two Routes* Eq. (8). **Theorem 3.1**, “Two finite-interferometer lower tails,” transfers them to Haar interferometers. **Theorem 3.2** combines those tails with an assumed additive-estimation guarantee to obtain relative accuracy. [Gaussian inputs, p. 4](https://arxiv.org/pdf/2609.01008v2#page=4) · [Theorem 3.1, p. 5](https://arxiv.org/pdf/2609.01008v2#page=5) · [Theorem 3.2, p. 6](https://arxiv.org/pdf/2609.01008v2#page=6) · [Reference [12], p. 48](https://arxiv.org/pdf/2609.01008v2#page=48).

Thus the arXiv hold delayed the complex manuscript's visibility, while its Lean releases and the companion citation were already public. Hiding plus weak moments transfers weak anticoncentration; the local theorem supplies the additional input for shrinking small-ball bounds. Additive estimation and average-case hardness are further ingredients in a complete GBS sampling-hardness argument.

## September 6: The subsequent real Gaussian result

After developing the complex case, I completed the real case and submitted [*Shifted Anticoncentration for Real Gram Hafnians and Symmetric Gaussian Hafnians*](https://arxiv.org/abs/2609.06526) on **September 6, 2026**. I also began explaining the result to researchers in probability. Its **Theorem 2.1** concerns real Gram hafnians and **Theorem 2.3** independent real symmetric Gaussian hafnians. The verification materials are in [RealGramHafnians](https://github.com/HongruZhao/RealGramHafnians) and [Zenodo v1.1.0](https://zenodo.org/records/22498111).

This was a subsequent real result. The independent **complex** result belongs to my separate complex manuscript and its verification archive.

## September 10–28: The catalog and concurrent complex work

### The September 10 open-problem entry

[QIQCOP's independent complex Gaussian hafnian entry](https://qiqc-op.com/problem/op_55be40726cdf7304/) was created on **September 10**. I had already proved the resolving result in my manuscript submitted by September 1, with the two headline complex bounds recorded in the September 6 Lean release. The September 9 resubmission receipt also expressly states the independent complex limit.

The catalog's creation therefore followed my resolution; its “Unsolved” label did not reflect that work. The catalog correctly notes that the cited **real** paper, arXiv:2609.06526, does not state the circular complex theorem. The missing reference is my **complex companion**, whose [Theorem 2.2 and Corollary 2.4](https://zenodo.org/records/22856033) give the catalog's requested conclusion. The September 1 *Two Routes* manuscript already states the independent complex bound in **Eq. (8)**, and the [September 11 hiding v2, Eq. (3.4)](https://arxiv.org/pdf/2609.01008v2#page=4), makes that bound explicit on arXiv. On September 30 I posted [a correction identifying those sources](https://github.com/Naixu-Guo/quantum-open-problems/issues/92#issuecomment-5917023518).

### Yuxuan Zhang's September 20 manuscript

Yuxuan Zhang's [*Anticoncentration of Independent Complex Gaussian Hafnians*](https://yuxuanzhang1995.github.io/agentic-research/complex-gaussian-hafnian/) is dated September 20. It credits Koehler–Leung, my real paper, and my earlier weak complex Gram paper, but omits my complex local-anticoncentration companion, the separate *Two Routes* manuscript, and the combined hiding paper. Its descriptions of the two Zhao papers it cites are accurate for those papers. As an account of my earlier results, however, this leaves out the independent complex theorem that I had already obtained.

The omitted record is explicit: *Two Routes* **Eq. (8), p. 2**, the [September 1 verification archive](https://zenodo.org/records/22102501), and [hiding v2 **Eq. (3.4), p. 4**](https://arxiv.org/pdf/2609.01008v2#page=4) all concern the independent **circular complex** symmetric ensemble. The catalog's lower-tail conclusion follows from my complex companion's [**Theorem 2.2 and Corollary 2.4**](https://zenodo.org/records/22856033). An implication that my prior work had not resolved the complex case is therefore incorrect. **My dated record of this solution precedes both Zhang's September 20 manuscript and Pant's September 28 submission.**

### Priyanshu Pant's September 28 paper

Priyanshu Pant submitted [*Anticoncentration of Complex Gaussian Hafnians*](https://arxiv.org/abs/2609.35019) on September 28. Its introduction acknowledges concurrent Zhao work “including the complex symmetric Gaussian ensemble.” Reference [9] points to my **[*Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling*](https://arxiv.org/abs/2609.01008v2)**, the September 11 v2 combining my two September 1 manuscripts. Its [**Eq. (3.4), p. 4**](https://arxiv.org/pdf/2609.01008v2#page=4), states the independent complex bound and cites the complex companion; this is the same input already used in *Two Routes* **Eq. (8)**. My companion's [**Theorem 2.2 and Corollary 2.4**](https://zenodo.org/records/22856033) give the shifted theorem and the polynomial lower-tail consequence. Pant's Theorem 1.1 gives the same coefficient $b_n$ for the shifted small-ball bound; his paper also develops product-Gamma comparison and negative-moment results. [Theorem 1.1, p. 2](https://arxiv.org/pdf/2609.35019v1#page=2) · [Concurrent-work discussion, p. 3](https://arxiv.org/pdf/2609.35019v1#page=3) · [Reference [9], p. 15](https://arxiv.org/pdf/2609.35019v1#page=15).

## Terminology and attribution

**“Hafnian-anti-concentration conjecture” is an established name in the literature.** Quesada, Arrazola, and Killoran use it explicitly in §IV of [*Gaussian Boson Sampling Using Threshold Detectors*](https://doi.org/10.1103/PhysRevA.98.062322). [PDF p. 3](https://arxiv.org/pdf/1807.01639#page=3). Deshpande et al. discuss the GBS anticoncentration conjecture and its role in additive-to-multiplicative approximation in [*Quantum Computational Advantage via High-Dimensional Gaussian Boson Sampling*](https://doi.org/10.1126/sciadv.abi7894), Discussion, point 2. Li et al.'s [*A Complexity Transition in Displaced Gaussian Boson Sampling*](https://doi.org/10.1038/s41534-025-01062-5), Conjecture 5 and Eq. (24), concern **loop-hafnians with displacement**, a different setting.

Titles such as “independent complex Gaussian hafnians” identify a particular ensemble and can be natural descriptions of the same question. Zhang's page explicitly links the catalog as its target; similarity of titles alone does not establish how another author chose a problem or became aware of earlier work. My attribution rests on the dated submissions, releases, theorem statements, and citations recorded here.

[Full dated chronology](CONCURRENT_TIMELINE.md) · [Source index and exact locators](SOURCES.md)
