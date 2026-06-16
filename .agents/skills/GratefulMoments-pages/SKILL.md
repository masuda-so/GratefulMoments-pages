```markdown
# GratefulMoments-pages Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the GratefulMoments-pages TypeScript codebase. You'll learn about file naming, import/export styles, commit message conventions, and how to write and run tests. The repository does not use a detected framework, so patterns are lightweight and framework-agnostic.

## Coding Conventions

### File Naming
- **Pattern:** PascalCase for all files.
- **Example:**  
  ```
  GratefulMomentPage.ts
  UserProfileComponent.ts
  ```

### Import Style
- **Pattern:** Relative imports are used throughout.
- **Example:**
  ```typescript
  import { UserProfile } from './UserProfileComponent';
  ```

### Export Style
- **Pattern:** Named exports.
- **Example:**
  ```typescript
  // In GratefulMomentPage.ts
  export const GratefulMomentPage = () => { /* ... */ };
  ```

### Commit Messages
- **Pattern:** Conventional commits, primarily with the `chore` prefix.
- **Example:**
  ```
  chore: update dependencies
  chore: fix typo in GratefulMomentPage
  ```

## Workflows

### Code Commit Workflow
**Trigger:** When making any change to the codebase  
**Command:** `/commit`

1. Make your code changes following the coding conventions.
2. Stage your changes:
   ```
   git add .
   ```
3. Write a commit message using the conventional commit format, typically starting with `chore:`.
   ```
   git commit -m "chore: describe your change"
   ```
4. Push your changes:
   ```
   git push
   ```

### Testing Workflow
**Trigger:** When you want to run or add tests  
**Command:** `/test`

1. Write your test files using the `*.test.*` naming pattern.
   - Example: `GratefulMomentPage.test.ts`
2. Use your preferred test runner (not specified in the repo; common options are Jest or Mocha).
   - Example with Jest:
     ```
     npx jest
     ```
3. Review test results and fix any failures.

## Testing Patterns

- **Test File Naming:**  
  All test files follow the `*.test.*` pattern.
  - Example: `UserProfileComponent.test.ts`
- **Test Framework:**  
  Not explicitly specified. Use your preferred TypeScript-compatible test runner.
- **Test Example:**
  ```typescript
  // UserProfileComponent.test.ts
  import { UserProfile } from './UserProfileComponent';

  test('should render user profile', () => {
    // ...test implementation
  });
  ```

## Commands
| Command   | Purpose                                   |
|-----------|-------------------------------------------|
| /commit   | Commit code changes using conventions     |
| /test     | Run or add tests to the codebase          |
```
