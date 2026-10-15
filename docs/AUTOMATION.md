# Optional automation

Automation is off by default. The included `Manual repository check` has only a manual trigger and requires the repository variable `ENABLE_ACTIONS` to equal `true` before a runner is allocated. Pushes, pull requests, and schedules cannot trigger it. No Dependabot updater is configured.

The template repository also has Actions disabled in its GitHub settings. Repository settings and variables are not inherited by generated repositories; the workflow guard provides the portable default. Keep `ENABLE_ACTIONS` unset in new projects until you want automation.

## Enable deliberately

1. In the generated repository, open **Settings → Actions → General** and allow Actions if disabled.
2. Open **Settings → Secrets and variables → Actions → Variables** and create a repository variable named `ENABLE_ACTIONS` with value `true`.
3. Open **Actions → Manual repository check → Run workflow** and select your branch.

The check uses one Ubuntu runner with a three-minute job timeout, read-only contents access, and no third-party actions. It fetches the selected commit and checks whitespace in that commit. It does not build, test, render, export, or deploy your project. Add real project checks when useful; document prerequisites in CONTRIBUTING.md. Timeout limits job duration, not an account-wide spending cap. Manual runs still consume applicable minutes.

To stop execution again, remove `ENABLE_ACTIONS` or disable Actions in repository settings. Cancel any already-running jobs separately. Review GitHub billing budgets before adding automatic triggers, matrices, artifacts, or paid runners.

For software, add the chosen build/test commands; for KiCad or Blender, use the appropriate validation/export tools only when needed. Keep large generated artifacts and credentials out of Git. Use Git LFS selectively for large source assets after confirming storage and bandwidth needs.
