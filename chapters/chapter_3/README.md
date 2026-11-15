# Chapter 3: Getting started

## Introduction

- [01_SimulatedDataset.ipynb](01_SimulatedDataset.ipynb): describes a simple simulator for payment card transaction data. Although simplistic, the simulator provides a sufficiently challenging setting to approach a typical fraud detection problem. In particular, the simulator will allow to generate datasets that i) are highly unbalanced (low proportion of fraudulent transactions), ii) contain both numerical and categorical variables (with categorical features that have a very high number of possible values), and iii) feature time-dependent fraud scenarios.
- [02_BaselineFeatureTransformation.ipynb](02_BaselineFeatureTransformation.ipynb) and [03_BaselineModeling.ipynb](03_BaselineModeling.ipynb) address the two main steps of a standard predictive modeling process: Feature transformation, and predictive modeling. These sections will provide some baseline strategies for performing meaningful feature transformations, and build a first predictive model whose accuracy will serve as a reference in the rest of the book.
- [04_Baseline_RealWorldData.ipynb](04_Baseline_RealWorldData.ipynb): applies this baseline methodology (feature transformation and predictive modeling) to a real-world dataset of card transactions and illustrate its ability to effectively detect fraudulent transactions.

## Summary

This chapter illustrated that the design of a baseline fraud detection system can be achieved using simple preprocessing strategies, and standard machine learning classifiers. In particular, we managed to obtain fraud detection performances that are well above those of a random classifier.

The chapter however only scratched the surface of how to approach a fraud detection problem. As we will see, a large number of more advanced techniques can be used to improve the performances. Performances can be addressed in terms of fraud detection accuracies, but also in terms of computational requirements (memory/execution times). The latter is in practice important during training, as fraud detection systems must deal with large amounts of data and also during inference for real-time or near real-time processing. One must generally carefully considers tradeoffs between accuracy and computational requirements.