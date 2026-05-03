# 🚀 GitOps CI/CD Workflow with Automated Quality Enforcement

## 📌 Overview

This project implements a GitOps-based development workflow designed to improve code quality, team visibility, and developer onboarding speed.

It integrates task tracking, source control, and automation to ensure that all code changes are validated through linting and testing before being merged.


## 🧱 Architecture

* **Flask API** (`app.py`) – Lightweight service with multiple endpoints
* **Pytest** (`test_app.py`) – Automated unit testing
* **GitHub Actions** – CI pipeline (Install → Lint → Test)
* **Trello** – Task tracking and workflow management


## 🔁 Workflow Design

* `main` branch remains stable at all times
* Feature branches follow: `feature/TRELLO-###-description`
* All changes go through Pull Requests
* Each PR is linked to a Trello task
* CI pipeline enforces code quality before merge


## ⚙️ CI/CD Pipeline

The pipeline runs automatically on:

* Push to feature branches
* Pull Requests to main

Stages:

1. Install dependencies
2. Lint code using flake8
3. Run tests using pytest

🚫 Any failure blocks merge into main


## 🧾 Commit Convention

All commits follow:
[TRELLO-###] Short description

Example:
[TRELLO-002] Add input validation for /sum endpoint


## 🚀 Getting Started

```bash
pip install -r requirements.txt
pytest -v test_app.py
python app.py
```


## 📄 Documentation

Detailed documentation (workflow decisions, onboarding, and engineering reasoning) is available in:
https://docs.google.com/document/d/1Lsn9Iw96NX8UejQhcAGAI7WIEIvOyOftNs4a58YjIAQ/edit?usp=sharing


## 🎯 Key Outcomes

* Enforced code quality through CI automation
* Improved team workflow visibility via GitOps
* Structured onboarding process for new developers

