# Contributing

Keep changes focused and use clear commit messages. Discuss substantial changes when useful; branch naming, review requirements, and release practices should fit the project and team, including solo development.

Read the repository documentation and existing conventions before editing. Add dependencies only when justified. Update documentation when setup or behavior changes. Use issues and pull requests when helpful, and link related discussions.

## Validation

This template has no runtime or test suite. For template changes:

- Check relative Markdown links and file references.
- Parse issue-form YAML with an available local YAML parser and check GitHub form fields, unique IDs, and required inputs.
- Use `git diff --check` to catch whitespace errors.
- Inspect ignore behavior with `git check-ignore -v --no-index PATH` and attributes with `git check-attr text eol -- PATH`.
- Review the diff for secrets, overly broad ignore rules, broken instructions, and accidental automation.

Once a project has tooling, document exact setup and relevant test commands here. Run applicable checks and report what passed, failed, or could not run. Do not claim unperformed testing. Reviewers should assess scope, correctness, security, documentation, and validation evidence.

Never include secrets in commits, logs, issues, or review comments. See [SECURITY.md](SECURITY.md) for private reporting.
