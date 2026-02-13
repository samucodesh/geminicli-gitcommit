# Conventional Commit Standards

## Structure
```
<type>(<scope>): <concise subject>

<body explaining the "why" of the change>

<footer for BREAKING CHANGES or issue references>
```

## Mandatory Types
*   **feat**: A new feature.
*   **fix**: A bug fix.
*   **docs**: Documentation only changes.
*   **style**: Changes that do not affect the meaning of the code (white-space, formatting, etc.).
*   **refactor**: A code change that neither fixes a bug nor adds a feature.
*   **perf**: A code change that improves performance.
*   **test**: Adding missing tests or correcting existing tests.
*   **build**: Changes that affect the build system or external dependencies (e.g., npm, make).
*   **ci**: Changes to our CI configuration files and scripts (e.g., GitHub Actions).
*   **chore**: Other changes that don't modify source or test files (e.g., updating `.gitignore`).

## Scope Detection
*   **Infer Scope:** Look at file paths.
    *   If changes are isolated (e.g., `src/auth/`, `lib/utils.ts`), use that as scope (e.g., `auth`, `utils`).
    *   If changes are global or spread across many modules, omit the scope.

## Subject Rules
*   Max 50 characters.
*   Use **imperative mood** (e.g., "add", "fix", "change").
*   Lowercase start, no trailing period.
*   **NO BACKTICKS**: Never use backticks (`) in the subject.

## Body Formatting
*   Blank line after subject.
*   Explain **intent** and **reasoning** ("why", not just "what").
*   Use bulleted lists (`-`) for multiple distinct changes.
*   Wrap at 72 characters.
*   **NO BACKTICKS**: Never use backticks (`) in the body. Use single quotes (') instead if needed.

## Breaking Changes
*   **Detection:** Look for removal of public API, signature changes, or incompatible config changes.
*   **Format:** Footer MUST start with `BREAKING CHANGE:` followed by description and migration instructions.

## Footer
*   Reference issues using `Closes: #`.
