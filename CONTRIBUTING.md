# Contributing to Fynbos Ltd Projects

Thank you for your interest in contributing to our projects! We welcome contributions from the community and are grateful for any help you can provide.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Process](#development-process)
- [Style Guidelines](#style-guidelines)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.

## Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git
   cd REPOSITORY-NAME
   ```
3. **Add the upstream repository** as a remote:
   ```bash
   git remote add upstream https://github.com/fynbosltd/REPOSITORY-NAME.git
   ```
4. **Create a new branch** for your contribution:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include as many details as possible:

- Use a clear and descriptive title
- Describe the exact steps to reproduce the problem
- Provide specific examples to demonstrate the steps
- Describe the behavior you observed and what you expected
- Include screenshots if applicable
- Note your environment (OS, browser, version, etc.)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- Use a clear and descriptive title
- Provide a detailed description of the proposed enhancement
- Explain why this enhancement would be useful
- List any alternative solutions you've considered

### Code Contributions

1. Ensure your code adheres to the project's style guidelines
2. Write clear, commented code
3. Add or update tests as necessary
4. Update documentation to reflect your changes
5. Ensure all tests pass before submitting

## Development Process

### Setting Up Your Development Environment

Refer to the project's README.md for specific setup instructions. Generally:

1. Install dependencies
2. Set up any required environment variables
3. Run tests to ensure everything is working
4. Start the development server

### Making Changes

1. **Keep changes focused**: Each PR should address a single concern
2. **Write tests**: Ensure your changes are covered by tests
3. **Update documentation**: Keep docs in sync with code changes
4. **Follow conventions**: Match the existing code style and patterns

### Testing

- Write unit tests for new functionality
- Ensure all existing tests pass
- Add integration tests where appropriate
- Test edge cases and error conditions

Run tests with:
```bash
# Add project-specific test commands here
npm test
# or
pytest
# or
go test ./...
```

## Style Guidelines

### General Principles

- Write clear, readable code
- Use meaningful variable and function names
- Keep functions small and focused
- Comment complex logic
- Follow the DRY (Don't Repeat Yourself) principle

### Language-Specific Guidelines

#### Python
- Follow PEP 8
- Use type hints where appropriate
- Maximum line length: 88 characters (Black formatter)

#### JavaScript/TypeScript
- Use ES6+ features
- Follow the Airbnb style guide
- Use TypeScript for type safety

#### Go
- Follow the official Go style guide
- Run `gofmt` before committing
- Use meaningful package names

## Commit Messages

Write clear and meaningful commit messages following these guidelines:

### Format
```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that don't affect code meaning (formatting, etc.)
- **refactor**: Code change that neither fixes a bug nor adds a feature
- **perf**: Performance improvement
- **test**: Adding or updating tests
- **chore**: Changes to build process or auxiliary tools

### Examples
```
feat(auth): add OAuth2 authentication

Implement OAuth2 authentication flow with support for Google and GitHub providers.

Closes #123
```

```
fix(api): handle null response in user endpoint

Add null check to prevent crashes when user data is not available.

Fixes #456
```

## Pull Request Process

1. **Update your branch** with the latest upstream changes:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Push your changes** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

3. **Create a Pull Request** on GitHub:
   - Use a clear and descriptive title
   - Fill out the PR template completely
   - Link related issues
   - Describe your changes in detail
   - Add screenshots for UI changes

4. **Respond to feedback**:
   - Address reviewer comments promptly
   - Make requested changes
   - Keep the conversation professional and constructive

5. **Merge requirements**:
   - All tests must pass
   - Code review approval from maintainers
   - No merge conflicts with main branch
   - Documentation updated if necessary

## Community

### Getting Help

- Check the project documentation
- Search existing issues and discussions
- Ask questions in GitHub Discussions
- Join our community chat (if applicable)

### Recognition

Contributors are recognized in:
- The project's README
- Release notes
- GitHub's contributor graph

### Code Review

All submissions require review. We use GitHub pull requests for this purpose. Reviewers will look for:

- Code quality and style
- Test coverage
- Documentation completeness
- Performance implications
- Security considerations

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (see LICENSE file).

## Questions?

Don't hesitate to ask questions. We're here to help!

Thank you for contributing to Fynbos Ltd projects! 🌿
