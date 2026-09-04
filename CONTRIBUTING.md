# Contributing to YatraAI

Thank you for your interest in contributing to YatraAI! This document provides guidelines and instructions for contributing.

## Getting Started

1. **Fork** the repository
2. **Clone** your fork locally
3. **Create a branch** for your feature
4. **Make changes** and test thoroughly
5. **Submit a Pull Request**

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/yatra-ai.git
cd yatra-ai

# Install dependencies
npm install

# Start development server
npm run dev

# Run linting
npm run lint

# Build for testing
npm run build
```

## Code Quality Standards

- **Linting**: Run `npm run lint` before committing
- **React Hooks**: Follow rules of hooks
- **Component Exports**: Only export components (not constants)
- **File Structure**: Follow existing folder structure

## Commit Message Format

```
type: subject

body (optional)

footer (optional)
```

**Types:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation
- `style:` Formatting
- `refactor:` Code reorganization
- `test:` Tests
- `chore:` Build/dependency updates

**Example:**
```
feat: Add transport comparison component

This component displays various transportation options
with cost and duration comparisons.

Closes #123
```

## Pull Request Process

1. **Update** main branch: `git pull origin main`
2. **Create feature branch**: `git checkout -b feature/your-feature-name`
3. **Make changes** and commit
4. **Push branch**: `git push origin feature/your-feature-name`
5. **Create Pull Request** with:
   - Clear title
   - Description of changes
   - Reference to related issues
   - Screenshots (if UI changes)

## Testing

Before submitting:

```bash
# Run linting
npm run lint

# Build production
npm run build

# Preview build
npm run preview
```

## Code Style

- **JavaScript**: ES6+ features
- **React**: Functional components with hooks
- **CSS**: Mobile-first responsive design
- **Naming**: Clear, descriptive names

## Issues

Found a bug? Please:

1. Check existing issues
2. Create detailed issue with:
   - Steps to reproduce
   - Expected behavior
   - Actual behavior
   - Screenshots/videos
   - Environment info

## Questions?

- Create a **Discussion**: GitHub Discussions
- Check **README**: Common questions answered
- Open an **Issue**: For bug reports

## License

By contributing, you agree your code is licensed under MIT License.

---

Thank you for making YatraAI better! 🚀
