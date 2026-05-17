---
name: skill-git-commit
description: Expert Git commit message generation following Conventional Commits. Use when the user wants to commit changes, needs help writing a commit message, or asks to "commit this".
---

# Git Commit Generator

This skill transforms staged changes into professional, meaningful commit messages.

## Workflow

1.  **Analyze Staged Changes**: Use `git diff --staged` to understand the code changes.
2.  **Apply Standards**: Follow the detailed rules in [references/commit-standards.md](references/commit-standards.md).
3.  **Generate Output**: Produce a commit command that the user can run.

## Guidelines

- **Context First**: Always read the diff before proposing a message.
- **No Backticks**: **CRITICAL**: Never include backticks (`) in the commit message or any part of the output. Gemini CLI interprets backticks as shell commands.
- **Why over What**: Prioritize the reasoning behind the change in the message body.
- **Breaking Changes**: Be extremely vigilant about breaking changes and document them in the footer as per the standards.

## Example Usage

When a user says "Commit these changes", you should:
1. Run `git diff --staged`.
2. Review the output.
3. Construct the message following the standards.
4. Output the final `git commit` command for the user.
