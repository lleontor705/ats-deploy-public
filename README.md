# ATS Deploy — Public Reusable Workflows

Public CI/CD reusable workflows for ATS open-source projects.

## Available Workflows

| Workflow | Description |
|----------|-------------|
| `quality-node.yml` | Node.js quality gate (lint, typecheck, test) |
| `quality-go.yml` | Go quality gate (golangci-lint, test, coverage) |
| `quality-dotnet.yml` | .NET quality gate (build, test) |
| `security-scan.yml` | Trivy filesystem + secret scan |

## Usage

```yaml
jobs:
  quality:
    uses: lleontor705/ats-deploy-public/.github/workflows/quality-node.yml@main
  security:
    uses: lleontor705/ats-deploy-public/.github/workflows/security-scan.yml@main
```

Private repos should use `lleontor705/ats-deploy` instead.
