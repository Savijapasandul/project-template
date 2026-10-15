# Getting started

1. Create a repository using GitHub's **Use this template** button. Use the new repository's clone URL with Git or your preferred client; work in the cloned directory.
2. Replace the root README with project purpose, prerequisites, setup, usage, and support. Resolve licensing; the existing placeholder grants no reuse rights.
3. Configure private vulnerability reporting or a private contact and update the security policy. Adapt contribution and agent guidance to your team.
4. Add only the source layout, dependencies, and tooling the project needs. No particular stack or directory layout is required. Commit appropriate lockfiles.
5. Add precise ignore rules for generated output and local secrets. Check representative source and asset paths remain tracked. Adjust editor rules to match your tools.
6. Document configuration using harmless placeholders. Never put real credentials in examples, screenshots, logs, or commits.
7. Introduce meaningful tests and document exact local commands and prerequisites in the contribution guide. Do not require nonexistent checks.
8. Keep automation off until needed. Follow [Actions setup](AUTOMATION.md) to enable the included manual check. Add project-specific tests or exports only after choosing tools; select automatic triggers and budgets deliberately.
9. Add Dependabot configuration only after dependency manifests or action dependencies exist. Select actual ecosystems and directories, and a suitable update cadence. There is no default scheduled updater.
10. Replace architecture notes with real decisions, reset the changelog, and remove this guide and other template-specific text once setup is complete. Repair links after removing files.

## Repository settings

Settings do not transfer simply because configuration files exist. Review visibility, default branch, access, private reporting, secret scanning availability, dependency alerts, and protection rules. Enable **Template repository** only if the generated repository itself should serve as a template. No workflow or deployment needs to run during initialization.
