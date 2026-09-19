# Non-Parametric Test Prediction

An academic notebook exploring how natural-language problem descriptions can guide the selection and execution of non-parametric statistical tests.

## What it contains

- TF-IDF text features and a decision-tree classifier for test selection.
- Implementations for runs, Wilcoxon signed-rank, and Mann–Whitney tests.
- Individual experiments and a combined workflow in the final code cell.

## Stack

Python, pandas, NumPy, SciPy, scikit-learn, and Jupyter.

## Project status

This is a research prototype, not a validated statistical calculator. The original saved classifier evaluation reported 0.9259 accuracy on 27 examples; this result has not been reproduced here and should not be interpreted as a general performance guarantee. Saved notebook outputs were removed for a clean review copy.

The Wilcoxon decision logic requires correction and comparison with SciPy before results should be relied on. Dataset-dependent evaluation remains pending.

## Required data

The original notebook references these files, which are not included:

- `Non_Parametric_combined.csv`
- `ARJ SIR DATASET.xlsx`
- `runs_test_critical_values_complete.csv`
- `z_table_complete.csv`
- `p_critical_values.csv`

The notebook currently uses `/content/` paths from Google Colab. Supply the original data and update those paths for your environment. Do not run all cells until the data and test logic have been checked.

## Local setup

```sh
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab notebooks/statistical_test_prediction.ipynb
```

Dependencies are listed from imports and are not yet version-pinned through a reproduced environment.

## Author

Harshil Prashant Shah · [Portfolio](https://harshil-prashant-shah.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/harshilpshah/)
