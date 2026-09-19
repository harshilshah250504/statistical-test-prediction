# Validation notes

## Classifier reproduction — 19 September 2026

The initial notebook classifier was reproduced with the supplied `Non_Parametric_combined.csv`, preserving its split and model settings: test size 0.25, split random state 16, TF-IDF unigrams/bigrams with English stop words, and a decision tree with random state 42.

- Dataset: 107 records.
- Training: 80 records; test: 27 records.
- Correct predictions: 25 of 27 (92.59%).
- Exact duplicate questions: 23 duplicate rows beyond their first occurrences.
- One distinct question appears in both training and test sets.

This reproduces the original split, not a leakage-free estimate of generalization. Deduplication or grouping equivalent questions before splitting is required for a stronger evaluation. No claim is made that all statistical execution functions are correct; those remain under review.

Environment: Python 3.12, scikit-learn 1.9.1. Raw data is not distributed.
