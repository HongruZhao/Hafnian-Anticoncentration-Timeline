# Concurrent Timeline

**Hongru Zhao**  
**Last updated: September 30, 2026**

This note records the development, submission, and public release of my related work on hafnian anticoncentration and Gaussian boson sampling. It connects the complex-Gaussian manuscript, its Lean verification releases, the companion hiding paper, and the later real-Gaussian paper with the earlier moment literature.

My complex-Gaussian work preceded my real-Gaussian paper. The sequence begins with code completion on August 25 and an initial complex-Gaussian submission on August 26. It continues through an updated submission and public Lean release on September 1, a reorganized submission on September 9, and the public manuscript deposit on September 20.

The September 20 manuscript's **Theorem 2.2 and Corollary 2.4 resolve the exact independent circular complex symmetric Gaussian hafnian lower-tail statement** in [QIQCOP problem op_55be40726cdf7304](https://qiqc-op.com/problem/op_55be40726cdf7304/), with the polynomial $p(n,1/\delta)=2n/\delta$. The proof first treats finite Gaussian transpose-Gram hafnians under stated dimension hypotheses, then fixes $n$ and takes $k\to\infty$ after normalizing the matrix by $k^{-1/2}$. [The result in context](README.md#the-result-and-the-exact-problem) gives the ensemble, normalization, and lower-tail inequality.

All times below are UTC. Public papers, version histories, and archive metadata are linked at each entry and collected in the [source index](SOURCES.md). My submission acknowledgments, removal requests, and account-status dates come from my retained arXiv records. The development sequence and the contents of the earlier submitted manuscript are my account of the work.

## Chronology

### 2017: Hamilton et al. discuss hafnian anticoncentration

Craig S. Hamilton, Regina Kruse, Linda Sansoni, Sonja Barkhofen, Christine Silberhorn, and Igor Jex published **“Gaussian Boson Sampling”**, *Physical Review Letters* **119**, 170501 (2017). The “Approximate GBS” discussion after Eq. (11) addresses hafnian anticoncentration in relating additive and multiplicative approximation.

This is the historical setting for the question. The precise independent-entry ensemble and quantified lower-tail statement in the QIQCOP entry are a later catalog formulation. The entry's September 10, 2026 creation date is distinct from the historical question. The Hamilton et al. preprint first appeared on December 4, 2016; 2017 is its journal publication year.

