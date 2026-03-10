# AWS CodePipeline Branch Filter Demo

## Project goal

Demonstrate how AWS CodePipeline can be configured to trigger only for a specific Git branch.

This repository is used to test **branch filtering in the Source stage** of AWS CodePipeline.

---

## Architecture

Developer → GitHub → CodePipeline → Build

The pipeline is configured to trigger **only when commits are pushed to the `main` branch**.

---

## Scenario tested

1. Push to `dev` branch  
Result: Pipeline **does not start**

2. Push to `main` branch  
Result: Pipeline **starts automatically**

This confirms that **branch filtering works correctly**.

---

## Technologies used

- AWS CodePipeline
- GitHub repository
- GitHub App connection
- Branch filtering in Source stage

---

## Repository structure
dev branch → development changes main branch → production pipeline trigger
Копіювати код

---

## DevOps concept demonstrated

Branch filtering allows CI/CD pipelines to run only for specific branches.

Typical real-world setup:

feature branches → pull request → merge to main → pipeline triggers build and deploy

This prevents unnecessary pipeline executions and protects production environments.

---

## Author

Hands-on DevOps practice project.
