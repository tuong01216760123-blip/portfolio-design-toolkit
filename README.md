# Portfolio Design Toolkit

Pinned reusable frontend-design skills for portfolio and web-app work.

## Included

- `portfolio-director` — local routing and precedence rules.
- `clone-website` — JCodesMore website reverse-engineering skill.
- `redesign-existing-projects` — Taste Skill for existing projects.
- `gpt-taste` — Taste Skill variant oriented to GPT/Codex.
- `impeccable` — Codex/OpenAI-compatible Impeccable skill.

## Precedence

1. The user's current explicit request.
2. The downstream project's `PRODUCT.md` and `DESIGN.md`.
3. Project-specific `AGENTS.md`.
4. `portfolio-director`.
5. Specialist third-party skills.

Third-party skills advise implementation; they must not silently replace an established project identity.

## Recommended routing

- Existing portfolio: `portfolio-director` → `redesign-existing-projects` → `impeccable` verification/polish.
- Generic or timid visual output: add `gpt-taste`.
- Reference website: `clone-website` for observation/reverse-engineering, then reinterpret through the project's own `DESIGN.md`.
- Pre-release: `impeccable audit` and/or `impeccable polish`.

## Install

The folders under `skills/` follow the Agent Skills convention and can be discovered by compatible skill installers:

```bash
npx skills add https://github.com/tuong01216760123-blip/portfolio-design-toolkit
```

See `SOURCES.md`, `sources.lock.json`, and `THIRD_PARTY_LICENSES.md` for provenance and exact pins.
