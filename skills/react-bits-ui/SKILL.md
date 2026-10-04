---
name: react-bits-ui
description: Use when the user explicitly asks for React Bits, wants animated React UI/effects, or needs a polished interactive text, component, background, animation, or micro-interaction that React Bits can provide. Select and integrate components from the official React Bits registry without vendoring the library into this toolkit. Preserve the project's existing design language, accessibility, performance, and motion constraints.
---

# React Bits UI

Use React Bits as an implementation resource, not as the design director.

The user request, PRODUCT.md, DESIGN.md, and project AGENTS.md outrank this skill. A visually impressive component is not automatically appropriate.

## Source

Official project:
- Repository: https://github.com/DavidHDev/react-bits
- Documentation: https://reactbits.dev
- Pinned reference commit: `ca44b3f9ee180676a06d7de8ec6bea84cddff85b`

React Bits provides four variants:
- JavaScript + CSS: `JS-CSS`
- JavaScript + Tailwind: `JS-TW`
- TypeScript + CSS: `TS-CSS`
- TypeScript + Tailwind: `TS-TW`

Do not copy the React Bits repository wholesale into this toolkit or a downstream project. Install only selected components from the official registry.

## Workflow

1. Inspect the downstream project:
   - confirm it is React;
   - detect JavaScript vs TypeScript;
   - detect CSS vs Tailwind;
   - read existing design tokens/components.

2. State the job of the effect in one sentence.

3. Choose the smallest React Bits component that solves that job. Read [references/portfolio-picks.md](references/portfolio-picks.md) for a curated starting point.

4. Install from the official registry:

   ```bash
   npx shadcn@latest add https://reactbits.dev/r/<Component>-<LANG>-<STYLE>
   ```

   or:

   ```bash
   npx jsrepo@latest add https://reactbits.dev/r/<Component>-<LANG>-<STYLE>
   ```

   Example for TypeScript + Tailwind:

   ```bash
   npx shadcn@latest add https://reactbits.dev/r/BlurText-TS-TW
   ```

5. Inspect the installed component and its dependencies before integrating. Components may depend on packages such as `motion`, `gsap`, `three`, or `ogl`. Do not introduce a heavy graphics dependency for a minor decorative gain.

6. Adapt it to project tokens, typography, spacing, color and motion language. The React Bits demo appearance is not the target art direction.

7. Verify:
   - desktop and mobile;
   - keyboard/focus where interactive;
   - `prefers-reduced-motion`;
   - console/runtime errors;
   - loading and layout shift;
   - touch behavior;
   - animation smoothness and performance regressions.

## Portfolio rules

- Prefer one authored visual moment over many unrelated effects.
- Never stack multiple animated backgrounds behind the same content area.
- Avoid custom cursor effects on touch devices.
- Keep body copy readable; animation must not become the information hierarchy.
- Use WebGL/shader effects sparingly and provide simpler mobile/reduced-motion behavior when necessary.
- Do not add an effect merely because it exists in the library.
- Reuse a coherent motion language across related sections.

## Licensing

React Bits is licensed under **MIT + Commons Clause**. At the pinned commit, it permits use, including commercial use, as part of an application, website, or product, but restricts selling, sublicensing, or redistributing the components themselves as a component library/bundle/ported version.

This toolkit intentionally contains **no React Bits component source code**. Install components directly from the official upstream registry. See [references/source-and-license.md](references/source-and-license.md).
