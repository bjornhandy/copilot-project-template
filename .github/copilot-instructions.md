# GitHub Copilot Repository Instructions

## General

- Prefer clean, maintainable, production-ready code.
- Follow the existing architecture and conventions in the repository.
- Inspect existing code before introducing new patterns.
- Do not modify unrelated code.
- Do not remove existing functionality unless explicitly requested.
- Prefer simple, explicit implementations over unnecessary abstractions.

## Security

- Never hardcode passwords, API keys, tokens, credentials, or secrets.
- Validate all external and user-provided input.
- Use parameterized SQL.
- Check authentication and authorization independently.
- Follow secure coding practices.
- Consider common OWASP vulnerabilities.

## Architecture

- Maintain separation of concerns.
- Keep business logic outside controllers and views where appropriate.
- Reuse existing services, utilities, and abstractions.
- Avoid unnecessary dependencies.
- Preserve backwards compatibility unless explicitly requested otherwise.

## Testing

- Add or update tests for meaningful changes.
- Run relevant tests after implementation.
- Do not disable tests simply to make a build pass.

## Debugging

- Identify the root cause before applying a fix.
- Do not hide exceptions or errors without understanding them.
- Add regression tests when fixing bugs.

## Communication

- Briefly explain significant architectural decisions.
- When multiple valid approaches exist, recommend one and explain why.
