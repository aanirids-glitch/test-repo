# Contributing Guidelines

Thank you for your interest in contributing to `test-repo`! This document provides guidelines and instructions for contributing.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [Available Scripts](#available-scripts)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.

## Getting Started

1. **Fork the Repository**
   - Click the 'Fork' button on GitHub to create your own copy.

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/test-repo.git
   cd test-repo
   ```

3. **Install Dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

## Development Setup

1. **Start the Development Server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```
   This will start the Vite dev server, usually at `http://localhost:5173`.

2. **Run Tests**
   ```bash
   npm test
   # or
   yarn test
   ```

3. **Run Linting**
   ```bash
   npm run lint
   # or
   yarn lint
   ```

## Available Scripts

| Script | Description |
|--------|-------------|
| `dev` | Starts the development server |
| `build` | Creates a production build |
| `preview` | Locally preview the production build |
| `lint` | Runs ESLint on the codebase |
| `test` | Runs the test suite |
| `format` | Formats code with Prettier (if configured) |

## Coding Standards

### JavaScript/React

- Use **ESLint** to enforce code style. Run `npm run lint` before committing.
- Use **functional components** and **hooks** over class components.
- Use **destructuring** for cleaner code.
- Use **template literals** for string interpolation.
- Write **meaningful variable and function names**.
- Add **JSDoc comments** to functions and components.

### File Naming

- Use **PascalCase** for component files: `MyComponent.jsx`
- Use **camelCase** for utility files: `formatDate.js`
- Use **SCREAMING_SNAKE_CASE** for constants: `API_CONSTANTS.js`

### Component Structure

```jsx
import React from 'react';

/**
 * Description of the component
 * @param {Object} props - Component props
 * @returns {JSX.Element}
 */
const MyComponent = ({ prop1, prop2 }) => {
  // Component logic

  return (
    <div>
      {/* JSX */}
    </div>
  );
};

export default MyComponent;
```

## Commit Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, etc.)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `perf`: A code change that improves performance
- `test`: Adding missing tests or correcting existing tests
- `chore`: Changes to the build process or auxiliary tools and libraries

### Example

```
feat(auth): add login page component

- Create LoginForm component with email and password fields
- Add form validation using Formik and Yup
- Implement password visibility toggle

Closes #123
```

## Pull Request Process

1. **Create a Feature Branch**
   ```bash
   git checkout -b feature/my-new-feature
   ```

2. **Make Your Changes**
   - Write clean, tested, and documented code.
   - Ensure all tests pass.
   - Ensure linting passes.

3. **Push to Your Fork**
   ```bash
   git push origin feature/my-new-feature
   ```

4. **Open a Pull Request**
   - Go to the original repository on GitHub.
   - Open a pull request against the `main` branch.
   - Fill out the PR template with a clear description of your changes.

5. **Code Review**
   - Your PR will be reviewed by maintainers.
   - Address any feedback or requested changes.

6. **Merge**
   - Once approved, your changes will be merged.

## Reporting Issues

If you find a bug or have a feature request, please [open an issue](https://github.com/aanirids-glitch/test-repo/issues) with the following information:

- **Clear description** of the issue or feature.
- **Steps to reproduce** (for bugs).
- **Expected behavior**.
- **Actual behavior**.
- **Environment** (OS, browser, Node.js version, etc.).
- **Screenshots** (if applicable).