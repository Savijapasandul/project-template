name: Feature Request
about: Suggest a new feature or enhancement
title: "[Feature]: "
labels: enhancement
assignees: []
body:
  - type: markdown
    attributions: []
    value: |
      Thanks for suggesting an improvement. Describe the problem and your proposed solution below.

  - type: textarea
    id: problem
    attributes:
      label: Problem
      description: Is your feature request related to a problem? Please describe.
      placeholder: I'm always frustrated when...
    validations:
      required: true

  - type: textarea
    id: solution
    attributes:
      label: Proposed Solution
      description: Describe the solution you'd like.
    validations:
      required: true

  - type: textarea
    id: alternatives
    attributes:
      label: Alternatives Considered
      description: Describe any alternative solutions or features you've considered.
    validations:
      required: false

  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Add any other context, mockups, or examples about the feature request.
    validations:
      required: false
