# Azure DevOps CI Pipeline Demo

## What this is

A simple Python calculator app with a CI pipeline built in Azure DevOps. This is one of my first hands-on DevOps projects, built to learn how pipelines work in practice.

## What the pipeline does

```
GitHub Push → Install dependencies → Lint with flake8 → Run tests → Publish results
```

## What I learned

- How to write a YAML pipeline and connect it to a GitHub repository
- Self-hosted agents run as a service on your own machine — no VM is created
- Calling `python -m pytest` instead of `pytest` directly avoids PATH issues on Windows agents
- flake8 catches code style issues before tests even run

## Tech used

- Python, pytest, flake8
- Azure DevOps Pipelines
- Self-hosted Windows agent

## Screenshots

![Pipeline summary](screenshots/pipeline-summary.jpg)
![Test results](screenshots/pipeline-tests.jpg)
![Code coverage](screenshots/pipeline-coverage.jpg)