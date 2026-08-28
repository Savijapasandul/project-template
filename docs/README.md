# Using This Template

This guide explains how to turn this framework-agnostic template into a working project.

## Overview

This repository is a **template**, not an application. It provides documentation, Git conventions, and GitHub configuration without prescribing a language or framework. Your new project adds the technology stack and source code.

## Step-by-Step

### 1. Create a new repository from the template

On GitHub, open this template repository and click **"Use this template"** → **"Create a new repository"**. Choose visibility, name, and options, then create the repository.

### 2. Clone the new repository

```bash
git clone <your-repository-url>
cd <your-repository-name>
```

### 3. Remove or modify template-specific documentation

- Replace [README.md](../README.md) with your project overview
- Update [CONTRIBUTING.md](../CONTRIBUTING.md) with project-specific standards
- Update [SECURITY.md](../SECURITY.md) with your security contact
- Replace [LICENSE](../LICENSE) with your chosen license
- Adjust or remove this docs page when no longer needed

### 4. Select your technology stack

Choose languages, frameworks, and tools for your project. Examples:

- Python + FastAPI or Django
- TypeScript + Node.js + Express
- React or Next.js for frontends
- Go, Rust, or other stacks as appropriate

Add the corresponding source directories and configuration files.

### 5. Add framework-specific tooling

Depending on your stack, you may add:

- Package manifests (`package.json`, `pyproject.toml`, `go.mod`, etc.)
- Linters and formatters
- Test frameworks
- Build tools

Extend [.editorconfig](../.editorconfig) with language-specific rules if needed.

### 6. Configure environment variables

- Document required variables in `.env.example` (committed)
- Store real values in `.env` or your deployment platform (never committed)
- Review [.gitignore](../.gitignore) — secrets and local env files are already ignored

### 7. Configure CI/CD

The default workflow ([template-validation.yml](../.github/workflows/template-validation.yml)) validates template structure only.

After adding your stack:

- Add jobs for build, test, and lint
- Replace or extend the validation workflow
- Configure deployment workflows when ready

### 8. Begin development

- Create feature branches following [CONTRIBUTING.md](../CONTRIBUTING.md)
- Use issue and PR templates for consistent collaboration
- Keep documentation updated as the project evolves

## Extending Dependabot

The template configures Dependabot for **GitHub Actions** only. After adding dependency manifests, extend [.github/dependabot.yml](../.github/dependabot.yml) with ecosystems such as:

- `npm` or `docker` for Node.js projects
- `pip` for Python projects
- `gomod` for Go projects

See [Dependabot configuration options](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file).

## Related Documentation

- [README](../README.md) — Project overview and post-template checklist
- [CONTRIBUTING](../CONTRIBUTING.md) — Contribution guidelines
- [SECURITY](../SECURITY.md) — Security policy
