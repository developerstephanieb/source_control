# 03: Branch Naming Conventions

---

## Standard Prefixes

The prefix acts as a category folder. Most Git GUI clients (like SourceTree or GitKraken) treat forward slashes as directory separators, visually grouping branches into folders based on these prefixes.

- `feature/`: Used for new features or functionality that adds value to the product.

- `bugfix/`: Used for fixing non-critical bugs in the code.

- `hotfix/`: Used for urgent fixes that must go directly to production, bypassing standard release cycles.

- `chore/`: Used for maintenance tasks that do not alter the source code functionality, such as updating build scripts or dependencies.

- `docs/`: Used for changes that only affect documentation.

- `refactor/`: Used for code changes that neither fix a bug nor add a feature, but improve code structure.

- `release/`: Used for preparing a new production release (e.g., updating version numbers).

```
# A new feature branch
git checkout -b feature/dark-mode-toggle

# A maintenance branch
git checkout -b chore/upgrade-node-version

# A documentation branch
git checkout -b docs/update-readme-instructions
```

---

## Integration Ticket IDs

Including the Ticket ID in the branch name creates a traceable link between the source code and the task requirements.

- Prefix Integration: The ID usually follows the category prefix.

- Traceability: CI/CD tools can scan the branch name to automatically link the code to the specific ticket in systems like Jira or Linear.

- Placement: The ID should come before the description so it is easily searchable.

```
# Pattern: prefix/ID-description

# Linking to ticket #42 regarding a password reset
git checkout -b feature/PROJ-42-password-reset

# Linking to ticket #404 regarding a broken link
git checkout -b bugfix/PROJ-404-fix-broken-link
```

