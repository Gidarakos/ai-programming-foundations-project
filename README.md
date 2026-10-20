# AI Programming Foundations: Bank Telemarketing Data Workflow

Author: Lampros Gidarakos. Repository: https://github.com/Gidarakos/ai-programming-foundations-project

A reproducible cleaning and exploratory-analysis workflow for the UCI Bank Marketing data (`bank-additional-full.csv`).

## Contents
- `data_workflow.ipynb` – the executed notebook (load → audit → clean → EDA → export)
- `module_summary.pdf` – project report
- `data/bank-additional-full.csv` – raw data, unchanged (SHA-256 `74adfc578bf77a7ff4bb1ba4a9f8709d9e3c6907342959c2c8416847e0afb4d8`)
- `figures/` – the three figures used in the report
- `requirements.txt` – pinned package versions

## How to run
```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter nbconvert --to notebook --execute --inplace data_workflow.ipynb   # or open it in Jupyter and Run All
```
Running the notebook recreates `figures/*.png` and writes the cleaned table to `data/bank_clean.csv`.