Sources: [published paper](https://doi.org/10.1103/PhysRevLett.119.170501) · [arXiv history](https://arxiv.org/abs/1612.01199) · [PDF, page 3](https://arxiv.org/pdf/1612.01199v2#page=3).

### December 13, 2023: Anticoncentration transition

Adam Ehrenberg, Joseph T. Iosue, Abhinav Deshpande, Dominik Hangleiter, and Alexey V. Gorshkov submitted **“Transition of Anticoncentration in Gaussian Boson Sampling”**, arXiv:2312.08433, at **19:00:00 UTC**.

The paper develops a graph-theoretic framework for moments of the GBS distribution and studies the transition between regimes with and without weak anticoncentration as the number of squeezed inputs changes relative to the photon count.

Source: [arXiv record and submission history](https://arxiv.org/abs/2312.08433).

### March 20, 2024: Companion second-moment work

The same five authors submitted **“The Second Moment of Hafnians in Gaussian Boson Sampling”**, arXiv:2403.13878, at **18:00:00 UTC**.

The paper develops a recursive moment expression, evaluates it numerically exactly up to photon sector $2n=80$, and derives further analytical moment results and consequences for ideal linear cross-entropy benchmarking.

Source: [arXiv record and submission history](https://arxiv.org/abs/2403.13878).

### April 8, 2025: Journal publication of both moment papers

Both companion papers were published on **April 8, 2025**:

- **“Transition of Anticoncentration in Gaussian Boson Sampling”**, *Physical Review Letters* **134**, 140601. [Publisher record](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.134.140601).
- **“Second moment of Hafnians in Gaussian boson sampling”**, *Physical Review A* **111**, 042412. [Publisher record](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.111.042412).

Their moment-based weak-anticoncentration conclusions provide background for the later local small-ball problem. These journal dates follow the 2023 and 2024 initial arXiv submissions.

### August 17, 2026: My earlier weak-anticoncentration paper

I submitted **“Exact Moments of Gaussian Gram Hafnians Reveal an n²/log n Threshold for Weak Anticoncentration”**, arXiv:2608.17065. The public history records v1 at **19:12:22 UTC**.

This paper evaluates the second and fourth absolute moments of complex Gaussian Gram hafnians and identifies the scaling threshold for an inverse-polynomial weak-anticoncentration moment criterion. It is an earlier part of the research program; the subsequent complex-Gaussian manuscript develops local small-ball estimates.

Source: [arXiv record and submission history](https://arxiv.org/abs/2608.17065).

### August 25, 2026: Completion of Lean v1.0.0

I completed the first complex-Gaussian Lean verification release on **August 25**, and publicly released it on **September 1**.

The archive is **“Lean Verification for ‘Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry’”**, version **1.0.0**, DOI **10.5281/zenodo.22102635**. It contains verification code and supporting materials concerning conditional Wishart estimates and the complex symmetric Gaussian limit. The manuscript was distributed separately.

Zenodo lists **August 25** as its publication date. The archival record was created on **September 1 at 06:30:38 UTC**. These dates record different events in the release sequence.[^dates]

Sources: [Lean v1.0.0](https://zenodo.org/records/22102635) · [record metadata](https://zenodo.org/api/records/22102635).

### August 26, 2026: Initial complex-Gaussian submission

At **05:45:55 UTC**, arXiv acknowledged submission **7994335**, titled **“Shifted Anticoncentration of Complex Gaussian Transpose-Gram Hafnians via Conditional Wishart Geometry”**.

The acknowledgment describes an **18-page** manuscript and identifies the accompanying Lean archive, DOI 10.5281/zenodo.22102635. This is the earliest submission acknowledgment in my records for the complex-Gaussian manuscript.

### August 27, 2026: Related closed-form moment and weak-threshold result

Laura Shou, Adam Ehrenberg, Yu-Xin Wang, Joseph T. Iosue, and Alexey V. Gorshkov submitted **“Anticoncentration and entanglement in Gaussian boson sampling”**, arXiv:2609.01241. Its public v1 history records **17:55:00 UTC on August 27**, despite the September-formatted identifier.

Theorem 2.1 gives a closed form for $M_2(k,n)=\mathbb E|\mathrm{haf}(X^{\mathsf T}X)|^4$ and identifies the sharp scaling threshold $k$ of order $n^2/\log n$ for weak anticoncentration. Here “second moment” is the second moment of the squared hafnian magnitude, hence the fourth absolute moment of the amplitude.

The **Note added** acknowledges my independent work, arXiv:2608.17065, for the closed-form moment and the same weak-anticoncentration transition. This acknowledgment concerns the August 17 moment paper. The local, high-probability small-ball estimates in my complex-Gaussian companion address the lower-tail question.

Sources: [arXiv history](https://arxiv.org/abs/2609.01241) · [v1 PDF, Theorem 2.1, page 2](https://arxiv.org/pdf/2609.01241v1#page=2) · [Note added, page 15](https://arxiv.org/pdf/2609.01241v1#page=15).

### September 1, 2026: Updated complex submission, public Lean release, and hiding v1

An updated acknowledgment under **7994335** records the title **“Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry”** and a **22-page** manuscript. This follows the August 26 initial acknowledgment. The first Lean archive was publicly released on September 1.

I also submitted **“Uniform Hiding of Haar Block Transpose Gram Matrices”**, arXiv:2609.01008v1, at **09:55:29 UTC**, as recorded in its public history.

The actual **v1 PDF, page 22, reference [13]**, cites the complex-Gaussian companion under the *Shifted Anticoncentration* title. This version-specific citation documents the connection in the version submitted on September 1, before the September 20 Zenodo manuscript deposit.

Sources: [hiding submission history](https://arxiv.org/abs/2609.01008) · [v1 PDF, page 22](https://arxiv.org/pdf/2609.01008v1#page=22) · [Lean v1.0.0](https://zenodo.org/records/22102635).

### September 4, 2026: Removal request to reorganize the work

At **22:59:04 UTC**, I asked arXiv to remove submissions **7994335** and **7994183** so that I could merge, reorganize, and resubmit the work. Submission 7994183 was titled **“Two Routes from Additive to Relative Accuracy in Gaussian Boson Sampling”**.

The original complex submission was on hold. I requested removal to prepare the reorganized manuscripts, received confirmation on September 8, and submitted the revised complex manuscript on September 9 under a new identifier.

### September 6, 2026: Real-Gaussian paper and complex Lean v1.1.0

I subsequently developed the real-Gaussian results and submitted **“Shifted Anticoncentration for Real Gram Hafnians and Symmetric Gaussian Hafnians”**, arXiv:2609.06526. Its public v1 history records **10:47:33 UTC on September 6**, after the initial complex-Gaussian submission.

The complex verification archive was also updated to **version 1.1.0**, DOI **10.5281/zenodo.22554594**, under **“Lean Verification for ‘Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry’”**. Its record was created at **23:29:30 UTC**.

Zenodo identifies v1.1.0 as the successor to v1.0.0 under the earlier *Shifted Anticoncentration* title. The [ComplexGramHafnians repository](https://github.com/HongruZhao/ComplexGramHafnians) is the development location, and the Zenodo archives preserve versioned verification materials for the same complex-Gaussian project.

Sources: [real-Gaussian arXiv history](https://arxiv.org/abs/2609.06526) · [complex Lean v1.1.0](https://zenodo.org/records/22554594) · [record metadata](https://zenodo.org/api/records/22554594).

### September 8, 2026: Removal confirmed

At **12:17:38 UTC**, arXiv confirmed removal of **7994335** and **7994183** in response to my September 4 request.

### September 9, 2026: New complex-Gaussian submission

At **07:19:23 UTC**, arXiv acknowledged the new submission **8055779**, titled **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”**.

The acknowledgment describes a **39-page** manuscript whose abstract explicitly includes the independent complex symmetric Gaussian limit. Submission 7994335 and submission 8055779 are separate administrative stages: the former was removed, and the latter is the reorganized submission.

### September 10, 2026: QIQCOP entry created

The [QIQCOP entry](https://qiqc-op.com/problem/op_55be40726cdf7304/) was created on **September 10**, nine days after my updated September 1 submission and one day after the new September 9 acknowledgment.

The result resolving its anticoncentration statement was already in my September 1 submitted manuscript. The entry subsequently listed the problem as unsolved. As of September 30, the page's latest visible revision is dated **September 25**.

Source: [QIQCOP statement and edit log](https://qiqc-op.com/problem/op_55be40726cdf7304/).

### September 11, 2026: Hiding v2 and two relative-accuracy routes

I submitted arXiv:2609.01008v2 at **07:30:07 UTC**, under **“Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling”**.

The actual **v2 PDF, page 48, reference [12]**, cites **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”**. Section 3 combines the companion's finite-Gram and independent-symmetric small-ball bounds with hiding and an assumed additive-estimation guarantee to obtain two routes to relative-probability accuracy.

The reference changes from **[13], page 22, in v1**, under the earlier title, to **[12], page 48, in v2**, under the *Local Anticoncentration* title. Both citations concern the same complex-Gaussian project.

Sources: [arXiv history](https://arxiv.org/abs/2609.01008) · [v2 PDF, Section 3, pages 4–6](https://arxiv.org/pdf/2609.01008v2#page=4) · [v2 PDF, page 48](https://arxiv.org/pdf/2609.01008v2#page=48).

### September 17, 2026: New submission confirmed on hold

arXiv support confirmed that **8055779** was on hold with the moderators and that no action was needed from me at that time. This status concerns the new September 9 submission.

### September 20, 2026: Public manuscript release

While submission **8055779** remained on hold, I deposited **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”** on Zenodo as manuscript **version 1.0.0**, DOI **10.5281/zenodo.22856033**. I made this public release because of the prolonged arXiv delay.

Zenodo lists **September 20** as the publication date and records creation at **09:41:35 UTC**. The deposit contains the **14-page main article** and **33-page supplement** and links the accompanying Lean archive and repository.

**Theorem 2.1**, on page 4 of the main article, treats finite complex Gaussian transpose-Gram hafnians for $n\ge1$ and $k\ge4n$. **Theorem 2.2**, on page 5, treats independent complex symmetric Gaussian hafnians for every $n\ge1$. Its proof in **Supplementary Section S9.1, page S24**, fixes $n$, normalizes $X^{\mathsf T}X$ by $k^{-1/2}$, and passes the finite small-ball bound to the Gaussian limit.

**Corollary 2.4**, on page 6, supplies $p(n,1/\delta)=2n/\delta$ for the exact QIQCOP lower-tail statement. The diagonal variance convention in the paper does not affect the ordinary hafnian, so it also covers the catalog's zero-diagonal ensemble.

The manuscript's v1.0.0 and the Lean archive's v1.0.0 are version labels for separate artifacts with separate release dates.

Sources: [manuscript archive](https://zenodo.org/records/22856033) · [main article, pages 4–6](https://zenodo.org/records/22856033/files/main.pdf#page=4) · [supplement, page S24](https://zenodo.org/records/22856033/files/supplement.pdf#page=24) · [record metadata](https://zenodo.org/api/records/22856033).

### September 30, 2026: Public correction comment and current arXiv status

At **18:12:56 UTC**, I posted a comment in the quantum-open-problems discussion identifying the September 20 manuscript, its independent complex-Gaussian theorem and corollary, and the verification materials. I asked the maintainers to review the result, add the preprint to the progress record and references, and assess the entry's status and attribution.

The comment also explains the numbering: **Theorem 2.2 in the September 20 main article corresponds to revised Lean `theorem2_3`**. The [recorded September 6 verification](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md) reports a successful build and the exact standard-foundation dependencies for the finite and independent-symmetric declarations.

The comment is in **issue #92**, another candidate report concerning the catalog problem. The catalog still displays **“Unsolved”** as of September 30.

My arXiv dashboard still shows **8055779** as **on hold** on September 30. The earlier **7994335** was removed on September 8; the current hold belongs to the new submission acknowledged on September 9.

Sources: [public correction comment](https://github.com/Naixu-Guo/quantum-open-problems/issues/92#issuecomment-5917023518) · [QIQCOP entry](https://qiqc-op.com/problem/op_55be40726cdf7304/).

## How the companion results fit together

The hiding paper compares finite interferometer matrix laws with Gaussian reference laws. The complex-Gaussian companion controls how often their hafnians fall in a small disk around any prescribed center.

The two routes use different Gaussian references:

1. **Finite transpose-Gram route.** For a rectangular Gaussian matrix $G$, the reference $GG^{\mathsf T}$ retains dependence between entries. Uniform product hiding combines with the companion's local bound for this finite ensemble.
2. **Independent symmetric route.** The reference has independent complex Gaussian entries above the diagonal. A corresponding hiding estimate combines with the companion's bound for that symmetric ensemble.

In [Section 3 of hiding v2](https://arxiv.org/pdf/2609.01008v2#page=4), **Theorem 3.1** transfers these small-ball bounds to finite-interferometer lower tails. **Theorem 3.2** uses those tails with an assumed additive-estimation guarantee to obtain relative-accuracy bounds. The comparison uses the same estimator and absolute additive threshold and accounts for the different reference probability scales.

Local anticoncentration is a key mathematical input to these applications. The hiding and Gaussian small-ball proofs are developed separately. Their composition provides lower-tail and relative-accuracy guarantees in the stated regimes; additive estimation and average-case computational hardness remain separate inputs to a full GBS sampling-hardness argument.

## The submission and release sequence

The complex-Gaussian manuscript follows two arXiv submission stages:

**August 26 initial submission 7994335 → September 1 update → September 4 removal request → September 8 removal confirmed → September 9 new submission 8055779 → September 17 hold confirmed → September 20 public Zenodo release → September 30 still on hold.**

The public record also connects the project through the September 1 Lean archive and hiding-v1 citation, the September 6 Lean update, and the September 11 hiding-v2 citation. These dates place the September 20 deposit within the development and release sequence of the complex-Gaussian work.

[^dates]: Zenodo's publication-date field and record-created timestamp describe different events. For Lean v1.0.0, the [metadata](https://zenodo.org/api/records/22102635) gives `publication_date: 2026-08-25` and `created: 2026-09-01T06:30:38.827108+00:00`; my code-completion and public-release dates explain that distinction. arXiv history timestamps record submissions, which can precede public announcements.
