# React Bits source and license

- Official repository: https://github.com/DavidHDev/react-bits
- Official docs: https://reactbits.dev
- Toolkit reference commit: `ca44b3f9ee180676a06d7de8ec6bea84cddff85b`
- License at that commit: MIT + Commons Clause License Condition v1.0

## Toolkit integration model

React Bits component source is **not vendored** into Portfolio Design Toolkit.

The `react-bits-ui` skill:
- helps choose an appropriate component/effect;
- selects the correct JS/TS + CSS/Tailwind variant;
- directs installation from the official React Bits registry;
- requires adaptation and QA in the downstream app.

This avoids redistributing React Bits as a component bundle.

## License behavior relevant to downstream use

At the pinned commit, upstream permits use, including commercial use, as part of an application, website, or product, while restricting selling, sublicensing, or redistributing the components themselves as components/bundles/ported versions.

Re-check upstream terms before redistributing React Bits code outside an end application.
