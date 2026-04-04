# GitOps Capstone Project

## Project Overview
This project demonstrates a GitOps workflow with Trello, GitHub, and GitHub Actions. 
It automates linting, testing, and onboarding for new developers.

## Architecture
- **app.py** → Flask API
- **test_app.py** → Unit tests with pytest
- **.github/workflows/ci.yml** → CI pipeline (Install → Lint → Test)

## Workflow Description
- Branch strategy: `main` = stable, feature branches = TRELLO-###
- PRs required for merge, linked to Trello cards
- CI pipeline ensures quality (lint + test)
- Minimum 3 PRs, 8 commits

## Commit Conventions
- `[TRELLO-###] Short description` format
- Example: `[TRELLO-002] Add input validation for /sum endpoint`

## Setup Instructions
1. Install Python 3.14
2. Install dependencies: `pip install -r requirements.txt`
3. Run tests: `pytest -v test_app.py`
4. Run the app: `python app.py`# gitops-capstone-project
DevOps GitOps workflow with CI/CD automation
