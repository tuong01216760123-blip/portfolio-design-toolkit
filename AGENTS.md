# Toolkit maintenance rules

- Treat `skills/clone-website/`, `skills/redesign-existing-projects/`, `skills/gpt-taste/`, and `skills/impeccable/` as vendored upstream material.
- Do not casually edit vendored files. Update them from the exact pinned source commit in `sources.lock.json`.
- `skills/portfolio-director/` is local toolkit logic.

For downstream projects, explicit user instructions and project `PRODUCT.md` / `DESIGN.md` outrank all bundled skills.

Use reference websites to learn layout, motion, responsive behavior, component boundaries and implementation patterns. Do not copy third-party branding, proprietary copy, protected assets, or create deceptive replicas.
