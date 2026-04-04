# Getting Started

## Environment Setup
1. Install Python 3.14
2. Install Git
3. Install VS Code (optional)

## Running Tests
- `pytest -v test_app.py`

## Branch Workflow
1. Checkout main: `git checkout main`
2. Pull latest: `git pull origin main`
3. Create feature branch: `git checkout -b feature/TRELLO-###-description`
4. Make changes, commit, push

## PR Creation
- Open PR on GitHub
- Link Trello card
- Wait for CI green build

## Troubleshooting
- Failed lint: fix formatting with flake8 rules
- Failed test: check logic and rerun tests
