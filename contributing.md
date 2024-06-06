# Contributing to Serverless Workflow

Welcome to our community! We're thrilled to have you here and appreciate your interest in contributing to the Serverless Workflow project. This document outlines the process for reporting issues, suggesting changes, and the conventions we follow to maintain our documentation's integrity and readability.

## Table of Contents

- [Reporting an Issue](#reporting-an-issue)
- [Suggesting a Change](#suggesting-a-change)
- [Versioning](#versioning)
- [Spec Formatting Conventions](#spec-formatting-conventions)
- [Contributing Guidelines](#contributing-guidelines)
- [Checks](#checks)

## Reporting an Issue

If you have a question or need clarification, we encourage you to start a [discussion](https://github.com/serverlessworkflow/specification/discussions) rather than opening an issue right away.

For reporting an issue or suggesting an idea for a change that you haven't fully fleshed out yet, please open an [issue](https://github.com/serverlessworkflow/specification/issues). It's a good idea to check existing [issues](https://github.com/serverlessworkflow/specification/issues) first to avoid duplication.

## Suggesting a Change

We understand that enhancements or bugs in a specification may require some back-and-forth discussion. Before submitting a pull request, please initiate a [discussion](https://github.com/serverlessworkflow/specification/discussions) or an [issue](https://github.com/serverlessworkflow/specification/issues) to engage with the community on your proposal.

Once there's a consensus, you can submit a [pull request](https://github.com/serverlessworkflow/specification/pulls) (PR) with the changes that have been discussed. For details on document formatting, refer to the [Spec Formatting Conventions](#spec-formatting-conventions) section.

## Versioning

Our versioning strategy is designed to reflect the nature of changes made through PRs. Please refer to the table below for how different types of changes affect version numbers:

| Label | Version Change | Description |
|:-- |:---:|:---|
| `change: documentation` | - | Documentation improvements or clarifications. |
| `change: fix` | `0.0.x` | Bug fixes in the DSL specification or its implementations. |
| `change: feature` | `0.x.0` | New features that enhance the DSL's capabilities. |
| `change: breaking` | `x.0.0` | Changes that break backward compatibility. |

Pre-release versions are indicated with suffixes such as `alphaX`, `betaX`, or `rcX`, where `X` is the pre-release version number.

## Spec Formatting Conventions

We strive for consistency and readability in our documentation by adhering to the following rules:

- Wrap lines at 80 columns where feasible.
- Use [RFC2119](https://tools.ietf.org/html/rfc2119) keywords for normative requirements.

## Contributing Guidelines

### Focus on the Topic

When creating an issue or discussion, stick to one specific topic to keep the conversation clear and efficient. Ensure your replies are relevant to the main subject, even when the discussion branches into related topics.

### Constructive Communication

Craft your contributions to discussions thoughtfully. Organize your thoughts coherently, and use quotes to reference specific points made by others. This helps reduce fragmented responses and maintains a clear dialogue.

### Thoughtful Participation

Be considerate of the frequency of your replies. Allow time for others to contribute and for you to reflect on your response. This pacing can lead to a richer variety of input and a more balanced discussion.

### Engaging the Community

For decisions that benefit from diverse opinions, seek feedback from the community through polls or open requests. The collective wisdom of the community can guide us to better decisions.

### Pull Request Etiquette

Only open a PR after reaching a consensus on the proposed changes. The PR review should focus on the correct implementation of the agreed-upon changes, not on further debate. Ensure discussions occur before the PR is created.

## Checks

### Markdown Style

Markdown files should be formatted according to our [markdownlint rules](https://github.com/DavidAnson/markdownlint#rules--aliases), with some customizations found in our [.markdownlint.yaml](.markdownlint.yaml) and [settings](.vscode/settings.json). We encourage line breaks at 80 characters for readability. If you're using Visual Studio Code, the `fixAll` command of the [vscode markdownlint extension](https://github.com/DavidAnson/vscode-markdownlint) can help with this.

To check for style violations, you can use the following commands:

```bash
# Ruby and gem are required for mdl
gem install mdl
mdl -c .mdlrc .
```

For fixing style violations, refer to the [markdownlint instructions](https://github.com/**********/markdownlint#optionsresultversion) with the Node version of markdownlint.

### Typos

Please ensure that typos are corrected before submitting your changes. You can check for typos using:

```bash
# Golang is needed for the misspell tool.
make install-misspell
make misspell
```

To fix typos quickly, use:

```bash
make misspell-correction
```

### Assigning and Owning Work

If you're interested in taking ownership of an issue, you can signal this by adding a comment or using “#dibs” in the issue thread. A maintainer will then assign the issue to you and label it accordingly.

## Final Thoughts

These guidelines are here to help us work together more effectively. They are not strict rules but rather recommendations to foster a constructive and collaborative environment. By considering our responses and engaging thoughtfully, we can have more meaningful discussions.

Your ideas, enthusiasm, and active participation are what make this community thrive. Let's keep our energy positive and our collaboration strong. Thank you for your time, dedication, and contributions. Your efforts are greatly valued and appreciated! ❤️

---

We hope this document helps you understand how to contribute effectively to the Serverless Workflow project. If you have any questions or need further clarification on any of these points, please reach out to the community through our discussions page. We're here to help and look forward to your contributions!
