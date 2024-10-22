# OCA Repository Guideline

Every OCA subproject may have one or more GitHub repositories. Each repository
(repo) could fall under one or more of the three categories: code, document,
and data.

OCA TSC establishes this guideline to help project growth and facilitate
collaborations with high-quality GitHub repositories.

## Life Cycle of an OCA Repository

1. Request: when a new repo is needed, the project maintainer
emails/slacks OCA TSC to create a new repo.

    - The repo can be instantiated from OCA template provided in this repo:

        - `README.md`
        - `LICENSE.md`
        - `CONTRIBUTING.md`
        - `CHANGELOG.md`
        - `AUTHORS.md`
        
        The Markdown files can be replaced with reStructuredText if needed.

    - The maintainer(s) prepare information in the *minimal requirements*
      section before submitting the repo creation request.

2. Creation: OCA GitHub admin creates the repo based on the request information
and adds the maintainer's team to the repo.

3. Maturing: The maintainer(s) of the new repo have 6 months to upgrade the
repo (minimal requirements) to meet the standard requirements. Optionally, the
repo can meet the bonus requirements to achieve an outstanding status.

4. Retirement: If a repo is no longer in use, any TSC member (usually the
maintainer of the project) can request a TSC voting to archive it. The voting
communicates with every TSC member to check dependent projects and repos.

## Repository Minimal Requirements

Use the OCA repo template to initialize a repo with key markdown files provided
and repo-specific information to be added.

Required information/files for the first 6 months of a new repo:

- GitHub Repo Metadata
    - Repo description (about)
    - Repo keywords
- `README.md`
    - Repo/project title
    - Short description
- `LICENSE.md`
    - Copy of one of the OCA-approved licenses
- `CONTRIBUTING.md`
- Simple documentation
    - In the form of a Markdown file, or more comprehensive readthedocs
    - Can be part of `README.md`
    - [if code repo] How to install?
    - [if code repo] How to compile/build locally?
    - [if code repo] How to deploy?

## Repository Standard Requirements

### Information and Documentation

- GitHub Repo Metadata
    - Repo description (about)
    - Repo keywords
- `README.md`
    - Repo/project title
    - Clear description
    - [if code repo] reference to installation doc
    - [if code repo] reference to buildling doc
    - [if code repo] reference to deployment doc
    - Related projects/repos
    - Reference to LICENSE
    - Reference to CONTRIBUTING
    - How to cite the project/repo
    - Where to ask questions and give feedback
        - Maillist
        - Slack
- `LICENSE.md`
    - Copy of one of the OCA-approved licenses
- `AUTHORS.md`
    - List of maintainers
    - List of contributors
- `CONTRIBUTING.md`
- Documentation
    - [if code repo] How to install?
    - [if code repo] How to compile/build locally?
    - [if code repo] How to deploy?
    - [if code repo] How to configure?
    - [if code repo] How to use the API?
    - [if code repo] How to enable debug mode if implemented?
    - [if data repo] How to use the data?
    - Reference to talks/presentations
- Governance [if code repo]
    - In `README.md`, a standalone Markdown, or in the documentation
    - Pull request management
        - Typical PR flow
        - How a PR is approved
        - Number of reviewers required
        - Checklist to get approved
    - Release
        - Release procedure
        - [optional] release frequency
    - Versioning
        - Versioning guideline
    - Vulnerability disclosure procedure
- GitHub issue templates

### Procedures and Actions

#### Branch Protection

Setup GitHub branch protection.

#### Continuous Integration

[GitHub Actions](https://docs.github.com/en/actions) for:

- Linting, example library: [black](https://github.com/psf/black)
- Unit tests
- Integration tests
- Code coverage

#### Continuous Delivery

One or more delivery channels to setup via [GitHub Actions](https://docs.github.com/en/actions):

- Docker Hub
- Package repository
    - PyPI
    - npm registry
- Linux distribution repository
    - Debian/Ubuntu
    - Fedora/OpenSUSE
    - Archlinux

## Repository Bonus Requirements

- Standalone documentation site
    - `readthedocs` or equivlant document hosting
- Advanced governance documentation
    - Maintainers
        - How are they selected by the community?
        - How long are their terms?
- Code quality
    - Static analysis
    - Dynamic analysis
    - Transparent crypto
        - Compliance levels, e.g., FIPS
- Transparent software supply chain
    - Dependency tracking
        - GitHub `dependabot` integration
    - SBOM
    - Vulnerability-Exploitability eXchange (VEX)
        - Multi-depth deps vulnerability analysis
        - Disclosure procedure
        - Vulnerability contact
        - Patching/mitigation procedure
- [OpenSSF scorecard](https://securityscorecards.dev/)
