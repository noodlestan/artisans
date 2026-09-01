# Artisans

Artisan applications built with Art JS. Hand-crafted micro applications for humans working with Art and Artificials.

## Recommended Reading

Agents SHOULD scan these files for relevant clarifications when faced with ambiguity or omissions that may result from missing definitions.

- `_guide.md` — this file: system overview, layout, setup, verification.
- `apps/art-mantras/_guide.md` — the Art Mantras application guide.

## Repository Layout

```
_guide.md    — this file
_records/    — records (project, repository, namespaces, dependency, scaffolders, scripts)
apps/        — application packages
```

## Projects

| Project     | Guide                        | Backlog                      |
| ----------- | ---------------------------- | ---------------------------- |
| Art Mantras | `apps/art-mantras/_guide.md` | `apps/art-mantras/_backlog/` |

## Records Management

Records are co-located with the resources they describe in `_records/` directories:

- **Project:** `_records/project.art`
- **Repository:** `_records/repository.art`
- **Namespace:** `_records/namespace.art`
- **License:** `_records/license.art`
- **Packages:** `{package-path}/_records/package.art`
- **Deployments:** `{app-path}/_records/static-web-deployment.art`

## Operating Instructions

### Operating Instructions: Setting Up

**Instructions:**

Run from the repository root (monorepo):

```bash
npm ci # to install dependencies.
```

### Operating Instructions: Verifying Completion

**Instructions:**

Runs automatically on pre-commit hook (from the repository root):

```bash
npm run ci # lint, test and build
```
