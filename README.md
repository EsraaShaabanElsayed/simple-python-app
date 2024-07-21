# Simple Python Application with GitHup Actions CI/CD

## Overview

This repository contains a simple Python application with an automated CI/CD pipeline set up using GitHub Actions. The pipeline is designed to run tests automatically whenever changes are pushed to the repository.

## Project Structure

```
simple-python-app/
├── app.py
├── test_app.py
├── requirements.txt
└── .github/
    └── workflows/
        └── ci-cd-pipeline.yml
```

### Files

- **app.py**: Contains the main Python application code.
- **test_app.py**: Includes test cases for the application functions.
- **requirements.txt**: Lists the Python dependencies.
- **.github/workflows/ci-cd-pipeline.yml**: GitHub Actions workflow configuration.

## Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/simple-python-app.git
   cd simple-python-app
   ```

2. **Install Dependencies:**

   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Run Tests Locally:**

   ```bash
   pytest test_app.py
   ```

## GitHub Actions Workflow

The CI/CD pipeline is defined in `.github/workflows/ci-cd-pipeline.yml`. It includes the following stages:

- **Checkout Code**: Clones the repository.
- **Set Up Python**: Sets up Python environment.
- **Install Dependencies**: Installs project dependencies.
- **Run Tests**: Executes tests using `pytest`.


