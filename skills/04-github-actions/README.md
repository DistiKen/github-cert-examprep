# GitHub Actions

## Exam focus

This repository helps practice automated workflows and CI checks used in GitHub certification scenarios.

## Practice tasks

1. Create a `.github/workflows` directory.
2. Add a workflow that runs on every push and pull request.
3. Include a job that checks out the repo and runs a simple command such as `echo` or a test script.
4. Confirm the workflow passes in the Actions tab.

## Example workflow

```yaml
name: CI Demo

on:
  push:
  pull_request:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run a simple check
        run: echo "GitHub Actions is working!"
```

## Skills practiced

- Workflow automation
- CI/CD fundamentals
- GitHub Actions syntax
- Validation and review
