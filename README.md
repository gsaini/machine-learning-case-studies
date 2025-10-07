# Machine Learning (ML)

This repository is a personal collection of machine-learning case studies, study materials, notebooks, datasets, and small projects. Its goal is to be a practical workspace where you (and contributors) can learn, reproduce experiments, and share compact case-study examples that demonstrate common ML concepts and workflows.

## Repository intent

- Host self-contained case studies that demonstrate end-to-end ML workflows (data, notebooks, models, evaluation).
- Keep reference materials and short tutorials that complement the case studies.
- Use an organized folder layout so each case study is easy to run locally or convert into a short tutorial.

This repo is meant for learning, teaching, and lightweight reproducible examples — not for production model deployments.

## Recommended structure

The repository follows a simple convention so it's easy to find and add content:

- `case-studies/` — one folder per case study. Example: `case-studies/anime-rating-case-study`.
- `reference-material/` — papers, PDFs, FAQs and other external references.
- `README.md` — repository-level documentation and frequently asked questions.

Each case-study folder should ideally contain:

- `README.md` — short summary, how to run, data sources, and expected outputs.
- `notebooks/` or `.ipynb` — Jupyter notebooks that reproduce the core analysis.
- `data/` or CSV files (or pointers to download scripts) — small datasets or scripts to fetch larger datasets.
- `requirements.txt` or `environment.yml` (optional) — dependencies for reproducibility.

## How to add a new case study

1. Create a new folder under `case-studies/` with a descriptive name (kebab-case). Example:

```bash
case-studies/my-new-case-study/
```

1. Add a short `README.md` that explains the data, steps, and how to run the analysis.
1. Add notebooks and small datasets (or download scripts). Keep datasets small or provide links to hosted data.
1. Optionally add `requirements.txt` so others can recreate the environment.

If the content should remain synced with a separate Git repository, prefer adding it as a git submodule. Example (already used in this repo):

```
git submodule add https://github.com/gsaini/anime-rating-case-study case-studies/anime-rating-case-study
```

## Contributing

- Open an issue if you want to propose a new case study or need help.
- Create a fork and a topic branch for your changes. Keep each PR focused (one case study or one doc update).
- Add or update `README.md` inside the case-study folder to document how to run the notebook(s).
- Small data files (< 50MB) can be committed directly. For larger datasets, include a download script and instructions.

## Reproducibility & running examples

- Use virtual environments (venv, conda) and install dependencies listed in the case-study's `requirements.txt` or in a shared `environment.yml`.
- To run notebooks locally, install `jupyter` or `jupyterlab` and open the notebook.

Example (macOS / zsh):

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r case-studies/<your-case-study>/requirements.txt
jupyter lab
```

## License & notes

This repository contains examples and learning materials. Check each case-study for license notes on data and code. If you reuse large datasets, ensure you comply with their license and attribution requirements.

## Reference Materials

- [A guide on how to compare different models](https://people.duke.edu/~rnau/compare.htm)

- [Document that explains what are decision tree, their working, and different impurity measures](https://tanthiamhuat.files.wordpress.com/2015/10/decision-tree-tutorial-by-kardi-teknomo.pdf)

- [Sklearn - Decision Tree documentation [Documentation of decision trees that gives very concise information on the advantages and disadvantages of the Decision tree along with practical use case and mathematical formulation behind the algorithm]](https://scikit-learn.org/stable/modules/tree.html)

- [An article that explains why and how class weights are used and also sheds light on how to find and assign class weights](https://machinelearningmastery.com/cost-sensitive-decision-trees-for-imbalanced-classification/)