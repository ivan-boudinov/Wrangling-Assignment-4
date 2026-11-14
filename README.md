# ROC on Adult, German and COMPAS

Reproduction of Reject Option based Classification (Kamiran, Karim and Zhang, 2012). Open `roc_fairness_code.ipynb` and run all cells; it compares fairness and accuracy before and after ROC.

## Data 

| File | Used for |
|---|---|
| `adult.csv` | Predict income > 50K; deprived group: female |
| `german.data` | Predict good credit; deprived group: female (A92) |
| `compas-scores-two-years.csv` | Predict no recidivism within 2 years; deprived group: African-American |

## Code notes

- Needs Python 3 with numpy, pandas, scikit-learn and jupyter.
- Logistic regression, stratified 60/20/20 split, random seed 42.
- The threshold is chosen on the validation set; results are reported on the test set.
