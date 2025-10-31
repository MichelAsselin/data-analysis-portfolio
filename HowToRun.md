```markdown
# How to run — Superstore_Profitability_Analysis

Quick summary
- The notebook expects `Sample - Superstore.csv` (Sample Superstore dataset) to be placed in the repo root or in a `data/` folder. Download it manually from:
  https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

1) Clone repo
```bash
git clone https://github.com/MichelAsselin/data-analysis-portfolio.git
cd data-analysis-portfolio
```

2) Place the dataset
- Save the CSV as either `Sample - Superstore.csv` (repo root) or `data/Sample - Superstore.csv`.
- Do NOT commit the dataset if redistribution is restricted; instruct reviewers to download it manually.

3) Create & activate a virtual environment
```bash
python -m venv venv
# macOS / Linux
source venv/bin/activate
# Windows
venv\Scripts\activate
```

4) Install dependencies
```bash
pip install -r requirements.txt
```

5) Open the notebook
- Local: `jupyter lab` or `jupyter notebook` then open `Superstore_Profitability_Analysis.ipynb`.
- Colab: use the "Open in Colab" link at the top of the notebook. In Colab, upload the CSV (left pane -> Files -> Upload) or mount Drive and update the csv_path.

6) Run the notebook
- Kernel → Restart & Run All to ensure it runs top-to-bottom with no hidden state.

7) Optional: render to HTML for sharing
```bash
jupyter nbconvert --to html Superstore_Profitability_Analysis.ipynb
```

8) Clean outputs before committing (recommended)
- Clear outputs in-place:
```bash
jupyter nbconvert --clear-output --inplace Superstore_Profitability_Analysis.ipynb
```
- Or install/use nbstripout so outputs are removed automatically on commit:
```bash
pip install nbstripout
nbstripout --install
```
