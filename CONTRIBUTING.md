# Contributing to My Projects

Thank you for your interest in contributing! I welcome contributions from the community. This document provides guidelines and instructions for contributing.

## 🤝 Code of Conduct

Please be respectful and constructive in all interactions. We are committed to providing a welcoming and inclusive environment for all contributors.

### Expected Behavior
- Be respectful and inclusive
- Provide constructive feedback
- Focus on the code, not the person
- Help others learn and grow

### Unacceptable Behavior
- Harassment or discrimination
- Offensive language or behavior
- Disruptive comments
- Violations of privacy

---

## 🚀 Getting Started

### Prerequisites
- Git installed and configured
- Node.js/npm or PHP/Composer (depending on project)
- Basic understanding of the project

### Setup Development Environment

1. **Fork the repository**
   ```bash
   # Visit the repository on GitHub and click "Fork"
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/project-name.git
   cd project-name
   ```

3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/programinglive/project-name.git
   ```

4. **Install dependencies**
   ```bash
   # For Node.js projects
   npm install
   
   # For PHP projects
   composer install
   ```

5. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

---

## 📝 Commit Guidelines

### Commit Message Format

Follow the conventional commits specification:

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
- **perf**: Code change that improves performance
- **test**: Adding or updating tests
- **chore**: Changes to build process, dependencies, etc.

### Examples

```
feat(auth): add JWT authentication

Implement JWT-based authentication with refresh tokens.
Supports both access and refresh token flows.

Closes #123
```

```
fix(api): handle null response in user endpoint

Add null check before accessing user properties
to prevent runtime errors.

Fixes #456
```

---

## 🔄 Pull Request Process

### Before Submitting

1. **Update your branch**
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Run tests**
   ```bash
   npm test
   # or
   composer test
   ```

3. **Check code quality**
   ```bash
   npm run lint
   # or
   composer lint
   ```

4. **Build the project**
   ```bash
   npm run build
   # or
   composer build
   ```

### Creating a Pull Request

1. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Open a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill in the PR template

3. **PR Description Template**
   ```markdown
   ## Description
   Brief description of changes
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Breaking change
   - [ ] Documentation update
   
   ## Related Issues
   Closes #123
   
   ## Testing
   Describe how to test these changes
   
   ## Checklist
   - [ ] Tests pass
   - [ ] Code follows style guidelines
   - [ ] Documentation updated
   - [ ] No breaking changes
   ```

---

## 🧪 Testing

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm test -- --watch

# Run tests with coverage
npm test -- --coverage
```

### Writing Tests

- Write tests for new features
- Update tests when modifying existing code
- Aim for >80% code coverage
- Use descriptive test names

### Test Structure

```javascript
describe('Feature Name', () => {
  beforeEach(() => {
    // Setup
  });

  it('should do something specific', () => {
    // Arrange
    const input = 'test';
    
    // Act
    const result = functionUnderTest(input);
    
    // Assert
    expect(result).toBe('expected');
  });
});
```

---

## 📋 Code Style

### JavaScript/TypeScript

- Use ESLint configuration from the project
- Use Prettier for formatting
- Follow the existing code style
- Use meaningful variable names
- Add comments for complex logic

```javascript
// Good
function calculateUserScore(user) {
  const baseScore = user.points * 1.5;
  const bonusScore = user.achievements.length * 10;
  return baseScore + bonusScore;
}

// Bad
function calc(u) {
  return u.p * 1.5 + u.a.length * 10;
}
```

### PHP

- Follow PSR-12 coding standards
- Use meaningful class and method names
- Add PHPDoc comments
- Use type hints

```php
/**
 * Calculate user score
 *
 * @param User $user
 * @return int
 */
public function calculateUserScore(User $user): int
{
    $baseScore = $user->points * 1.5;
    $bonusScore = count($user->achievements) * 10;
    
    return (int)($baseScore + $bonusScore);
}
```

---

## 📚 Documentation

### Update Documentation
- Update README.md if adding features
- Add/update API documentation
- Include code examples
- Document breaking changes

### Documentation Format

```markdown
## Feature Name

Brief description of the feature.

### Usage

```javascript
// Code example
```

### Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| param1 | string | Description |

### Returns

Description of return value
```

---

## 🐛 Reporting Bugs

### Bug Report Template

```markdown
## Description
Clear description of the bug

## Steps to Reproduce
1. Step 1
2. Step 2
3. Step 3

## Expected Behavior
What should happen

## Actual Behavior
What actually happens

## Environment
- OS: [e.g., Windows 10]
- Node version: [e.g., 18.0.0]
- Package version: [e.g., 1.0.0]

## Screenshots
If applicable, add screenshots
```

---

## 💡 Feature Requests

### Feature Request Template

```markdown
## Description
Clear description of the feature

## Use Case
Why this feature is needed

## Proposed Solution
How the feature should work

## Alternatives
Alternative approaches considered
```

---

## 🔍 Code Review

### What to Expect

- Constructive feedback on your code
- Requests for tests or documentation
- Suggestions for improvements
- Approval once all feedback is addressed

### Responding to Feedback

- Address all comments
- Ask for clarification if needed
- Push updates to the same branch
- Mark conversations as resolved

---

## 📦 Release Process

### Version Numbering

We follow Semantic Versioning (MAJOR.MINOR.PATCH):
- MAJOR: Breaking changes
- MINOR: New features (backward compatible)
- PATCH: Bug fixes

### Release Checklist

- [ ] All tests pass
- [ ] Documentation updated
- [ ] CHANGELOG.md updated
- [ ] Version bumped
- [ ] Release notes written

---

## 🎯 Development Workflow

### Recommended Workflow

1. Create feature branch from `main`
2. Make changes with meaningful commits
3. Write/update tests
4. Update documentation
5. Submit pull request
6. Address review feedback
7. Merge to `main`
8. Delete feature branch

---

## 📞 Getting Help

- **Questions**: Open a discussion or issue
- **Documentation**: Check project README and docs
- **Community**: Join our community discussions
- **Email**: mahatmamahardhika200588@gmail.com

---

## ✨ Recognition

Contributors will be recognized in:
- CONTRIBUTORS.md file
- Release notes
- Project documentation

Thank you for contributing! 🙏

---

*Last updated: December 2025*
