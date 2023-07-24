---
title: Manuscript Title
keywords:
- markdown
- publishing
- manubot
lang: en-US
date-meta: '2023-07-24'
author-meta:
- John Doe
- Jane Roe
header-includes: |
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta property="og:type" content="article" />
  <meta name="dc.title" content="Manuscript Title" />
  <meta name="citation_title" content="Manuscript Title" />
  <meta property="og:title" content="Manuscript Title" />
  <meta property="twitter:title" content="Manuscript Title" />
  <meta name="dc.date" content="2023-07-24" />
  <meta name="citation_publication_date" content="2023-07-24" />
  <meta property="article:published_time" content="2023-07-24" />
  <meta name="dc.modified" content="2023-07-24T14:07:55+00:00" />
  <meta property="article:modified_time" content="2023-07-24T14:07:55+00:00" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="John Doe" />
  <meta name="citation_author_institution" content="Department of Something, University of Whatever" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="twitter:creator" content="@johndoe" />
  <meta name="citation_author" content="Jane Roe" />
  <meta name="citation_author_institution" content="Department of Something, University of Whatever" />
  <meta name="citation_author_institution" content="Department of Whatever, University of Something" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <link rel="canonical" href="https://greenelab.github.io/generalization-manuscript/" />
  <meta property="og:url" content="https://greenelab.github.io/generalization-manuscript/" />
  <meta property="twitter:url" content="https://greenelab.github.io/generalization-manuscript/" />
  <meta name="citation_fulltext_html_url" content="https://greenelab.github.io/generalization-manuscript/" />
  <meta name="citation_pdf_url" content="https://greenelab.github.io/generalization-manuscript/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://greenelab.github.io/generalization-manuscript/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://greenelab.github.io/generalization-manuscript/v/056f683d4f1c0d561635a4e1ce8eaa9fb1e0683b/" />
  <meta name="manubot_html_url_versioned" content="https://greenelab.github.io/generalization-manuscript/v/056f683d4f1c0d561635a4e1ce8eaa9fb1e0683b/" />
  <meta name="manubot_pdf_url_versioned" content="https://greenelab.github.io/generalization-manuscript/v/056f683d4f1c0d561635a4e1ce8eaa9fb1e0683b/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://greenelab.github.io/generalization-manuscript/v/056f683d4f1c0d561635a4e1ce8eaa9fb1e0683b/))
