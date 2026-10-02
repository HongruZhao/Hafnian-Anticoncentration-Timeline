# Research and Submission Timeline for Hafnian Anticoncentration

**Update — October 1, 2026 (US Eastern): [arXiv:2610.00112](https://arxiv.org/abs/2610.00112) is now publicly available; submitted September 9, 2026.**

**Hongru Zhao**  
**Last updated: October 2, 2026 (UTC)**

This chronology follows the earlier literature, the talk that inspired me, my weak-anticoncentration solution, the complex and real small-ball results, and their submissions and releases. The [README](README.md) gives the research narrative; the [source index](SOURCES.md) supplies version-specific locators.

My complex-Gaussian work preceded my real-Gaussian paper. The sequence begins with code completion on August 25 and an initial complex-Gaussian submission on August 26. It continues through an updated submission and public Lean release on September 1, a reorganized submission on September 9, the public manuscript deposit on September 20, and public arXiv availability on October 1 (US Eastern).

Times are UTC unless an entry explicitly identifies another timezone or quotes a displayed time from my records. Public papers, version histories, and archive metadata are linked at each entry and collected in the [source index](SOURCES.md). My submission acknowledgments, Overleaf history, removal requests, and account-status dates come from my retained records.

## Chronology

### 2017: Hamilton et al. discuss hafnian anticoncentration

Hamilton et al. published **[“Gaussian Boson Sampling”](https://doi.org/10.1103/PhysRevLett.119.170501)** in 2017. Its discussion after Eq. (11) addresses hafnian anticoncentration and additive-to-multiplicative approximation.

The historical question predates the September 2026 catalog entry. The preprint first appeared December 4, 2016; 2017 is the journal year.

Sources: [published paper](https://doi.org/10.1103/PhysRevLett.119.170501) · [arXiv history](https://arxiv.org/abs/1612.01199) · [PDF, page 3](https://arxiv.org/pdf/1612.01199v2#page=3).

### December 13, 2023: Anticoncentration transition

Adam Ehrenberg, Joseph T. Iosue, Abhinav Deshpande, Dominik Hangleiter, and Alexey V. Gorshkov submitted **[“Transition of Anticoncentration in Gaussian Boson Sampling”](https://arxiv.org/abs/2312.08433)**, arXiv:2312.08433, at **19:00:00 UTC**.

The paper studies the weak-anticoncentration transition. Supplement §S5.B explains transfer to the exact Haar distribution; Eq. (S62) formulates the quantitative hiding conjecture. My later [hiding paper, Theorem 2.1 and Corollary 2.2](https://arxiv.org/pdf/2609.01008v2#page=3), resolves this quantitative product-hiding conjecture with its quadratic scaling and uniformity over the number of squeezed inputs. Its [Theorem 3.1](https://arxiv.org/pdf/2609.01008v2#page=5) combines hiding with the companion's Gaussian small-ball bound to obtain finite-Haar lower tails.

Source: [arXiv record and submission history](https://arxiv.org/abs/2312.08433).

### March 20, 2024: Companion second-moment work

The same five authors submitted **[“The Second Moment of Hafnians in Gaussian Boson Sampling”](https://arxiv.org/abs/2403.13878)**, arXiv:2403.13878, at **18:00:00 UTC**.

The paper develops a recursive moment expression, evaluates it numerically exactly up to photon sector $2n=80$, and derives further analytical moment results and consequences for ideal linear cross-entropy benchmarking.

Source: [arXiv record and submission history](https://arxiv.org/abs/2403.13878).

### September 16, 2024: The IMSI talk that inspired me

Alexey Gorshkov delivered **[“Anticoncentration and Entanglement in Gaussian Boson Sampling”](https://www.imsi.institute/videos/anticoncentration-and-entanglement-in-gaussian-boson-sampling/)** at IMSI. Watching this talk inspired my work on Gaussian Gram hafnian moments and weak anticoncentration. The date here is the talk's date.

### April 8, 2025: Journal publication of both moment papers

Both companion papers were published on **April 8, 2025**:

- **“Transition of Anticoncentration in Gaussian Boson Sampling”**, *Physical Review Letters* **134**, 140601. [Publisher record](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.134.140601).
- **“Second moment of Hafnians in Gaussian boson sampling”**, *Physical Review A* **111**, 042412. [Publisher record](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.111.042412).

Their moment-based weak-anticoncentration conclusions provide background for the later local small-ball problem. These journal dates follow the 2023 and 2024 initial arXiv submissions.

### July 22, 2026: Koehler–Leung's permanent breakthrough

Frederic Koehler and Pui Kuen Leung submitted **[“Anticoncentration of the Permanent in Ginibre Ensembles”](https://arxiv.org/abs/2607.20329)** at **16:15:28 UTC**. I regard their Fourier compression and Gaussian comparison framework as a decisive methodological breakthrough for my hafnian work.

### August 17, 2026: My earlier weak-anticoncentration paper

I submitted **[“Exact Moments of Gaussian Gram Hafnians Reveal an n²/log n Threshold for Weak Anticoncentration”](https://arxiv.org/abs/2608.17065)**, arXiv:2608.17065. The public history records v1 at **19:12:22 UTC**.

This paper evaluates the second and fourth absolute moments of complex Gaussian Gram hafnians and identifies the scaling threshold for an inverse-polynomial weak-anticoncentration moment criterion. It is an earlier part of the research program; the subsequent complex-Gaussian manuscript develops local small-ball estimates.

I used ChatGPT with **GPT 5.6 Sol** in this work. In subsequent correspondence with Alexey Gorshkov, I learned of his group's independent solution, and we agreed on independent-work acknowledgments. I have included a reciprocal acknowledgment in the version submitted to a journal.

While developing the weak result, I also worked on complex Gram small-ball bounds with **GPT 5.6 Sol in Ultra mode**. Adapting Koehler–Leung required an additional conditional Wishart argument to control dependent hafnian cofactors while preserving the transpose-Gram matrix.

Source: [arXiv record and submission history](https://arxiv.org/abs/2608.17065).

### August 25, 2026: Completion of Lean v1.0.0

I completed the first complex-Gaussian Lean verification release on **August 25**, and publicly released it on **September 1**.

The archive is **“Lean Verification for ‘Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry’”**, version **1.0.0**, DOI **10.5281/zenodo.22102635**. It contains verification code and supporting materials concerning conditional Wishart estimates and the complex symmetric Gaussian limit. The manuscript was distributed separately.

Zenodo lists **August 25** as its publication date. The archival record was created on **September 1 at 06:30:38 UTC**. These dates record different events in the release sequence.[^dates]

Sources: [Lean v1.0.0](https://zenodo.org/records/22102635) · [record metadata](https://zenodo.org/records/22102635).

### August 26, 2026: Initial complex-Gaussian submission

At **05:45:55 UTC**, arXiv acknowledged submission **7994335**, titled **“Shifted Anticoncentration of Complex Gaussian Transpose-Gram Hafnians via Conditional Wishart Geometry”**.

The acknowledgment describes an **18-page** manuscript and identifies the accompanying Lean archive, DOI 10.5281/zenodo.22102635. This is the earliest submission acknowledgment in my records for the complex-Gaussian manuscript.

### August 27, 2026: Related closed-form moment and weak-threshold result

Laura Shou, Adam Ehrenberg, Yu-Xin Wang, Joseph T. Iosue, and Alexey V. Gorshkov submitted **[“Anticoncentration and entanglement in Gaussian boson sampling”](https://arxiv.org/abs/2609.01241)**, arXiv:2609.01241. Its public v1 history records **17:55:00 UTC on August 27**, despite the September-formatted identifier.

Theorem 2.1 gives a closed form for $M_2(k,n)=\mathbb E|\mathrm{haf}(X^{\mathsf T}X)|^4$ and identifies the sharp scaling threshold $k$ of order $n^2/\log n$ for weak anticoncentration. Here “second moment” is the second moment of the squared hafnian magnitude, hence the fourth absolute moment of the amplitude.

The **Note added** acknowledges my independent closed-form moment and weak-threshold work, arXiv:2608.17065. My subsequent complex companion develops the local small-ball bounds.

Their [acknowledgments, p. 14](https://arxiv.org/pdf/2609.01241v1#page=14), disclose assistance from **GPT 5.5 Thinking and Pro**.

Sources: [arXiv history](https://arxiv.org/abs/2609.01241) · [v1 PDF, Theorem 2.1, page 2](https://arxiv.org/pdf/2609.01241v1#page=2) · [Note added, page 15](https://arxiv.org/pdf/2609.01241v1#page=15).

### September 1, 2026: Complex submission, Two Routes, public Lean archives, and hiding v1

An updated acknowledgment under **7994335** records the title **“Shifted Anticoncentration of Complex Gaussian Gram Hafnians via Conditional Wishart Geometry”** and a **22-page** manuscript. This follows the August 26 initial acknowledgment. The first Lean archive was publicly released on September 1.

[Original September 1 receipt image](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-01-7994335.png).

I separately submitted **[“Two Routes from Additive to Relative Accuracy in Gaussian Boson Sampling”](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf)** under temporary arXiv number **7994183**. The acknowledgment identifies a **five-page manuscript with one figure** and prints the date **September 1, 2026**, with time **00:39:01 EST** as displayed in the receipt. Its abstract expressly names both the finite transpose-Gram reference and the independent complex symmetric Gaussian reference.

My Overleaf history also shows the *Two Routes* project on **September 1**, with `main.tex`, `references.bib`, and the figure file added by upload. The screenshot displays **“1st September, 6:28 am”** for that history entry.

In the [author-supplied manuscript](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf), **Eq. (4), p. 1**, uses the finite complex transpose-Gram theorem, while **Eq. (8), p. 2**, explicitly states the independent circular complex symmetric Gaussian small-ball bound with coefficient $b_n$. It cites **Theorem I.3 of reference [8]**, whose proof is identified as the first subsection of Appendix D. Reference [8], on p. 4, names the earlier *Shifted Anticoncentration of Complex Gaussian Gram Hafnians* companion; reference [7] names the hiding manuscript.

The [Two Routes Lean v1.0.0 archive](https://zenodo.org/records/22102501) was created at **05:02:29 UTC on September 1**. Its equation crosswalk explicitly records **row 8, `eq:symmetric-anticoncentration`**, and the bundled independent symmetric Gaussian package records `symmetricHafnian_shifted_smallBall` with only the standard Lean foundations in its axiom audit. This provides a dated public verification record for the independent complex result in addition to my retained submission and Overleaf records.

I also submitted **[“Uniform Hiding of Haar Block Transpose Gram Matrices”](https://arxiv.org/abs/2609.01008v1)**, arXiv:2609.01008v1, at **09:55:29 UTC**, as recorded in its public history.

The actual **v1 PDF, page 22, reference [13]**, cites the complex-Gaussian companion under the *Shifted Anticoncentration* title. This version-specific citation documents the connection in the version submitted on September 1, before the September 20 Zenodo manuscript deposit.

Sources: [Two Routes manuscript](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/manuscripts/two-routes-author-copy.pdf) · [Two Routes verification archive](https://zenodo.org/records/22102501) · [hiding submission history](https://arxiv.org/abs/2609.01008) · [v1 PDF, page 22](https://arxiv.org/pdf/2609.01008v1#page=22) · [complex Lean v1.0.0](https://zenodo.org/records/22102635).

### September 4, 2026: Removal request to reorganize the work

At **22:59:04 UTC**, I asked arXiv to remove submission **7994335** so that I could reorganize and resubmit the work.

The original complex submission was on hold. I requested removal to prepare the reorganized manuscripts, received confirmation on September 8, and submitted the revised complex manuscript on September 9 under a new identifier.

### September 6, 2026: Real-Gaussian paper and complex Lean v1.1.0

I subsequently developed the real-Gaussian results and submitted **[“Shifted Anticoncentration for Real Gram Hafnians and Symmetric Gaussian Hafnians”](https://arxiv.org/abs/2609.06526)**, arXiv:2609.06526. Its public v1 history records **10:47:33 UTC on September 6**, after the initial complex-Gaussian submission. The real verification materials are in **[RealGramHafnians](https://github.com/HongruZhao/RealGramHafnians)** and **[Zenodo v1.1.0](https://zenodo.org/records/22498111)**. I also began communicating the real result to researchers in probability.

The complex verification archive was also updated to **version 1.1.0**, DOI **10.5281/zenodo.22554594**, under **“Lean Verification for ‘Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry’”**. Its record was created at **23:29:30 UTC**.

Zenodo identifies v1.1.0 as the successor to v1.0.0 under the earlier *Shifted Anticoncentration* title. The [ComplexGramHafnians repository](https://github.com/HongruZhao/ComplexGramHafnians) is the development location, and the Zenodo archives preserve versioned verification materials for the same complex-Gaussian project.

The [September 6 verification record](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md) records a successful build for `theorem2_1` and `theorem2_3`, with exactly `propext`, `Classical.choice`, and `Quot.sound` in their dependency lists. These declarations cover the finite complex Gram and independent complex symmetric bounds. Revised `theorem2_3` corresponds to deposited Theorem 2.2.

Sources: [real-Gaussian arXiv history](https://arxiv.org/abs/2609.06526) · [complex Lean v1.1.0](https://zenodo.org/records/22554594) · [record metadata](https://zenodo.org/records/22554594).

### September 8, 2026: Removal confirmed

At **12:17:38 UTC**, arXiv confirmed removal of **7994335** in response to my September 4 request.

### September 9, 2026: New complex-Gaussian submission

At **07:19:23 UTC**, arXiv acknowledged the new submission **8055779**, titled **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”**.

The acknowledgment describes a **39-page** manuscript whose abstract explicitly includes the independent complex symmetric Gaussian limit. Submission 7994335 and submission 8055779 are separate administrative stages: the former was removed, and the latter is the reorganized submission.

[Original September 9 receipt image](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-09-8055779.png).

### September 10, 2026: QIQCOP entry created

The [QIQCOP entry](https://qiqc-op.com/problem/op_55be40726cdf7304/) was created on **September 10**, nine days after my updated September 1 submission and one day after the new September 9 acknowledgment.

The result resolving its anticoncentration statement was already in my September 1 submitted manuscript. The entry's creation followed that resolution, while the complex manuscript was still delayed by arXiv. Its discussion cites my later real paper, which has a different Gaussian ensemble, and omits the complex companion. As of September 30 it still displays “Unsolved,” and its latest visible revision is dated **September 25**.

Source: [QIQCOP statement and edit log](https://qiqc-op.com/problem/op_55be40726cdf7304/).

### September 11, 2026: Hiding v2 and two relative-accuracy routes

I submitted arXiv:2609.01008v2 at **07:30:07 UTC**, under **[“Uniform Hiding and Two Routes to Relative Accuracy in Gaussian Boson Sampling”](https://arxiv.org/abs/2609.01008v2)**.

This **v2** combines my **September 1 hiding v1** with the separate **September 1 Two Routes manuscript, submission 7994183**. The independent complex small-ball input in *Two Routes* Eq. (8) appears in the combined paper as Eq. (3.4).

The actual **v2 PDF, page 48, reference [12]**, cites **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”**. **Eq. (3.2)** gives the finite Gram small-ball input; **Eq. (3.4)** gives the independent complex symmetric input. **Theorem 3.1**, “Two finite-interferometer lower tails,” transfers them through hiding, and **Theorem 3.2** combines them with an assumed additive-estimation guarantee for two relative-accuracy routes.

The reference changes from **[13], page 22, in v1**, under the earlier title, to **[12], page 48, in v2**, under the *Local Anticoncentration* title. Both citations concern the same complex-Gaussian project.

Sources: [arXiv history](https://arxiv.org/abs/2609.01008) · [v2 PDF, Section 3, pages 4–6](https://arxiv.org/pdf/2609.01008v2#page=4) · [v2 PDF, page 48](https://arxiv.org/pdf/2609.01008v2#page=48).

### September 17, 2026: New submission confirmed on hold

In a reply dated **September 17 at 14:13:28 UTC**, arXiv Technical Support confirmed that **8055779** was on hold pending a decision by the volunteer moderators and that no action was required from me at that time. This status concerns the new September 9 submission. September 17 is the support-confirmation date; September 20 is the subsequent Zenodo release date.

### September 20, 2026: Public manuscript release

While submission **8055779** remained on hold, I deposited **“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”** on Zenodo as manuscript **version 1.0.0**, DOI **10.5281/zenodo.22856033**. I made this public release because of the prolonged arXiv delay.

Zenodo lists **September 20** as the publication date and records creation at **09:41:35 UTC**. The deposit contains the **14-page main article** and **33-page supplement** and links the accompanying Lean archive and repository.

**Theorem 2.1**, on page 4 of the main article, treats finite complex Gaussian transpose-Gram hafnians for $n\ge1$ and $k\ge4n$. **Theorem 2.2**, on page 5, treats independent complex symmetric Gaussian hafnians for every $n\ge1$. Its proof in **Supplementary Section S9.1, page S24**, fixes $n$, normalizes $X^{\mathsf T}X$ by $k^{-1/2}$, and passes the finite small-ball bound to the Gaussian limit.

**Corollary 2.4**, on page 6, supplies $p(n,1/\delta)=2n/\delta$ for the exact QIQCOP lower-tail statement. The diagonal variance convention in the paper does not affect the ordinary hafnian, so it also covers the catalog's zero-diagonal ensemble.

The manuscript's v1.0.0 and the Lean archive's v1.0.0 are version labels for separate artifacts with separate release dates.

Sources: [manuscript archive](https://zenodo.org/records/22856033) · [main article, pages 4–6](https://zenodo.org/records/22856033/files/main.pdf#page=4) · [supplement, page S24](https://zenodo.org/records/22856033/files/supplement.pdf#page=24) · [record metadata](https://zenodo.org/records/22856033).

### September 20, 2026: Zhang's complex manuscript

Yuxuan Zhang's **[“Anticoncentration of Independent Complex Gaussian Hafnians”](https://yuxuanzhang1995.github.io/agentic-research/complex-gaussian-hafnian/)** is dated September 20. Its references include Koehler–Leung and my real and weak Gram papers, but omit my complex companion, the separate *Two Routes* manuscript, and the combined hiding paper. Its lower-tail conclusion is supplied by my complex companion's [Theorem 2.2 and Corollary 2.4](https://zenodo.org/records/22856033).

My independent complex theorem was already explicit in *Two Routes* **Eq. (8), p. 2**, supported by the [September 1 verification archive](https://zenodo.org/records/22102501), and stated publicly in [hiding v2 **Eq. (3.4), p. 4**](https://arxiv.org/pdf/2609.01008v2#page=4). An implication that my earlier work had not resolved the independent complex case is therefore incorrect. My dated record precedes the Zhang and Pant manuscripts compared here.

The [first site commit](https://github.com/yuxuanzhang1995/yuxuanzhang1995.github.io/commit/9ba4cd37740c3ec9e88895a0e994dd3087b0d5ac) is timestamped **September 21, 00:50:33 UTC**, corresponding to September 20 in Chicago. This distinguishes the page's preparation date from the UTC commit date.

### September 28, 2026: Pant's concurrent complex paper

Priyanshu Pant submitted **[“Anticoncentration of Complex Gaussian Hafnians”](https://arxiv.org/abs/2609.35019)** at **12:18:39 UTC**. The [introduction, p. 3](https://arxiv.org/pdf/2609.35019v1#page=3), acknowledges concurrent Zhao work covering the complex symmetric Gaussian ensemble. **Reference [9]** points to my **[September 11 hiding v2](https://arxiv.org/abs/2609.01008v2)**, which combines the two September 1 manuscripts. Its [**Eq. (3.4), p. 4**](https://arxiv.org/pdf/2609.01008v2#page=4), cites the complex companion and carries forward the independent complex bound in *Two Routes* **Eq. (8)**. My companion's [**Theorem 2.2 and Corollary 2.4**](https://zenodo.org/records/22856033) give the shifted small-ball bound and its polynomial specialization. Pant's paper also develops product-Gamma and negative-moment results.

### September 30, 2026: Public correction comment and arXiv status recorded that day

At **18:12:56 UTC**, I posted a comment in the quantum-open-problems discussion identifying the September 20 manuscript, its independent complex-Gaussian theorem and corollary, and the verification materials. I asked the maintainers to review the result, add the preprint to the progress record and references, and assess the entry's status and attribution.

The comment also explains the numbering: **Theorem 2.2 in the September 20 main article corresponds to revised Lean `theorem2_3`**. The [recorded September 6 verification](https://github.com/HongruZhao/ComplexGramHafnians/blob/95ab10dc594ac92207054413220ae9fd2adab08c/verification/STATUS.md) reports a successful build and the exact standard-foundation dependencies for the finite and independent-symmetric declarations.

The comment is in **issue #92**, another candidate report concerning the catalog problem. The catalog still displays **“Unsolved”** as of September 30.

My arXiv dashboard still showed **8055779** as **on hold** on September 30. The earlier **7994335** was removed on September 8; the hold recorded that day belonged to the new submission acknowledged on September 9.

Sources: [public correction comment](https://github.com/Naixu-Guo/quantum-open-problems/issues/92#issuecomment-5917023518) · [QIQCOP entry](https://qiqc-op.com/problem/op_55be40726cdf7304/).

### October 1, 2026 (US Eastern): Public arXiv availability

My **[“Local Anticoncentration for Gaussian Boson Sampling via Conditional Wishart Geometry”](https://arxiv.org/abs/2610.00112)** is now publicly available as **arXiv:2610.00112**, authored by **Hongru Zhao**, in **math.PR** with a **quant-ph** cross-list. Its public v1 history retains **September 9, 2026, 07:19:22 UTC** as the submission timestamp. The retained acknowledgment for **8055779** is dated **07:19:23 UTC** that day; the one-second difference distinguishes the submission metadata from the acknowledgment time.

October 1 is the public-availability date in US Eastern time. Public access was checked on October 2 UTC, while it was still October 1 in US Eastern. The abstract page does not separately display the exact announcement timestamp. The [official announcement schedule](https://info.arxiv.org/help/availability.html) uses US Eastern time; an October 1 announcement at 20:00 EDT corresponds to October 2 at 00:00 UTC. The original September 9 submission date is not evidence that the manuscript was public on September 9.

The earlier **7994335** submission and removal, the September 9 **8055779** receipt, the September hold records, and the September 20 Zenodo manuscript release are preserved as distinct events.

Sources: [public arXiv record and v1 history](https://arxiv.org/abs/2610.00112) · [availability and announcement schedule](https://info.arxiv.org/help/availability.html) · [September 9 receipt](https://github.com/HongruZhao/Hafnian-Anticoncentration-Timeline/blob/main/assets/submission-receipts/2026-09-09-8055779.png).

## How the companion results fit together

The hiding paper compares finite interferometer matrix laws with Gaussian reference laws. The complex-Gaussian companion controls how often their hafnians fall in a small disk around any prescribed center. The separate September 1 *Two Routes* manuscript composed these inputs; I incorporated that manuscript into the September 11 hiding v2.

The two routes use different Gaussian references:

1. **Finite transpose-Gram route.** For a rectangular Gaussian matrix $G$, the reference $GG^{\mathsf T}$ retains dependence between entries. Uniform product hiding combines with the companion's local bound for this finite ensemble.
2. **Independent symmetric route.** The reference has independent complex Gaussian entries above the diagonal. A corresponding hiding estimate combines with the companion's bound for that symmetric ensemble.

In [Section 3 of hiding v2](https://arxiv.org/pdf/2609.01008v2#page=4), **Theorem 3.1** transfers these small-ball bounds to finite-interferometer lower tails. **Theorem 3.2** uses those tails with an assumed additive-estimation guarantee to obtain relative-accuracy bounds. The comparison uses the same estimator and absolute additive threshold and accounts for the different reference probability scales.

Local anticoncentration is a key mathematical input to these applications. The hiding and Gaussian small-ball proofs are developed separately. Their composition provides lower-tail and relative-accuracy guarantees in the stated regimes; additive estimation and average-case computational hardness remain separate inputs to a full GBS sampling-hardness argument.

The earlier moment papers and hiding estimates together transfer weak anticoncentration. A shrinking small-ball conclusion additionally uses the local Gaussian bounds. This distinguishes the earlier weak-threshold question from the polynomial lower-tail statement resolved by my complex companion.

## Names and attribution

Quesada, Arrazola, and Killoran explicitly use **“Hafnian-anti-concentration conjecture”** in [*Gaussian Boson Sampling Using Threshold Detectors*, §IV](https://arxiv.org/pdf/1807.01639#page=3). The name therefore predates the September 2026 catalog entry. Precise ensemble descriptions in later titles are also natural mathematical terminology. Zhang's page names the catalog as its target; title similarity alone does not establish another author's motivation or awareness. The chronology records submissions, releases, and citations as the basis for attribution.

## The submission and release sequence

The complex-Gaussian manuscript follows two arXiv submission stages:

**August 26 initial submission 7994335 → September 1 update → September 4 removal request → September 8 removal confirmed → September 9 new submission 8055779 → September 17 hold confirmed → September 20 public Zenodo release → September 30 still on hold → October 1 (US Eastern) publicly available as arXiv:2610.00112.**

The public record also connects the project through the September 1 complex and Two Routes Lean archives and hiding-v1 citation, the September 6 Lean update, and the September 11 combined hiding-v2 statement and citation. The separate Two Routes submission **7994183** and its September 1 Overleaf history document another part of that development sequence. My dated independent complex result precedes the September 10 catalog entry and the later Zhang and Pant manuscripts.

## Separate submission-policy note — effective October 1, 2026

The [official October 1 announcement and FAQ](https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/) set a limit of **two submissions per calendar month per submitter**, across all categories, alongside **three total active submissions at any time**. Coauthors may coordinate who submits a jointly authored paper: only the submitter's limits are affected. The three-active-submission limit has existed since 2024. This October 1 policy update is not evidence of the cause of the September moderation hold.

[^dates]: The [Lean v1.0.0 archive](https://zenodo.org/records/22102635) lists August 25, 2026, as its publication date. I completed the Lean code that day and released it publicly on September 1. Zenodo created the record on September 1, 2026, at 06:30:38 UTC. arXiv history timestamps record submissions, which can precede public announcements.
