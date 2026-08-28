# Contributing

Thank you for your interest in contributing. This guide applies to repositories created from this template and can be adapted as your project grows.

## Development Workflow

1. **Discuss** significant changes via an issue or discussion before large work, when practical.
2. **Branch** from the default branch (`main` or your project's equivalent).
3. **Implement** focused changes with clear commits.
4. **Test** your changes using the project's test suite (add tests when introducing new behaviour).
5. **Document** user-facing or setup changes.
6. **Open a pull request** using the PR template and respond to review feedback.

## Branch Naming

Use short, descriptive branch names with a type prefix:

| Prefix | Use for |
|--------|---------|
| `feature/` | New features or enhancements |
| `fix/` | Bug fixes |
| `docs/` | Documentation only |
| `refactor/` | Code changes that neither fix bugs nor add features |
| `test/` | Test additions or corrections |
| `chore/` | Maintenance, tooling, dependencies |
| `ci/` | CI/CD configuration |

Examples: `feature/add-export`, `fix/login-timeout`, `docs/update-setup-guide`

## Commit Conventions

We recommend a conventional commit style for clarity and changelog generation:

| Prefix | Description |
|--------|-------------|
| `feat:` | A new feature |
| `fix:` | A bug fix |
| `docs:` | Documentation only |
| `refactor:` | Code change that neither fixes a bug nor adds a feature |
| `test:` | Adding or updating tests |
| `chore:` | Maintenance, tooling, or non-user-facing changes |
| `ci:` | CI/CD configuration changes |

Examples:

```
feat: add user authentication endpoint
fix: handle empty input in parser
docs: clarify environment variable setup
```

Projects may adapt or replace this convention (e.g. issue references, scope prefixes) as needed. Consistency within a repository matters more than the exact format.

## Pull Requests

- Keep PRs focused — one logical change per PR when possible
- Fill out the pull request template completely
- Link related issues when applicable
- Ensure CI checks pass before requesting review
- Update documentation for behaviour or setup changes
- Be responsive to review feedback

## Code Quality

Quality standards depend on your chosen language and framework. After adopting a stack, consider:

- Linters and formatters (e.g. ESLint, Ruff, golangci-lint)
- Type checking where applicable
- Consistent naming and module structure
- Meaningful names and small, readable functions

Document project-specific standards in this file or a linked style guide.

## Testing

- Add tests for new features and bug fixes when a test suite exists
- Run the full test suite locally before opening a PR
- Do not merge failing tests without team agreement and documentation

This template does not include tests by default. Add testing guidance here after setting up your framework.

## Documentation

- Update README and docs when setup, APIs, or behaviour changes
- Keep examples accurate and runnable
- Use clear, concise language
- Fix typos and broken links when you notice them

## Security

- **Never** commit secrets, API keys, passwords, or private keys
- **Never** include sensitive data in issues or pull requests
- Report security vulnerabilities privately (see [SECURITY.md](SECURITY.md))
- Review dependency updates for security implications

## Keeping Changes Focused

- Avoid mixing unrelated changes in one PR
- Prefer incremental, reviewable commits
- Remove debug code and commented-out blocks before merging
- Do not reformat entire files unrelated to your change unless that is the purpose of the PR

## Questions

Open an issue for questions about contributing, or reach out to the maintainers through your project's preferred channel.
