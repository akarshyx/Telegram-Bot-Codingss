# [Project name]

_Replace the heading above with the project's name, and this line with one sentence describing what this app does for users._

## Run & Operate

- `pnpm --filter @workspace/api-server run dev` — run the API server (port 5000)
- `pnpm run typecheck` — full typecheck across all packages
- `pnpm run build` — typecheck + build all packages
- `pnpm --filter @workspace/api-spec run codegen` — regenerate API hooks and Zod schemas from the OpenAPI spec
- `pnpm --filter @workspace/db run push` — push DB schema changes (dev only)
- Required env: `DATABASE_URL` — Postgres connection string

## Stack

- pnpm workspaces, Node.js 24, TypeScript 5.9
- API: Express 5
- DB: PostgreSQL + Drizzle ORM
- Validation: Zod (`zod/v4`), `drizzle-zod`
- API codegen: Orval (from OpenAPI spec)
- Build: esbuild (CJS bundle)

## Where things live

_Populate as you build — short repo map plus pointers to the source-of-truth file for DB schema, API contracts, theme files, etc._

## Architecture decisions

_Populate as you build — non-obvious choices a reader couldn't infer from the code (3-5 bullets)._

## Product

_Describe the high-level user-facing capabilities of this app once they exist._

## User preferences

_Populate as you build — explicit user instructions worth remembering across sessions._
- Keep casino messages professional: prefer the static, non-animated premium emoji icons shown in the user's latest reference image for normal casino UI text; use standard Unicode as a fallback instead of turning every symbol into an animated custom emoji. Use animated emojis only in locations the user explicitly marks. Wait for the user's marked examples before changing emoji placement; do not replace, rename, or modify the existing emoji packs.
- Use the public `RaikaRanks` set only for rank labels; the owner-triggered copy should be titled “Rollers Rank Emoji”.
- Use `ST_5PUsQEHbxN5l8Vy2fX6sGtMS_QszrcOUd9xfUjno_by_StickersPackRobot` only for the Diamonds game, not general casino text.

## Gotchas

_Populate as you build — sharp edges, "always run X before Y" rules._

## Pointers

- See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details
