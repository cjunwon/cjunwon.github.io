---
title: "Synthetic Survey Data Generation and Evaluation"
collection: publications
permalink: /publication/2025-07-20-Synthetic-Survey-Data-Generation-and-Evaluation
excerpt: 'An end-to-end evaluation of five synthetic data generation methods for survey microdata using utility, fidelity, and privacy metrics.'
date: 2025-07-20
venue: 'Proceedings of the 31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD ’25)'
paperurl: 'https://doi.org/10.1145/3690624.3709421'
citation: 'Jiang, Y., Liang, S., & Choi, J. (2025). <i>Synthetic Survey Data Generation and Evaluation.</i> In <i>Proceedings of the 31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining</i> (pp. 2292–2302). ACM. https://doi.org/10.1145/3690624.3709421'
---

**Abstract**

Survey data are common and invaluable in social science research for understanding population processes and supporting policymaking and planning. Depending on the nature and scale, survey data sharing comes with privacy risks, and data collectors and agencies are constrained by disclosure permissions, limiting usage across research groups and institutes. Previous methods for synthetic data generation and deidentification may not entirely prevent information disclosures, or they may sacrifice data quality and granularity.

Using a large-scale national voter file at both national and state levels, this paper introduces an end-to-end pipeline to streamline synthetic data generation and evaluation for survey researchers. This study selects four generative approaches based on different statistical assumptions: the regression-based Synthpop, the generative deep learning-based CTGAN and TVAE, and the large language model-based REaLDTabFormer, and compares them to the baseline synthetic minority oversampling technique (SMOTE). We consider three key dimensions of evaluation (utility, fidelity, and privacy) to highlight the strengths and weaknesses of each approach, and systematically evaluate across various datasets and training sizes. The results reveal that Synthpop is optimized for general utility (i.e., fidelity), while TVAE excels in downstream applications (i.e., target-specific utility) but compromises on general utility and potentially risks data overfitting. REaLDTabFormer demonstrates a balanced performance in both general and target-specific utility, whereas CTGAN offers the best privacy protection. We recommend that future researchers select a generative method by considering the trade-offs between performance across various evaluation dimensions, training size, data type, and computational infrastructure.