---
argument-hint: "<issue-number>"
description: "Implement feature from issue, add tests, push PR"
model: claude-opus-4-5-20251101
---

Implement feature from GitHub issue #$ARGUMENTS. Follow these steps:

1. **Understand**: Use `gh issue view $ARGUMENTS` to get issue details, acceptance criteria, and comments
2. **Explore**: Search the codebase for relevant patterns, similar implementations, and integration points
3. **Plan**: Outline the implementation approach and identify files to create/modify
4. **Branch**: Create a feature branch (`feat/$ARGUMENTS-<short-desc>`)
5. **Implement**: Build the feature following existing code patterns and conventions
6. **Test**: Write comprehensive tests covering the new functionality
7. **Verify**: Run the full test suite, linting, and type checking
8. **Submit**: Commit, push, and create a PR referencing the issue

Use extended thinking for complex analysis.
