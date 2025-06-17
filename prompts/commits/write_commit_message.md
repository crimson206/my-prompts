## commit_message file prompt:

```
Based on the git diff analysis above, write a commit message in commit_message file:

**Requirements:**
- Follow Conventional Commits format: `type(scope): description`
- Types: feat, fix, docs, style, refactor, test, chore
- Scope: main change area (src/, components/, utils/, etc.)
- First line under 50 chars, imperative present tense
- Add body for significant changes (wrap at 72 chars)

**Analysis focus:**
- New/deleted files in src/ folder
- Major logic changes in existing files
- API modifications
- Dependency changes
- Bug fixes

Write appropriate commit message for current changes.
```