# Medication Prescription Association-Rule Mining

Analyzes hospital prescription records as transaction baskets to discover medications that frequently occur together. The notebook cleans drug names, groups prescriptions by admission, applies Apriori, filters association rules, and visualizes the strongest patterns.

## Workflow

1. Load and standardize `PRESCRIPTIONS.csv`.
2. Remove very rare medications and build one basket per admission.
3. One-hot encode the baskets and mine frequent itemsets with Apriori.
4. Generate and filter rules using support, confidence, and lift.
5. Export charts for the most important medications and rules.

## Data Requirements

- `PRESCRIPTIONS.csv` — hospital prescription records with admission and medication fields.

Datasets and generated artifacts are not included unless they are embedded directly in the notebook.

## Requirements

- pandas
- NumPy
- mlxtend
- Matplotlib
- Seaborn

Install missing packages in your Jupyter or Google Colab environment before running the notebook.

## Running the Notebook

1. Open [`4dataminingtechniques.ipynb`](4dataminingtechniques.ipynb) in Jupyter Notebook or Google Colab.
2. Place any required data files in the path expected by the notebook.
3. Update local or Google Drive paths where needed.
4. Run the cells from top to bottom.

## Outputs

- Top-medication frequency chart
- Support-versus-confidence scatter plot
- Top-lift rule chart
- Rule-metric distribution figure

## Repository Contents

```text
.
|-- README.md
`-- 4dataminingtechniques.ipynb
```

## Notes

- This repository preserves the analysis as a notebook-first educational project.
- Results may vary with dataset versions, random splits, package versions, and available hardware.
- Review file paths and runtime-specific commands before executing outside Google Colab.
