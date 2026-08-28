# Security Policy

## Supported Versions

Security support depends on how maintainers choose to version and support the project after adopting this template. Update this section with your release and support policy once your project has defined versions.

## Reporting a Vulnerability

**Do not report security vulnerabilities through public GitHub issues.**

If you discover a security issue, report it privately to the repository maintainers. Configure a security contact in your GitHub repository settings (Settings → Security → Code security and analysis → Private vulnerability reporting) and reference that contact here once it is set up.

Include as much detail as possible:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

Maintainers will acknowledge receipt and work with you on a responsible disclosure timeline.

## Security Expectations for Contributors

All contributors must follow these practices:

### Do not commit secrets

- API keys, tokens, and passwords
- Private keys and certificates (`.pem`, `.key`, etc.)
- Database connection strings with credentials
- Cloud provider access keys
- Local environment files (`.env`, `.env.local`)

Use environment variables or a secrets manager. Provide `.env.example` with non-sensitive placeholders only.

### Do not expose credentials in issues or pull requests

- Never paste secrets into GitHub issues, PR comments, or commit messages
- Redact sensitive information from logs and screenshots
- Rotate any credential that was accidentally exposed

### Keep dependencies updated

- Review Dependabot and security advisories regularly
- Apply security patches promptly
- Audit new dependencies before adding them

### Follow secure development practices

- Validate and sanitize input
- Use least-privilege access for services and credentials
- Enable GitHub secret scanning and branch protection where appropriate

## Security Configuration Recommendations

After creating a project from this template, consider enabling:

- GitHub Dependabot alerts
- Secret scanning (if available for your repository)
- Branch protection on the default branch
- Required status checks for CI
- Private vulnerability reporting

## Additional Resources

- [GitHub Security Best Practices](https://docs.github.com/en/code-security/getting-started/github-security-features)
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)
