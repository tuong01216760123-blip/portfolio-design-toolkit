# React Bits — portfolio selection guide

This is a curated starting point, not an exhaustive catalogue. Confirm current availability against the official React Bits docs/registry before installing.

## Hero / title

- **SplitText** — clean staggered character/word entrance.
- **BlurText** — soft-focus reveal for calm premium intros.
- **MaskedHeading** — large headline with moving image/mesh inside glyphs.
- **ScrollFloat** / **ScrollReveal** — scroll-reactive text without dominating the page.
- **TextPressure** — expressive pointer-driven display type; reserve for short hero copy.
- **VariableProximity** — subtle letter response to pointer distance.
- **DecryptedText** — useful for engineering/automation motifs when restrained.

For a professional engineering portfolio, prefer SplitText, BlurText, ScrollReveal, or VariableProximity before noisy glitch effects.

## Project / case-study cards

- **SpotlightCard** — subtle pointer illumination.
- **TiltedCard** — 3D pointer depth; keep the angle restrained.
- **MagicBento** — structured capability/case-study grids.
- **ChromaGrid** — image/project grids with hover reveal.
- **ScrollStack** — stacked case studies driven by scroll.
- **PixelTransition** — before/after or alternate visual states.
- **CardSwap** — compact rotating/stacked content.

Avoid combining TiltedCard + SpotlightCard + a heavy background shader on the same card group.

## Navigation

- **PillNav** — restrained active-state navigation.
- **GooeyNav** — expressive; use only when the rest of the interface is quiet.
- **Dock** — compact project/tool dock or optional showcase navigation.
- **StaggeredMenu** — full-screen navigation with authored motion.

## Media / showcase

- **ScrollExpand** — hero image/video expanding into a case study.
- **Masonry** — practical portfolio grid with animated reflow.
- **DomeGallery** / **CircularGallery** — immersive galleries when the media deserves the interaction.
- **ModelViewer** — for real 3D engineering artifacts, not decoration.

## Backgrounds

Calmer choices:
- **DarkVeil**
- **SoftAurora**
- **LightRays**
- **Threads**
- **GridMotion**
- **DotGrid**
- **Topography**

Heavier / more dominant:
- **LiquidEther**
- **Galaxy**
- **Dither**
- **Prism**
- **Plasma**
- **Hyperspeed**

For dense portfolio sections, prefer a static or low-motion background instead of a shader.

## Small motion

- **Magnet** for restrained CTA attraction.
- **GlareHover** for controlled highlights.
- **ClickSpark** only in playful areas.
- **AnimatedContent** / **FadeContent** for reusable entrance wrappers.
- Micro controls such as **SpringCheck**, **SquishSwitch**, or **WarmTooltip** only when a real control needs that behavior.

## Selection rule

Before installing, answer:
1. What user-facing job does this effect perform?
2. Is that job already handled by an existing project component?
3. Is there a lighter CSS/native solution?
4. Does it reinforce project identity or merely look impressive alone?

If answers 1 and 4 are weak, do not install it.
