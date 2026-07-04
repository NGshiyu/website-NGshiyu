```markdown
# website-NGshiyu Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `website-NGshiyu` repository, a React application written in TypeScript. It covers file naming, import/export styles, commit message conventions, and testing patterns. Use this as a reference for contributing code that matches the project's established style.

## Coding Conventions

### File Naming
- Use **camelCase** for all file names.
  - Example: `userProfile.tsx`, `mainHeader.ts`

### Imports
- Use **relative imports** for all modules.
  - Example:
    ```typescript
    import userService from './userService';
    import Header from '../components/header';
    ```

### Exports
- Use **default exports** for modules.
  - Example:
    ```typescript
    // userService.ts
    const userService = { /* ... */ };
    export default userService;
    ```

### Commit Messages
- Follow **Conventional Commits** with the `feat` prefix for features.
- Keep commit messages concise (average ~33 characters).
  - Example: `feat: add user authentication`

## Workflows

### Feature Development
**Trigger:** When adding a new feature  
**Command:** `/feature-development`

1. Create a new branch for your feature.
2. Implement the feature using camelCase file naming.
3. Use relative imports and default exports as per conventions.
4. Write or update tests in files matching `*.test.*`.
5. Commit your changes using the `feat` prefix and a concise message.
6. Open a pull request for review.

### Testing
**Trigger:** When verifying code correctness  
**Command:** `/run-tests`

1. Identify or create test files using the `*.test.*` pattern.
2. Run the test suite using the project's test runner (framework unknown; check project scripts).
3. Ensure all tests pass before merging changes.

## Testing Patterns

- Test files follow the `*.test.*` naming convention (e.g., `userProfile.test.tsx`).
- The specific testing framework is not identified; refer to project documentation or scripts for details.
- Place test files alongside the modules they test or in a dedicated `tests` directory, as per project structure.

## Commands
| Command              | Purpose                                   |
|----------------------|-------------------------------------------|
| /feature-development | Start the feature development workflow    |
| /run-tests           | Run the project's test suite              |
```
