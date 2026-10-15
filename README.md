# Project Template

A minimal, technology-neutral starting point for projects. Use it when you need documentation, contribution guidance, and GitHub issue forms before choosing implementation tools.

It can support applications for web, desktop, mobile, and embedded platforms; APIs, libraries, SDKs, CLI tools, AI and data projects, scientific computing, infrastructure, monorepos, hardware/PCB design, Blender/3D assets, documentation, and prototypes. No language, framework, runtime, package manager, or hosting provider is required.

## Create a project

On GitHub, select **Use this template → Create a new repository**, then choose a name and visibility. Clone the generated repository using its clone URL. If the button is absent, the owner must enable **Template repository** in repository settings.

Follow [Getting started](docs/GETTING_STARTED.md):

- [ ] Replace this README with the project's purpose, setup, usage, and support information.
- [ ] Review [LICENSE](LICENSE); it grants no license. Decide licensing before redistribution.
- [ ] Configure private security reporting and update [SECURITY.md](SECURITY.md).
- [ ] Select tools based on project needs; add source and dependency manifests only when needed.
- [ ] Track appropriate dependency lockfiles; extend Git and editor rules with precise project-specific patterns.
- [ ] Document local setup, configuration placeholders, and actual test commands.
- [ ] Read [Actions setup](docs/AUTOMATION.md) before enabling the optional manual check.
- [ ] Adapt issue forms, contribution guidance, agent instructions, and architecture notes.
- [ ] Remove template setup instructions and reset the changelog for your project.

## Defaults

The repository includes Git/editor settings, bug and feature forms, a pull request template, and concise documentation. Blank issues remain available for questions and other requests. No application scaffolding, dependencies, or scheduled dependency updates are included. A guarded, manual Actions workflow is available; automation is off by default.

The two-space editor default is adjustable; Makefiles use tabs. Git normalizes text to LF, with CRLF for Windows command scripts. Ignore rules stay narrow to avoid hiding source or assets; they are not a secret scanner.

## Documentation

- [Documentation index](docs/README.md)
- [Contribution guide](CONTRIBUTING.md)
- [Security policy](SECURITY.md)
- [Agent guidance](AGENTS.md)
- [Changelog](CHANGELOG.md)

## License

[LICENSE](LICENSE) is an explicit placeholder, not an open-source license or permission grant. GitHub's template mechanism does not change licensing rights. The owner must decide what reuse permissions to grant; generated projects must also resolve rights to copied material before distribution.
