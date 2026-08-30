# Artisans

Artisan applications built with Art JS. Hand-crafted micro applications for humans working with Art and Artificials.

## Recommended Reading

Agents SHOULD scan these files for definitions and resource locations when faced with uncertainty or ambiguity that may result from missing resources.

- `_guide.md` — this file: system overview, layout, records, and operating instructions.
- `apps/art-mantras/_guide.md` — the Art Mantras application guide.

## Repository Layout

```
_guide.md           — this file
_records/           — project and repository records
apps/               — application packages
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

#### Operating Instructions: Setting Up

**Instructions:**

Run from the repository root (monorepo):

```bash
npm ci # to install dependencies.
```

#### Operating Instructions: Verifying Commit

**Instructions:**

Runs automatically on pre-commit hook (from the repository root):

```bash
npm run ci # lint, build and test
```

#### Operating Instructions: Verifying Completion

**Instructions:**

Run from the repository root (monorepo):

```bash
npm run ci # lint, build and test
```
