# Contributing to Docker Templates

Thank you for considering contributing to the Docker Templates repository! This document provides guidelines and instructions for contributing.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Contribution Guidelines](#contribution-guidelines)
- [Pull Request Process](#pull-request-process)
- [Style Guide](#style-guide)

## Code of Conduct

This project adheres to a Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.

## How Can I Contribute?

### Reporting Bugs

- Use the GitHub issue tracker to report bugs
- Check if the bug has already been reported
- Include detailed steps to reproduce the issue
- Include your environment details (OS, Docker version, etc.)

### Suggesting Enhancements

- Use the GitHub issue tracker for feature requests
- Clearly describe the feature and its benefits
- Provide examples of how the feature would be used

### Adding New Templates

- Follow the existing template structure
- Include a comprehensive README.md
- Test the template thoroughly before submitting
- Document all environment variables and configuration options

### Improving Documentation

- Fix typos or clarify existing documentation
- Add examples and use cases
- Improve troubleshooting guides

## Getting Started

1. **Fork the Repository**
   ```bash
   # Fork via GitHub UI, then clone your fork
   git clone https://github.com/YOUR-USERNAME/docker-templates.git
   cd docker-templates
   ```

2. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

3. **Make Your Changes**
   - Follow the style guide
   - Test your changes
   - Update documentation as needed

4. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "Brief description of your changes"
   ```

5. **Push to Your Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Open a Pull Request**
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill out the PR template

## Contribution Guidelines

### Docker Compose Templates

- **File Naming**: Use `docker-compose.yml` (not .yaml, and no spaces in filenames)
- **Version**: Use Docker Compose file format version 3.8 or higher
- **Comments**: Add clear comments explaining each service and configuration
- **Security**: Never include real credentials; use environment variables
- **Images**: Specify exact versions instead of `latest` tag when possible
- **Volumes**: Use named volumes for data persistence
- **Networks**: Define custom networks when services need to communicate
- **Healthchecks**: Include healthchecks for services that support them

### Documentation

Each template directory must include:
- `docker-compose.yml` - The Docker Compose configuration
- `README.md` - Comprehensive documentation including:
  - Overview of the service/stack
  - Prerequisites
  - Quick start guide
  - Configuration options
  - Environment variables
  - Usage examples
  - Troubleshooting tips
  - Links to official documentation

### Environment Files

- Provide `.env.example` files with dummy values
- Document all environment variables
- Never commit actual `.env` files with real credentials

## Pull Request Process

1. **Update Documentation**
   - Update README.md if you've added/changed features
   - Add your template to the index if applicable

2. **Test Your Changes**
   - Ensure `docker-compose up` works without errors
   - Test with `docker-compose down` for proper cleanup
   - Verify volumes and data persistence

3. **Follow the Style Guide**
   - Consistent formatting
   - Clear, descriptive comments
   - Proper indentation (2 spaces for YAML)

4. **PR Description**
   - Clearly describe what your PR does
   - Reference any related issues
   - Include screenshots if applicable
   - List any breaking changes

5. **Review Process**
   - Maintainers will review your PR
   - Address any requested changes
   - Once approved, your PR will be merged

## Style Guide

### YAML Files

```yaml
version: '3.8'

services:
  service-name:
    # Use descriptive comments
    image: image-name:specific-version
    restart: unless-stopped
    ports:
      - "host-port:container-port"
    environment:
      - ENV_VAR=${ENV_VAR}
    volumes:
      - volume-name:/path/in/container
    networks:
      - network-name

volumes:
  # Volume for service data
  volume-name:

networks:
  # Custom network for service communication
  network-name:
```

### README Structure

```markdown
# Service Name

Brief description of what this service does.

## Prerequisites

- Docker installed
- Docker Compose installed
- Any other requirements

## Quick Start

1. Step one
2. Step two
3. Step three

## Configuration

### Environment Variables

- `VAR_NAME` - Description (default: value)

### Ports

- `8080` - Description

## Usage

Detailed usage instructions

## Troubleshooting

Common issues and solutions

## Resources

- [Official Documentation](url)
- [GitHub Repository](url)
```

### Commit Messages

- Use clear, descriptive commit messages
- Start with a verb in present tense (Add, Fix, Update, Remove)
- Keep the first line under 50 characters
- Add detailed explanation in the body if needed

Examples:
```
Add PostgreSQL template with pgAdmin
Fix port mapping in MongoDB template
Update Nginx configuration for SSL
Remove deprecated Docker Compose syntax
```

## Questions?

If you have questions or need help, please:
- Check existing issues and discussions
- Open a new issue with the "question" label
- Reach out to the maintainers

Thank you for contributing! 🚀