was automatically generated
from [greenelab/generalization-manuscript@056f683](https://github.com/greenelab/generalization-manuscript/tree/056f683d4f1c0d561635a4e1ce8eaa9fb1e0683b)
on July 24, 2023.
</em></small>



## Authors



+ **John Doe**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [johndoe](https://github.com/johndoe)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [johndoe](https://twitter.com/johndoe)
    · ![Mastodon icon](images/mastodon.svg){.inline_icon width=16 height=16}
    [\@johndoe@mastodon.social](https://mastodon.social/@johndoe)
    <br>
  <small>
     Department of Something, University of Whatever
     · Funded by Grant XXXXXXXX
  </small>

+ **Jane Roe**
  ^[✉](#correspondence)^<br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [janeroe](https://github.com/janeroe)
    <br>
  <small>
     Department of Something, University of Whatever; Department of Whatever, University of Something
  </small>


::: {#correspondence}
✉ — Correspondence possible via [GitHub Issues](https://github.com/greenelab/generalization-manuscript/issues)
or email to
Jane Roe \<jane.roe@whatever.edu\>.


:::


## Abstract {.page_break_before}




## Methods {.page_break_before}

### Mutation data download and preprocessing

To generate binary mutated/non-mutated gene labels for our machine learning model, we used mutation calls for TCGA samples from MC3 [@doi:10.1016/j.cels.2018.03.002] and copy number threshold calls from GISTIC2.0 [@doi:10.1186/gb-2011-12-4-r41].
MC3 mutation calls were downloaded from the Genomic Data Commons (GDC) of the National Cancer Institute, at <https://gdc.cancer.gov/about-data/publications/pancanatlas>.
Thresholded copy number calls are from an older version of the GDC data and are available here: <https://figshare.com/articles/dataset/TCGA_PanCanAtlas_Copy_Number_Data/6144122>.
We removed hypermutated samples, defined as two or more standard deviations above the mean non-silent somatic mutation count, from our dataset to reduce the number of false positives (i.e., non-driver mutations).
Any sample with either a non-silent somatic variant or a copy number variation (copy number gain in the target gene for oncogenes and copy number loss in the target gene for tumor suppressor genes) was included in the positive set; all remaining samples were considered negative for mutation in the target gene.

We followed a similar procedure to generate binary labels for cell lines from CCLE, using the data available on the DepMap download portal at <https://depmap.org/portal/download/all/>.
Mutation information was retrieved from the `OmicsSomaticMutations.csv` data file, and copy number inforamtion was retrieved from the `OmicsCNGene.csv` data file.
We thresholded the CNV log-ratios provided by CCLE into binary gain/loss calls using a lower threshold of log~2~(3/2) (i.e. cell lines with a log-ratio below this threshold were considered to have a full copy loss in the corresponding gene), and an upper threshold of log~2~(5/2) (i.e. cell lines with a log-ratio above this threshold were considered to have a full copy gain in the corresponding gene).
After applying the same hypermutation criteria that we used for TCGA, no cell lines in CCLE were identified as hypermutated.
After preprocesing, 1402 cell lines with mutation and copy number data remained.
We then combined non-silent point mutations and copy number gain/loss information into binary labels using the same criteria as for TCGA.

### Gene expression data download and preprocessing

RNA sequencing data for TCGA was downloaded from GDC at the same link provided above for the Pan-Cancer Atlas.
We discarded non-protein-coding genes and genes that failed to map, and removed tumors that were measured from multiple sites.
After filtering to remove hypermutated samples and taking the intersection of samples with both mutation and gene expression data, 9074 TCGA samples remained.

RNA sequencing data for CCLE was downloaded from the DepMap download portal, linked above, in the `CCLE_expression.csv` data file.
After taking the intersection of CCLE cell lines with both mutation and gene expression data, 1402 cell lines remained.
For experiments making predictions across datasets (i.e., training models on TCGA and evaluating performance on CCLE, or vice-versa) we took the intersection of genes in both datasets, resulting in 16041 gene features.
For experiments where only TCGA data was used (i.e., evaluating models on held-out cancer types), we used all 16148 gene features present in TCGA after the filtering described above.

### Cancer gene set construction

In order to study mutation status classification for a diverse set of cancer driver genes, we started with the set of 125 frequently altered genes from Vogelstein et al. [@doi:10.1073/pnas.1616440113] (all genes from Table S2A).
For each target gene, to ensure that the training dataset was reasonably balanced (i.e., that there would be enough mutated samples to train an effective classifier), we included only cancer types with at least 15 mutated samples and at least 5% mutated samples, which we refer to here as "valid" cancer types.
In some cases, this resulted in genes with no valid cancer types, which we dropped from the analysis.
Out of the 125 genes originally listed in the Vogelstein et al. cancer gene set, we retained 71 target genes for the TCGA to CCLE analysis, and 70 genes for the CCLE to TCGA analyses.
For these analyses, each gene needed at least one valid cancer type in TCGA and one valid cancer type in CCLE, to construct the train and test sets.
For the cancer type holdout analysis, we retained 56 target genes: in this case, each gene needed at least two valid cancer types in TCGA to be retained, one to train on and one to hold out.

### Classifier setup and cross-validation design

We trained logistic regression classifiers to predict whether or not a given sample had a mutational event in a given target gene using gene expression features as explanatory variables.
Our model was trained on gene expression data (X) to predict somatic mutation presence or absence (y) in a target gene.
To control for varying mutation burden per sample and to adjust for potential cancer type-specific expression patterns, we included one-hot encoded cancer type and log~10~(sample mutation count) in the model as covariates.
Since gene expression datasets tend to have many dimensions and comparatively few samples, we used a LASSO penalty to perform feature selection [@doi:10.1111/j.2517-6161.1996.tb02080.x].
LASSO logistic regression has the advantage of generating sparse models (some or most coefficients are 0), as well as having a single tunable hyperparameter which can be easily interpreted as an indicator of regularization strength/model simplicity.

LASSO ($\ell_1$-penalized) logistic regression finds the feature weights $\hat{w} \in \mathbb{R}^{p}$ solving the following optimization problem:

$$\hat{w} = \text{argmin}_{w} \ (C \cdot l(X, y; w)) + ||w||_1$$

where $i \in \{1, \dots, n\}$ denotes a sample in the dataset, $X_i \in \mathbb{R}^{p}$ denotes features (gene expression measurements) from the given sample, $y_i \in \{0, 1\}$ denotes the label (mutation presence/absence) for the given sample, and $l(\cdot)$ denotes the negative log-likelihood of the observed data given a particular choice of feature weights, i.e.

$$l(X, y; w) = -\sum_{i=1}^{n} y_i \log\left(\frac{1}{1 + e^{-w^{\top}X_i}}\right) + (1 - y_i) \log\left(1 - \frac{1}{1 + e^{-w^{\top}X_i}}\right)$$

Given weight values $\hat{w}$, it is straightforward to predict the probability of a positive label (mutation in the target gene) $P(y^{*} = 1 \mid X^{*}; \hat{w})$ for a test sample $X^{*}$:

$$P(y^{*} = 1 \mid X^{*}; \hat{w}) = \frac{1}{1 + e^{-\hat{w}^{\top}X^{*}}}$$

and the probability of no mutation in the target gene, $P(y^{*} = 0 \mid X^{*}; \hat{w})$, is given by (1 - the above quantity).

This optimization problem leaves one hyperparameter to select: $C$, which controls the inverse of the strength of the L1 penalty on the weight values (i.e. regularization strength scales with $\frac{1}{C}$).
Although the LASSO optimization problem does not have a closed form solution, the loss function is convex, and iterative optimization algorithms are commonly used for finding reasonable solutions.
For fixed values of $C$, we solved for $\hat{w}$ using `scikit-learn`'s `LogisticRegression` method [@url:https://jmlr.org/papers/v12/pedregosa11a.html], which uses the coordinate descent optimization method implemented in `liblinear` [@url:https://www.jmlr.org/papers/v9/fan08a.html].
We selected this implementation rather than the `SGDClassifier` stochastic gradient descent implementation because coordinate descent/`liblinear` tends to generate sparser models and does not depend on a learning rate parameter, although after hyperparameter tuning performance is generally comparable between the implementations [@doi:10.1101/2023.06.26.546586].

To assess model selection across contexts (datasets and cancer types), we trained models using a variety of LASSO parameters on 75% of the training dataset, holding out 25% of the training dataset as the "cross-validation" set and also evaluating across contexts as the "test" set.
We trained models using $C$ values evenly spaced on a logarithmic scale between (10^-3^, 10^7^); i.e. the output of `numpy.logspace(-3, 7, 21)`.
This range was intended to give evenly distributed coverage across genes and cancer types that included "underfit" models (predicting only the mean or using very few features, poor performance on all datasets), "overfit" models (performing perfectly on training data but comparatively poorly on cross-validation and test data), and a wide variety of models in between that typically included the best fits to the cross-validation and test data.
To assess variability between train/CV splits, we used all 4 splits (25% holdout sets) x 2 random seeds for a total of 8 different training sets for each gene, using the same test set (i.e. all of the held-out context, either one cancer type or one dataset) in each case.

### "Best model" vs. "smallest good model" analysis details

Description of "smallest good" heuristic
Statistical testing?

### Neural network setup and parameter selection

Inspired by the intermediate-complexity model in [@doi:10.1371/journal.pcbi.1010984], as a tradeoff between computational cost and ability to represent non-linear decision boundaries, we trained a three-layer fully connected neural network with ReLU nonlinearities [@https://dl.acm.org/doi/10.5555/3104322.3104425] to predict mutation status.
For the experiments described in the main paper, we varied the size of the first hidden layer in the range {1, 2, 3, 4, 5, 10, 50, 100, 500, 1000}.
We fixed the size of the second hidden layer to be half of the size of the first hidden layer, rounded up to the nearest integer, and the size of the third hidden layer was the number of classes, 2 in our case.
Our models were trained for 100 epochs of mini-batch stochastic gradient descent in PyTorch [@arxiv:1912.01703], using the Adam optimizer [@arxiv:1412.6980] and a fixed batch size of 50.
To select the remaining hyperparameters for each hidden layer size, we performed a random search over 10 combinations, with a single train/test split stratified by cancer type, using the following hyperparameter ranges: learning rate {0.1, 0.01, 0.001, 5e-4, 1e-4}, dropout proportion {0.1, 0.5, 0.75}, weight decay (L2 penalty) {0, 0.1, 1, 10, 100}.
We used the same train/cross-validation split strategy described above, generating 8 different performance measurements for each gene and hidden layer size, for the neural network experiments as well.

For the _EGFR_ gene, we also ran experiments where we varied the dropout proportion and the weight decay hyperparameter as the regularization axis, and selected the remaining hyperparameters (including the hidden layer size) using a random search.
In these cases, we used a fixed range for dropout of {0.0, 0.05, 0.125, 0.25, 0.375, 0.5, 0.625, 0.75, 0.875, 0.95}, and a fixed range for weight decay of {0.0, 0.001, 0.005, 0.01, 0.05, 0.1, 0.2, 0.3, 0.4, 0.5, 0.75, 1.0, 10.0}.
All neural network analyses were performed on a Ubuntu 18.04 machine with a NVIDIA RTX 2060 GPU.

### Open science/reproducibility stuff


## Results {.page_break_before}

### Evaluating model generalization using public cancer data

We collected data from the TCGA Pan-Cancer Atlas and the Cancer Cell Line Encyclopedia to predict the presence or absence of mutations in cancer genes, as a benchmark of cancer-related information content across cancer types and contexts.
We trained mutation status classifiers across approximately 70 genes involved in cancer development and progression from Vogelstein et al. 2013 [@doi:10.1126/science.1235122], using LASSO logistic regression with gene expression (RNA-seq) values as predictive features.
We designed experiments to evaluate the generalization of mutation status classifiers across datasets (TCGA to CCLE and CCLE to TCGA) and across biological contexts (cancer types) within TCGA, relative to a within-dataset baseline (Figure {@fig:overview}).

![
Schematic of experimental design. The colors of the "dots" in the training/model selection/model evaluation panels on the left correspond to train/CV/test curves in the following results figures.
](images/figure_1.png){#fig:overview width="90%"}

### Generalization from human tumor samples to cell lines is more effective than the reverse

To evaluate "cross-dataset" generalization, we trained mutation status classifiers on human tumor data from TCGA and evaluated them on cell line data from CCLE, as well as the reverse from CCLE to TCGA.
As an example, we examined _EGFR_, an oncogenic tyrosine kinase that is commonly mutated in diverse cancer types and cancer cell lines, including lung cancer, colorectal cancer, and glioblastoma [@doi:10.1146/annurev-pathol-011110-130206; @doi:10.1002/cac2.12005].
For EGFR mutation status classifiers trained on TCGA and evaluated on CCLE, we saw that AUPR on cell lines was slightly worse than on held-out tumor samples, but comparable across regularization levels/LASSO parameters (Figure {@fig:tcga_ccle_overall}A).
On the other hand, EGFR classifiers trained on CCLE and evaluated on TCGA performed considerably worse on human tumor samples as compared to held-out cell lines (Figure {@fig:tcga_ccle_overall}B).

To explore these tendencies more generally, we compared performance across all genes in the Vogelstein et al. dataset, for both TCGA to CCLE and CCLE to TCGA generalization.
We measured the difference between performance on the holdout data within the training dataset and performance across datasets, with a positive difference indicating poor generalization (better holdout performance than test performance) and a 0 or negative difference indicating good generalization (comparable test performance to holdout performance).
For generalization from TCGA to CCLE, we observed that median AUPR differences were mostly centered around 0 for most genes, with some exceptions at the extremes (Figure {@fig:tcga_ccle_overall}C; performance differences on the y-axis).
An example of a gene exhibiting poor generalization was _IDH1_, the leftmost gene in Figure {@fig:tcga_ccle_overall}C, with good performance on held-out TCGA data and poor performance on CCLE data.
IDH-mutant glioma cell lines are poorly represented compared to IDH-mutant patient tumors, which may explain the difficulty of generalization to cell lines for _IDH1_ mutation classifiers [@doi:10.1093/noajnl/vdaa088].
For generalization from CCLE to TCGA, we observed a more pronounced upward shift toward better performance on CCLE and worse on TCGA, with most genes performing better on the CCLE holdout data and very few genes generalizing comparably to the TCGA samples (Figure {@fig:tcga_ccle_overall}D).

![
**A.** _EGFR_ mutation status prediction performance on training samples from TCGA (blue), held-out TCGA samples (orange), and CCLE samples (green), across varying LASSO parameters.
**B.** _EGFR_ mutation status prediction performance on training samples from CCLE (blue), held-out CCLE samples (orange), and TCGA samples (green).
**C.** Difference in mutation status prediction performance for models trained on TCGA (holdout data) and evaluated on CCLE (test data), across 71 genes from Vogelstein et al. For each gene, the best model (LASSO parameter) was selected using holdout AUPR performance. Genes on x-axis are ordered by median AUPR difference across cross-validation splits, from highest to lowest.
**D.** Difference in mutation status prediction performance for models trained on CCLE (holdout data) and evaluated on TCGA (test data), across 70 genes from Vogelstein et al.
](images/figure_2.png){#fig:tcga_ccle_overall width="80%"}

### "Best" and "smallest good" model selection strategies perform comparably

To address the question of whether more parsimonious models tend to generalize better or not, we designed two model selection schemes and compared them for the TCGA to CCLE and CCLE to TCGA mutation prediction problems (Figure {@fig:tcga_ccle_smallest_best}A).
The "best" model selection scheme chooses the top-performing model/LASSO parameter on the holdout dataset from the same source as the training data and applies it to the test data from the other data source.
The intention of the "smallest good" model selection scheme is to balance parsimony with reasonable performance on the holdout data, since simply selecting the smallest possible model (generally, the dummy regressor/mean predictor) is not likely to generalize well.
To accomplish this, we first identify the top 25% of well-performing models on the holdout dataset; then, from this subset of models, we choose the smallest (i.e., highest LASSO parameter) to apply to the test data.
In both cases, we exclusively use the holdout data to select a model and only apply the model to out-of-dataset samples to evaluate generalization performance _after_ model selection.

For TCGA to CCLE generalization, 27/71 genes (38.0%) had better performance for the "best" model, and 17/71 genes (23.9%) had better generalization performance with the "smallest good" model.
The other 27 genes had the same "best" and "smallest good" model (in other words, the "smallest good" model was also the best-performing overall, and the difference was 0) (Figure {@fig:tcga_ccle_smallest_best}B).
For CCLE to TCGA generalization, 23/70 genes (32.9%) had better performance for the "best" model and 18/70 (25.7%) for the "smallest good," with the other 29 having the same model fulfill both criteria (Figure {@fig:tcga_ccle_smallest_best}C).
Overall, these results do not support the hypothesis that the most parsimonious model generalizes the best: for both generalization problems there are slightly more genes where the best-performing model on the holdout dataset is also the best-performing on the test set, although there are some genes where the "smallest good" approach works well.

We examined genes that fell into either category for TCGA to CCLE generalization (dotted lines on Figure {@fig:tcga_ccle_smallest_best}B).
For _NF1_, the "best" model outperforms the "smallest good" model (Figure {@fig:tcga_ccle_smallest_best}D).
Comparing holdout (orange) and cross-dataset (green) performance, both generally follow a similar trend, with the cross-dataset performance peaking when the holdout performance peaks at a regularization parameter of $\alpha = 0.00316$.
_PIK3CA_ is an example of the opposite, a gene where the "smallest good" model tends to outperform the "best" model (Figure {@fig:tcga_ccle_smallest_best}E).
In this case, the peak for the cross-dataset performance occurs at a higher level of regularization (further left on the x-axis), at $\alpha = 0.01$, than the peak for the holdout performance, at $\alpha = 0.0316$.
This suggests that a _PIK3CA_ mutation status classifier that is more parsimonious, but that has slightly worse performance, does tend to generalize better across datasets to CCLE.

![
**A.** Schematic of "best" vs. "smallest good" model comparison experiments.
**B.** Distribution of performance comparisons between "best" and "smallest good" model selection strategies, for TCGA -> CCLE generalization. Positive x-axis values indicate better performance for the "best" model, negative values indicate better performance for the "smallest good" model.
**C.** Distribution of performance comparisons between "best" and "smallest good" model selection strategies, for CCLE -> TCGA generalization.
**D.** _NF1_ mutation status prediction performance generalizing from TCGA (holdout, orange), to CCLE (green), with "best" and "smallest good" models labeled.
**E.** _PIK3CA_ mutation status prediction performance generalizing from TCGA (holdout, orange), to CCLE (green), with "best" and "smallest good" models labeled.
](images/figure_3.png){#fig:tcga_ccle_smallest_best width="90%"}

### Generalization across cancer types yields similar results to generalization across datasets

To evaluate generalization across biological contexts within a dataset, we trained mutation prediction classifiers on all but one cancer type in TCGA, performed model selection on a holdout set stratified by cancer type, and held out the remaining cancer type as a test set.
We performed the same "best" vs. "smallest good" analysis that was previously described, across 294 gene/holdout cancer type combinations (Figure {@fig:cancer_type_holdout}A).
We observed 127/294 gene/cancer type combinations (43.1%) that had better generalization performance with the "best" model, compared to 78/294 (26.5%) for the "smallest good" model.
The other 89 gene/cancer type combinations had the same "best" and "smallest good" model and thus no difference in performance.
This is consistent with our cross-dataset experiments, with slightly more instances where the "best" model on the stratified holdout data also generalizes the best, but no pronounced distributional shift in either direction.

We looked in more detail at two examples of gene/cancer type combinations, one on either side of the 0 point for cross-cancer type generalization.
For prediction of _SETD2_ mutation status in papillary renal cell carcinoma, we observed the best cross-cancer type performance for relatively low levels of regularization/high x-axis values (Figure {@fig:cancer_type_holdout}B).
For prediction of _CDKN2A_ mutation status in low grade glioma, on the other hand, we observed the best cross-cancer generalization for a high level of regularization ($\alpha = 0.01$), and generalization capability for the best parameter on the stratified holdout set ($\alpha = 0.0316$) was lower (Figure {@fig:cancer_type_holdout}C).

We also aggregated results across genes for each cancer type, looking at performance in the held-out cancer type compared to performance on the stratified holdout set (Figure {@fig:cancer_type_holdout}D).
Cancer types that were particularly difficult to generalize to (better performance on stratified data than cancer type holdout, or positive y-axis values) include testicular cancer (TGCT) and soft tissue sarcoma (SARC), which are notable because they are not carcinomas like the majority of cancer types included in TCGA, potentially making generalization harder.
Thyroid carcinoma (THCA) also had poor performance when held out, however.
In our experiments, the only genes in which THCA is included as a held-out cancer type are _BRAF_ and _NRAS_; previous work suggests that _BRAF_ mutation tends to have a different functional signature in THCA than other cancer types, and withholding THCA from the training set improved classifier performance [@doi:10.1016/j.celrep.2018.03.046].

![
**A.** Distribution of performance comparisons between "best" and "smallest good" model selection strategies, for generalization across TCGA cancer types. Each point is a gene/cancer type combination; positive x-axis values indicate better performance for the "best" model and negative values indicate better performance for the "smallest good" model.
**B.** _SETD2_ mutation status prediction performance generalizing from other cancer types in TCGA (stratified holdout, orange) to papillary renal cell carcinoma (KIRP, green), with "best" and "smallest good" models labeled.
**C.** _CDKN2A_ mutation status prediction performance generalizing from other cancer types in TCGA (stratified holdout, orange) to low grade glioma (LGG, green), with "best" and "smallest good" models labeled.
**D.** Distributions of performance difference between CV data (same cancer types as train data) and holdout data (cancer types not represented in train data), by held-out cancer type. Each point is a gene whose mutation status classifier was used to make predictions on out-of-dataset samples in the relevant cancer type.
](images/figure_4.png){#fig:cancer_type_holdout width="90%"}

### Small neural network hidden layer sizes tend to generalize poorly

To test whether or not findings generalize to non-linear models, we trained a 3-layer neural network to predict mutation status from gene expression for generalization from TCGA to CCLE, and we varied the size of the first hidden layer to control regularization/model complexity.
We fixed the size of the second hidden layer to be half the size of the first layer, rounded up to the nearest integer; further details in Methods.
For _EGFR_ mutation status prediction, we saw that performance for small hidden layer sizes was noisy, but generally lower than for higher hidden layer sizes (Figure {@fig:tcga_ccle_nn}A).
We also tried varying additional regularization parameters such as dropout and weight decay while holding the hidden layer size constant, and results followed a similar trend (Supplementary Figure TODO).
On average, over all 71 genes from Vogelstein et al., performance on both held-out TCGA data and CCLE data tends to increase until a hidden layer size of 10-50, then flatten (Figure {@fig:tcga_ccle_nn}B).

In order to measure which hidden layer sizes tended to perform relatively well or poorly, across different mutated cancer genes with different effect sizes, we ranked the range of hidden layer sizes by their generalization performance on CCLE (with low ranks representing good performance, and high ranks representing poor performance; Figure {@fig:tcga_ccle_nn}C).
For each hidden layer size, we then visualized the distribution of ranks above and below the median rank of 5.5/10; a high proportion of ranks above the median (True, or blue bar) signifies poor overall performance for that hidden layer size, and a high proportion of ranks below the median (False, or orange bar) signifies good performance.
We saw that small hidden layer sizes tended to generalize poorly (<5, but most pronounced for 1 and 2), and intermediate hidden layer sizes tended to generalize well (10-100, and sometimes 500/1000).
This suggests that some degree of parsimony/simplicity could be useful, but very simple models do not tend to generalize well.
We also performed the same "best"/"smallest good" analysis as with the linear models, using hidden layer size as the regularization axis instead of LASSO regularization strength.
We observed a distribution centered around 0, suggesting that the "best" and "smallest good" models tend to generalize similarly (Figure {@fig:tcga_ccle_nn}D).


![
**A.** _EGFR_ mutation status prediction performance on training samples from TCGA (blue), held-out TCGA samples (orange), and CCLE samples (green), across varying neural network hidden layer sizes.
**B.** Mutation status prediction performance summarized across all genes from Vogelstein et al. on training samples from TCGA (blue), held-out TCGA samples (orange), and CCLE samples (green), across varying neural network hidden layer sizes.
**C.** Distribution of ranked performance values above/below the median rank for each gene, for each of the hidden layer sizes evaluated. Lower ranks indicate better performance and higher ranks indicate worse performance, relative to other hidden layer sizes.
**D.** Distribution of performance comparisons between "best" and "smallest good" model selection strategies, for TCGA -> CCLE generalization with neural network hidden layer size as the regularization axis. Positive x-axis values indicate better performance for the "best" model, negative values indicate better performance for the "smallest good" model.
](images/figure_5.png){#fig:tcga_ccle_nn width="90%"}


## Discussion

Using public cancer genomics and transcriptomics data from TCGA and CCLE, we studied generalization of mutation status classifiers for a wide variety of cancer driver genes.
We designed experiments to evaluate generalization across biological contexts by holding out cancer types in TCGA, and to evaluate generalization across datasets by training models on TCGA and evaluating them on CCLE, and vice-versa.
We found that, in general, smaller or more parsimonious models do not tend to generalize more effectively across cancer types or across datasets, and in the absence of prior knowledge about a prediction problem, simply choosing the model that performs the best on a holdout dataset is at least as effective for selecting models that generalize.

Our results were similar in both linear models (LASSO logistic regression) and non-linear deep neural networks when using hidden layer size as the regularization parameter of interest.
In our non-linear model experiments, we did not observe better generalization across datasets for fully connected neural networks with fewer hidden layer nodes, and our preliminary results indicated a similar trend for dropout and weight decay.
Compared to linear models, it is less clear how to define a "small" or "parsimonious" neural network model since there are many regularization techniques that one may use to control complexity.
Rather than simply removing nodes and keeping the network fully connected, another approach to parsimony could be to select an inductive bias to guide the size reduction of the network.
Existing examples include network structures guided by protein-protein interaction networks or function/pathway ontologies [@doi:10.1016/j.ccell.2020.09.014; @doi:10.1093/bioinformatics/btx624; @doi:10.1186/s13059-020-02100-5; @doi:10.1016/j.patter.2022.100565].
It is possible that a smaller neural network with a structure that corresponds more appropriately to the prediction problem would achieve better generalization results, although choosing an apt network structure or data source can be a challenging aspect of such efforts.

For generalization from CCLE to TCGA, we observed that performance was generally worse on human tumor samples from TCGA than for held-out cell lines.
This could, at least in part, be a function of sample size: the number of cell lines in CCLE is approximately an order of magnitude smaller than the number of tumor samples in TCGA (~10,000 samples in TCGA vs. ~1,500 cell lines in CCLE, although the exact number of samples used to train and evaluate our classifiers varies by gene, see Methods for further detail).
There are also plausible biological and technical explanations for the difficulty of generalizing to human tumor samples.
This result could reflect the imperfect and limited nature of cancer cell lines as a model system for human tumors, which previous studies have pointed out [@doi:10.1093/jnci/djt007; @doi:10.1158/0008-5472.CAN-13-2971; @doi:10.1016/j.cell.2016.06.017].
In addition, the CCLE data is collected and processed uniformly, as described in [@doi:10.1038/s41586-019-1186-3], while the TCGA data is processed by a uniform pipeline but collected from a wide variety of different cancer centers around the US [@doi:10.1038/ng.2764].

When we ranked cancer types in order of their generalization difficulty aggregated across genes, we noticed a slight tendency toward non-carcinoma cancer types (TGCT, SARC, SKCM) being difficult to generalize to.
It has been pointed out in other biological data types that holding out entire contexts or domains is necesssary for a full picture of performance [@doi:10.1186/s13059-020-02177-y; @doi:10.1038/s41576-021-00434-9], which our results corroborate.
This highlights a potential weakness of using TCGA's carcinoma-dominant pan-cancer data as a training set for a broad range of tasks, for instance in foundation models which are becoming feasible for some genomics applications [@arxiv:2306.15794; @doi:10.1101/2023.04.30.538439; @doi:10.1101/2023.05.29.542705].
One caveat of our analysis is that each cancer type is included in the training data or held out for a different subset of genes, so it is difficult to detangle gene-specific effects (some mutations have less distinguishable functional effects on gene expression than others) from cancer type-specific effects (some cancer types are less similar to each other than others) on prediction performance using our experimental design.



## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
