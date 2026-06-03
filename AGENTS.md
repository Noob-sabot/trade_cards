# AGENTS.md

Guidance for AI agents working in the **trade_cards** repository.

## Repository type

This workspace is **documentation-only** (business ideation under `business-ideation/`). There is no application source code, `package.json`, Docker Compose, database, or CI configuration yet. The planned product is an Australia-first collectible card trading platform (Phase 1: AFL Team Coach 2026).

See `business-ideation/README.md` and `business-ideation/platform-concept-and-compliance-plan.md` for product scope and the “Immediate next steps” implementation roadmap.

## Cursor Cloud specific instructions

### What runs today

No long-lived services are required for this repository. There is nothing to `npm run dev`, migrate, or docker-compose up until the Next.js app is scaffolded per the planning docs.

### Smoke test (docs “hello world”)

From the repo root, verify planning artifacts and basic markdown quality:

```bash
# Required files and Phase 1 keywords
for f in business-ideation/README.md \
         business-ideation/platform-concept-and-compliance-plan.md \
         business-ideation/monetization-and-compliance-notes.md; do
  test -f "$f" || exit 1
done
rg -q "Phase 1" business-ideation/
rg -q "AFL Team Coach" business-ideation/

# Optional: markdown lint (no repo config required)
npx --yes markdownlint-cli2 "business-ideation/**/*.md"
```

A passing smoke test confirms the ideation bundle is present and internally consistent enough for agent work; it is not a substitute for app E2E tests once code exists.

### When application code lands

Per `platform-concept-and-compliance-plan.md`, the intended stack is **Next.js**, **PostgreSQL**, **Prisma**, background jobs for matching, and object storage for card photos. Future agents should follow whatever `package.json` / README the scaffold introduces; until then, do not assume ports, env vars, or migration commands.

### Lint / test / build

| Task | Today |
|------|--------|
| Lint | Optional: `npx --yes markdownlint-cli2 "business-ideation/**/*.md"` |
| Test | None in repo |
| Build | None in repo |
| Run | None in repo |
