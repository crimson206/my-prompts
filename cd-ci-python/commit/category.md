## Module

---
priority: 0
---

When there are changes in the src/ folder,

typically feat, fix, perf, or other related classifications will be used.

The AI determines the extent of changes and decides how to update the semantic version.

Since the version changes are determined by the AI, in the case of pyproject.toml, the AI should modify it according to this decision and commit it along with the src content.


## Docs

---
priority: 2
---

Changes in README.md or within docs/ are classified as docs.

If the module version has been updated, documents should also be updated.

If version information is missing in two --- sections, it should be added.

If the version doesn't match the current version in pyproject.toml, the document should be reviewed.

Modify based on the current state, latest version tag differences, and commit message content.

Of course, if there are no special changes, just updating the version is sufficient.

Consult with the developer if necessary.


## Examples

---
priority: 1
---

examples/ contains examples of the actual operation of the module.

When AI is tasked with writing unit tests, they often focus on useless things while ignoring the overall flow of module implementation.

So examples are written as replacements. These examples also serve as tests later.

Therefore, examples/ are committed as test along with tests/.


## Dev

---
priority: 2
---

### Runsh

Runsh is a module that directly converts .sh files into CLI commands.

The .runsh/ folder typically contains scripts loaded to help with cd/ci tasks.

Since there's no direct impact on the module, it's classified as chore. 