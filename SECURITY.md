# Security policy

## Reporting

Do not report vulnerabilities or sensitive reproduction details in public issues. Use **Security → Report a vulnerability** if private vulnerability reporting is enabled. If unavailable, use a private contact published by the maintainer; no private contact is configured by this template. Maintainers must enable private reporting or publish a monitored private channel before accepting sensitive reports.

Include affected versions or commits, impact, reproduction steps, and a suggested fix if available. Redact credentials and personal data. Coordinate disclosure with the maintainer; this template promises no response deadline or release support window.

## Maintainer setup

Define supported releases and a response policy when the project has releases. Review available secret scanning, dependency alerts, and branch protection settings. Require only checks that actually exist. Keep permissions minimal and review dependencies before adopting them.

Never commit credentials, private keys, or real environment values. Example configuration must use harmless placeholders. Ignore rules do not protect already tracked files or every secret format. If a credential is exposed, revoke or rotate it promptly, then assess cleanup and impact.
