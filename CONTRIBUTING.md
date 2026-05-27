# Contributing

Thank you for your interest in this project. This is an academic research repository for a Data Mining course project at Amrita Vishwa Vidyapeetham. Contributions that improve reproducibility, correctness, or extend the work are welcome.

---

## What You Can Contribute

| Type | Examples |
|------|---------|
| **Bug fixes** | Incorrect metric computation, broken notebook cells, wrong formula |
| **Reproducibility** | Fixing data path issues, environment setup problems |
| **Extensions** | Additional models (BPR, NCF, ALS), additional evaluation metrics |
| **Documentation** | Clarifications, better inline comments, improved docstrings |
| **Visualisations** | Additional plots, improved figure quality |

---

## Getting Started

### 1. Fork and Clone

```bash
# Fork via the GitHub UI, then:
git clone https://github.com/<your-username>/mars-recommender-system.git
cd mars-recommender-system
```

### 2. Set Up the Environment

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset

Download `explicit_ratings_fr.tab` and `items_fr.tab` from [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/BMY3UD), convert to `.csv`, and place them in `data/`.

### 4. Create a Branch

```bash
git checkout -b fix/metric-computation
# or
git checkout -b feature/bpr-model
```

---

## Code Standards

- **Language:** Python 3.9+
- **Style:** Follow [PEP 8](https://peps.python.org/pep-0008/). Keep lines under 100 characters.
- **Notebooks:** Every cell must produce visible output. Use descriptive cell headers as comments (e.g., `# SVD — Train/Test Split`).
- **Mathematics:** If you introduce a new formula, include the LaTeX equation in a Markdown cell immediately above the implementation cell.
- **No hardcoded paths:** Use relative paths from the repository root (e.g., `data/explicit_ratings_fr.csv`).
- **Random states:** Fix all random seeds to `42` for reproducibility.

---

## Submitting a Pull Request

1. Ensure your branch is up to date with `main`:
   ```bash
   git fetch origin
   git rebase origin/main
   ```
2. Run the full notebook from top to bottom with a clean kernel (`Kernel → Restart & Run All`) and confirm all cells execute without errors.
3. Open a Pull Request against `main` and fill in the PR template completely.
4. Reference any related Issue in your PR description (e.g., `Closes #12`).

---

## Reporting Issues

Use the Issue templates provided in `.github/ISSUE_TEMPLATE/`. Choose the appropriate template (bug report or feature request) and fill it in completely. Incomplete issues may be closed without action.

---

## Academic Integrity Note

This repository is associated with a graded academic course project. Any contribution that constitutes plagiarism, data fabrication, or academic misconduct under Amrita Vishwa Vidyapeetham's policies will be rejected and may be reported.

---

## Questions

Open a [GitHub Discussion](../../discussions) or tag `@souravmb` or `@kashyapramakrishnan` in an Issue.
