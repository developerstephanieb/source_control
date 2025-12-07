# 02: Conventional Commits

Conventional Commits is a lightweight convention for formatting commit messages. It provides a set of rules for creating an explicit commit history, which makes it easier to write automated tools on top of a project (such as generating changelogs or determining semantic version bumps).

---

## Message Structure

A conventional commit message consists of a header, an optional body, and an optional footer. The header has a specific format that includes a type, an optional scope, and a subject description.

- Type: Describes the category of the change (e.g., fix, feat).

- Scope (Optional): A noun describing the section of the codebase affected, enclosed in parentheses (e.g., (parser), (api)).

- Subject: A short, imperative description of the change.

- Body (Optional): A longer description of the motivation for the change.

- Footer (Optional): Metadata about the change, such as breaking changes or ticket references.

```

```

---

## Standard Types

The commit type communicates the intent of the change. These types often mirror the prefixes used in branch naming but serve a different purpose (history vs. workflow).

- `feat:`: A new feature (correlates with MINOR in Semantic Versioning).

- `fix:`: A bug fix (correlates with PATCH in Semantic Versioning).

- `docs:`: Documentation only changes.

- `style:`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).

- `refactor:`: A code change that neither fixes a bug nor adds a feature.

- `perf:`: A code change that improves performance.

- `test:`: Adding missing tests or correcting existing tests.

- `chore:`: Changes to the build process or auxiliary tools and libraries such as documentation generation.

```
# A feature commit
feat(auth): add google oauth login support

# A fix commit
fix(api): handle timeout error on slow connections

# A chore commit
chore: update eslint configuration
```