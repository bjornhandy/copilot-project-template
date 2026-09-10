# Agent Instructions

Before making changes:

1. Inspect the relevant existing code.
2. Inspect related tests.
3. Look for similar existing implementations.
4. Understand the current architecture.
5. Make the smallest coherent change.
6. Run relevant tests afterward.

Do not:

- Rewrite unrelated code.
- Remove functionality without instruction.
- Introduce unnecessary dependencies.
- Disable tests to make changes pass.
- Replace existing architecture without understanding why it exists.

When debugging:

1. Reproduce the issue.
2. Determine expected behavior.
3. Find the first incorrect state.
4. Identify the root cause.
5. Fix the root cause.
6. Add a regression test.
