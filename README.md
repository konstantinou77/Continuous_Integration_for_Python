# Python CI Pipeline with GitHub Actions

# Project Overview:

This project implements a CI workflow for a Python application using GitHub Actions.
The pipeline runs tests, generates code coverage reports, checks code style and
complexity, and uploads source code as an artifact. It is triggered on pushes
and pull requests to the main and develop branches.

# Tech Stack:

- Python (configurable via matrix or environment variable)
- pytest (for running tests)
- coverage (for test coverage)
- flake8 (for linting and complexity checks)
- GitHub Actions (CI)

# What was done:

- Created python-ci job that runs:
  - Unit tests using pytest
  - Coverage report with coverage
  - Code style check with flake8
  - Code complexity check with flake8

- Coverage report is printed in the console
- Python source code is uploaded as an artifact.

- The workflow is triggered on:
  - Push to main and develop
  - Pull request to main
  
- Workflow run name includes:
  - GitHub user who triggered the job
  - Commit hash that triggered the workflow

# Link to the successful GitHub Actions run:
https://github.com/konstantinou77/devops_todolist_cicd_task_2_python_ci/actions/runs/15443817526

