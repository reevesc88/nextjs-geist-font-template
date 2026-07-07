```markdown
# nextjs-geist-font-template Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill covers the core development patterns and conventions used in the `nextjs-geist-font-template` repository. The project is written in TypeScript and provides a template for integrating Geist fonts with a Next.js application. While no specific framework is detected, the codebase follows clear conventions for commits, file organization, and code style. This guide will help you contribute effectively and maintain consistency.

## Coding Conventions

### File Naming
- Use **kebab-case** for all file names.
  - Example:  
    ```
    my-component.tsx
    utils/helpers.ts
    ```

### Import Style
- Use **relative imports** for modules within the project.
  - Example:
    ```typescript
    import { myFunction } from './utils/helpers';
    ```

### Export Style
- Use **named exports** instead of default exports.
  - Example:
    ```typescript
    // In utils/helpers.ts
    export function myFunction() { ... }
    ```

### Commit Messages
- Follow the **conventional commit** style.
- Use the `feat` prefix for new features.
- Keep commit messages concise (average 52 characters).
  - Example:
    ```
    feat: add Geist font integration to layout
    ```

## Workflows

### Add a New Feature
**Trigger:** When implementing a new feature or enhancement  
**Command:** `/add-feature`

1. Create a new branch for your feature.
2. Write code using kebab-case file naming and relative imports.
3. Use named exports for all modules.
4. Write or update tests as needed.
5. Commit changes using a conventional commit message with the `feat` prefix.
6. Open a pull request for review.

### Run Tests
**Trigger:** When you want to verify code correctness  
**Command:** `/run-tests`

1. Identify test files (pattern: `*.test.*`).
2. Run the test suite using your preferred test runner (framework is unspecified).
3. Review test results and fix any failing tests.

## Testing Patterns

- Test files follow the pattern `*.test.*` (e.g., `component.test.ts`).
- The specific testing framework is not detected, but standard TypeScript testing practices apply.
- Place tests alongside the code they test or in a dedicated `__tests__` directory.
- Example test file:
  ```typescript
  // button.test.ts
  import { render } from '@testing-library/react';
  import { Button } from './button';

  test('renders button', () => {
    const { getByText } = render(<Button>Click me</Button>);
    expect(getByText('Click me')).toBeInTheDocument();
  });
  ```

## Commands
| Command        | Purpose                                   |
|----------------|-------------------------------------------|
| /add-feature   | Start the workflow for adding a new feature|
| /run-tests     | Run the test suite                        |
```
