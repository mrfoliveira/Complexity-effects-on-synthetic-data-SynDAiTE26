#  Data Complexity Effects on Synthetic Data Quality, Privacy, and Utility 

This repository contains the research compendium of the Syndaite 2026 workshop paper:

Oliveira, M., Soares, C. (2026). Data Complexity Effects on Synthetic Data Quality, Privacy, and Utility. Accepted at SynDAiTE: Synthetic Data for AI Trustworthiness and Evolution Workshop at the European Conference on Machine Learning and Principles and Practice of Knowledge Discovery in Databases (ECML-PKDD 2026).

## Reproducing experiments

![Methodology diagram. Input data of varying complexity is generated and split into training and test sets. Each training set is used to train two different synthesizer models (a TVAE and a CART model). Each synthesizer then generates three synthetic samples. The synthetic samples are compared to the input data in terms of their complexity, similarity, and privacy. Finally, the utility of the synthetic samples is determined by comparing the performance of three classifiers (logistic regression, decision tree, and random forest) trained on them with that obtained from training on the original training set.](assets/methodology_diagram.png)

To obtain all results and generate a notebook containing all figures in the article, please run the notebooks in the following order:

1. **s1_generate_date** - Generate synthetic input data of varying complexity
2. **s2_fit_synthetisze** - Fit synthesizer models and generate synthetic samples
3. **s3_eval_data** - Calculate output data complexity and synthetic data quality, privacy, and utility
4. **s4_analyze_paper** - Generate analysis tables and produce paper figures

## Reference

If you use this code in your work, please cite the associated paper.