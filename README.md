# COMP3104_Group63_Assignment

## Group Members
•⁠  ⁠*Leader:*Milan Patel(101397631)-https://github.com/Milan-p23
•⁠  ⁠*Member 1:*Parthkumar Patel(101399114)-Github: https://github.com/Parth-2601
•⁠  ⁠*Member 2:* Deep Patel(101415117)-Github: https://github.com/Deeppatel91
•⁠  ⁠*Member 3:* NeerajKumar (1011415118) - https://github.com/NeerajBudhiraja1807
•⁠  ⁠*Member 4:* Mohmadsahil Shaikh -101413469-sahils777 
GitHub link: https://github.com/sahils777

## Project Description
This repository contains the group assignment for the COMP3104 DevOps course. The assignment focuses on collaborative Git workflows, branching strategies, and CI/CD integration using GitHub Actions. Each member contributes to the project through individual branches that are later merged into the main branch, ensuring continuous integration and collaboration.

## Objectives
- Implement Git branching strategies and best practices.
- Set up continuous integration (CI) using GitHub Actions.
- Maintain version control and collaboration using Git and GitHub.
- Demonstrate teamwork through commits, pull requests, and merging.

# CI/CD Pipeline

This repository is integrated with GitHub Actions to automate testing and builds on every push event. The CI/CD pipeline is defined in the .github/workflows/ci.yml file and includes the following steps:

1. *Clone the Repository*: The pipeline checks out the code from the repository.
2. *Set Up the Environment*: It sets up the environment on an Ubuntu server.
3. *Run Basic Checks*: The pipeline runs checks on branch changes, including file integrity and repository structure.
4. *Display Job Statuses*: Job statuses and relevant outputs are displayed.

This automation ensures that code pushed to the repository is automatically validated through continuous integration, improving code quality and collaboration.

## GitHub Actions CI Workflow

The GitHub Actions workflow is designed to trigger automatically on every push to any branch, helping maintain a functional, conflict-free repository. Below is an example configuration found in the .github/workflows/ci.yml file:

```yaml
name: GitHub Actions CI

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run CI Pipeline
        run: |
          echo "CI pipeline triggered for ${GITHUB_REF}"
          # Add additional commands for testing and building the project.
```

## How It Works

- *Triggering the Workflow*: The workflow is automatically triggered by a push event to any branch.
- *Running on Ubuntu*: The pipeline runs on the latest version of Ubuntu.
- *Checkout Action*: The actions/checkout@v4 action is used to check out the repository code.
- *CI Pipeline Execution*: The pipeline runs and outputs a message that includes the reference of the triggered event.

## Customization

You can customize the workflow by adding commands in the run section to include specific testing, linting, or build commands necessary for your project.=
