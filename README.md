# Python CI Example Project

This project demonstrates a basic CI setup using GitHub Actions.

## Setup

1. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install development dependencies:
   ```bash
   pip install -r requirements-dev.txt
   ```

3. Run tests:
   ```bash
   pytest tests/
   ```

## CI Pipeline

The CI pipeline runs on push to main and pull requests:
- Runs tests on Python 3.8, 3.9, and 3.10
- Checks code coverage
- Runs linting with flake8