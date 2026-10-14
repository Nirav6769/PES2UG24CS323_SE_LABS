# Lab 5 — Static Code Analysis

This folder contains a cleaned version of `pet_shelter.py`, the issue log, reflection answers, a verification log, and a script to run the required analysis tools.

## Run the program

```bash
python pet_shelter.py
```

## Generate Pylint, Bandit, and Flake8 reports

```bash
bash run_analysis.sh
```

The script installs the tools and writes the three reports. If you already installed the tools into a virtual environment, you may instead run the commands below directly:

```bash
pylint pet_shelter.py > pylint_report.txt
bandit -r pet_shelter.py > bandit_report.txt
flake8 pet_shelter.py > flake8_report.txt
```

Review the generated reports and update `issues.md` to reflect the actual findings and corrected line numbers. `verification.txt` records only checks actually run while preparing this project; it is not a substitute for your analyzer reports.
