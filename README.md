# Host-Identification-Project

Host attribution of *Salmonella* Typhimurium from cgMLST allele profiles (EnteroBase), using a Random Forest.

## Contents

- `salmonella_host_pipeline.ipynb`: the full pipeline, step by step: load → check → clean → label → cap per HC20 cluster → model → cross-validate (random vs. grouped) → measure → test for confounders (country).

## How to run

1. Install the libraries:
   ```
   pip install pandas numpy scikit-learn matplotlib jupyter
   ```
2. Put the two EnteroBase exports in a folder called `data/` next to the notebook:
   `Allele_Profiles_FR.txt` and `Metadata_FR.txt`.
3. Open the notebook (e.g. in VS Code with the Python and Jupyter extensions) and run the cells top to bottom.

The `data/` folder is not uploaded to GitHub (see `.gitignore`).
