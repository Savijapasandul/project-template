name: Bug Report
about: Report a bug or unexpected behaviour
title: "[Bug]: "
labels: bug
assignees: []
body:
  - type: markdown
    attributions: []
    value: |
      Thanks for taking the time to report a bug. Please provide as much detail as possible to help us reproduce and fix the issue.

  - type: textarea
    id: description
    attributes:
      label: Description
      description: A clear and concise description of the bug.
      placeholder: What went wrong?
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      description: Steps to reproduce the behaviour.
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. See error
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected Behaviour
      description: What you expected to happen.
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: Actual Behaviour
      description: What actually happened.
    validations:
      required: true

  - type: textarea
    id: environment
    attributes:
      label: Environment
      description: Relevant environment details (OS, runtime version, browser, etc.).
      placeholder: |
        - OS:
        - Version:
        - Browser (if applicable):
    validations:
      required: false

  - type: textarea
    id: logs
    attributes:
      label: Relevant Logs / Screenshots
      description: Paste logs or add screenshots. Do not include secrets or credentials.
    validations:
      required: false

  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Any other context about the problem.
    validations:
      required: false
