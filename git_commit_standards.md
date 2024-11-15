# Git Commit Standards

## 1. Commit Message Structure

A commit message typically consists of three parts:

- **Header**: A short summary of the changes.
- **Body**: A detailed explanation of the commit.
- **Footer**: Additional information like issue references.

***

## 2. Header Guidelines

- **Length**: Maximum 50 characters.
- **Imperative Mood**: Use present tense, e.g., "Fix bug" (not "Fixed bug").
- **Capitalization**: Capitalize the first word.
- **No Period**: Avoid ending with a period.
- **Clear and Specific**: Clearly state the purpose.

***

## 3. Body Guidelines

- **Length**: Wrap text at 72 characters for readability.
- **Explanation**: Describe why the change was made and provide context.
- **Focus**: Emphasize why the change is necessary over how it was implemented.
- **Bullet Points**: Use bullet points for multiple points.

***

## 4. Footer Guidelines

- **Issue References**: Link to relevant issues (e.g., `Fixes #123`).
- **Breaking Changes**: Clearly indicate if there are breaking changes.

  ````
  BREAKING CHANGE: The API now requires an authentication token.
  ````


***

## 5. Types of Commit Messages

Use prefixes to classify commits:

- **feat**: Introduces a new feature.
- **fix**: Fixes a bug.
- **docs**: Changes to documentation.
- **style**: Code style changes (formatting, etc.).
- **refactor**: Refactoring code without changing functionality.
- **test**: Adding or modifying tests.
- **chore**: Routine tasks or maintenance (e.g., dependency updates).
- **ci**: Changes related to CI/CD.

Example:

````
feat: Add user authentication
fix: Resolve login bug with incorrect password validation
docs: Update README with setup instructions
````

***

## 6. Conventional Commits

Structure:

````
<type>(<scope>): <message>
````

Examples:

````
feat(auth): add JWT authentication
fix(api): correct data parsing error
````

***

## 7. Commit Granularity

- **Small Commits**: Make each commit represent a single logical change.
- **Atomic Commits**: Ensure each commit can stand alone and be reverted individually.

***

## Summary Example

````
feat(user-auth): add login and registration API

- Implemented JWT token-based authentication
- Updated user model to handle passwords securely
- Added tests for login and registration endpoints

Fixes #123
````