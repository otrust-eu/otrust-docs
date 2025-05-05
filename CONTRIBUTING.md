# Contributing to OTRUST

Thank you for your interest in contributing to OTRUST! This document provides guidelines and instructions for contributing to the OTRUST distributed truth protocol ecosystem.

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone. We expect all contributors to:

- Be respectful and considerate of differing viewpoints
- Accept constructive criticism gracefully
- Focus on what is best for the community
- Show empathy towards other community members

## How to Contribute

OTRUST consists of three main repositories:

1. [otrust-server](https://github.com/otrust-eu/otrust-server) - Server implementation
2. [otrust-cli](https://github.com/otrust-eu/otrust-cli) - Command-line interface
3. [otrust-docs](https://github.com/otrust-eu/otrust-docs) - Documentation

You can contribute to any of these repositories according to your skills and interests.

### Reporting Issues

If you find a bug or have a suggestion for improvement:

1. Check the existing issues to avoid duplicates
2. Open a new issue using the appropriate template
3. Provide detailed information about the problem or suggestion:
   - For bugs: Steps to reproduce, expected behavior, actual behavior
   - For features: Clear description, use cases, potential implementation approach

### Making Code Contributions

1. **Fork the repository** you want to contribute to
2. **Create a new branch** from the main branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**, following the coding standards
4. **Add tests** for new functionality
5. **Ensure all tests pass**
   ```bash
   npm test
   ```
6. **Commit your changes** with clear, descriptive messages
   ```bash
   git commit -m "Add feature: brief description of what you did"
   ```
7. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```
8. **Submit a pull request** to the original repository

### Documentation Contributions

For documentation improvements:

1. Fork the [otrust-docs](https://github.com/otrust-eu/otrust-docs) repository
2. Make your changes, ensuring they are clear and well-formatted
3. If documenting an API or feature, ensure the documentation matches the implementation
4. Submit a pull request with your changes

## Development Setup

### Server Development

```bash
# Clone the repository
git clone https://github.com/otrust-eu/otrust-server.git
cd otrust-server

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env
# Edit .env as needed

# Start development server
npm run dev
```

### CLI Development

```bash
# Clone the repository
git clone https://github.com/otrust-eu/otrust-cli.git
cd otrust-cli

# Install dependencies
npm install

# Create symbolic link for local development
npm link

# Test the CLI
otrust-cli --help
```

## Coding Standards

### JavaScript Style Guide

- Follow modern JavaScript conventions (ES6+)
- Use async/await for asynchronous operations
- Use arrow functions where appropriate
- Follow the principle of least privilege and immutability

### Naming Conventions

- Use camelCase for variables and functions
- Use PascalCase for classes
- Use UPPER_CASE for constants
- Use descriptive names that reflect purpose

### Comments and Documentation

- Write clear JSDoc comments for all functions
- Explain complex logic with inline comments
- Document public APIs thoroughly

### Testing

- Write unit tests for all new functionality
- Ensure all existing tests pass before submitting a PR
- Test edge cases and error conditions

## Pull Request Process

1. Update the README.md or documentation with any necessary changes
2. Include tests for new functionality
3. Ensure the CI build passes
4. Get at least one code review from a maintainer
5. Maintainers will merge the PR when approved

## Release Process

OTRUST follows semantic versioning (MAJOR.MINOR.PATCH):

- MAJOR: Incompatible API changes
- MINOR: Backwards-compatible new features
- PATCH: Backwards-compatible bug fixes

## Getting Help

If you have questions about contributing:

- Open an issue in the appropriate repository
- Contact the maintainers

Thank you for contributing to OTRUST!
