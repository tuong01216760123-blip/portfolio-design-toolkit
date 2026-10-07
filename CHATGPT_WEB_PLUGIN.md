# ChatGPT Web personal plugin

This repository is packaged as a skills-only portable Agent Plugin.

## Recommended path

1. Download the repository as a ZIP from the main branch.
2. In ChatGPT Web, open **Plugins**.
3. Choose **Upload new or existing plugin** (or the equivalent upload action available to your account).
4. Choose **Skills only**.
5. Upload the ZIP.
6. Wait for metadata and skill scans to finish.
7. Install the resulting personal plugin.
8. Start a new **Work** chat and invoke **@Portfolio Design Toolkit**.

The package intentionally contains no MCP server. Live tools such as GitHub, Vercel, TinyFish, or other connected plugins remain separately installed and authorized by the user.

## Web-first behavior

Use **Portfolio Director** as the master workflow. It should preserve project truth before invoking specialist skills:

1. current explicit user request;
2. project PRODUCT.md;
3. project DESIGN.md;
4. project AGENTS.md;
5. Portfolio Director;
6. specialist skills.

Specialist skills should be loaded only when they materially help.

## Included skills

- portfolio-director
- redesign-existing-projects
- gpt-taste
- impeccable
- react-bits-ui
- clone-website (locally patched to treat references as evidence and avoid copying third-party identity/assets wholesale)

## Notes

- The root `plugin.json` is the portable manifest.
- `.codex-plugin/plugin.json` remains as a compatibility fallback for Codex/Desktop.
- Skills are discovered under `skills/`.
- The Web package does not depend on the local marketplace under `.agents/plugins/marketplace.json`.
- Account, plan, workspace, and regional eligibility still control whether skills-only personal plugin upload is exposed.
