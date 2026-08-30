# Art Mantras

A micro app that generates mantras through a 12-step race.

## Recommended Reading

Agents SHOULD scan these files for definitions and resource locations when faced with uncertainty or ambiguity that may result from missing resources.

- `_guide.md` — this file: package overview, layout, records, workflows, and operating instructions.
- `_wip.md` — the parking lot and progress tracker — open actions, questions and blockers (no dones!).
- `_architect.md` — the architecture — Why, What, How, Follow-ups (no code).
- `_pseudo.md` — the function declarations — name, params, responsibility, pseudo code — entry point first, grouped by layer.

## Package Layout

```
_guide.md           — this file
_backlog/           — plans, instructions, reports
_records/           — package and deployment records
_architect.md       — project direction, principles, and follow-ups
_pseudo.md          — pseudo-code contract
_wip.md             — parking lot and progress tracker
src/                — application source
scripts/            — build scripts
```

## Records Management

Records are co-located with the resources they describe in `_records/` directories:

- **Package:** `_records/package.art`
- **Deployments:** `_records/static-web-deployment.art`
- **Environments:** `_records/production-environment.art`, `_records/staging-environment.art`

## Knowledge References

This package does not maintain a dedicated architecture reference; see `_architect.md` for project direction and `_pseudo.md` for the pseudo-code contract.

## Workflows

### Planning Work

This project plans its work with the workflow defined in `$DOMAINS/work/workflows/planning-work/workflow.art`.

- The backlog lives at `_backlog/` with subdirectories such as `/3-now` and `/4-next/`.
- The short-term focus is captured in `_wip.md`.
- The requirements, use cases, and principles are captured in `_architect.md`.

## Operating Instructions

### Operating Instructions: Setting Up

**Instructions:**

Run from the repository root (monorepo):

```bash
npm ci # to install dependencies.
```

### Operating Instructions: Verifying Step

**Instructions:**

Run from this package directory:

```bash
npm run lint:fix # to fix formatting issues automatically
npm run lint # to report other issues (prettier, eslint)
npm run build # to bundle the application
```

### Operating Instructions: Verifying Completion

**Instructions:**

Run from this package directory:

```bash
npm run ci # lint and build
```
