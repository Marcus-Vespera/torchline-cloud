# Torchline Cloud — brand theme

The palette Marcus approved 2026-11-24 ("I really like this color theme"). Every value here is already a
CSS variable in `index.html` under `:root`. To restyle the site, change the token, not the component.

## Surface — midnight blue into purple

| Token | Hex | Use |
|---|---|---|
| `--void` | `#04051a` | page base, near-black navy |
| `--deep` | `#070828` | top of the background gradient |
| `--plum` | `#140a33` | lower background, the purple floor |
| `--plum-2` | `#1d0d45` | raised purple surfaces |
| `--surface` | `rgba(255,255,255,.038)` | cards |
| `--surface-2` | `rgba(255,255,255,.062)` | hover / raised cards |
| `--hairline` | `rgba(168,140,255,.20)` | borders |
| `--hairline-2` | `rgba(168,140,255,.34)` | emphasised borders |

## Ink

| Token | Hex | Use |
|---|---|---|
| `--ink` | `#f4f3ff` | headings, primary text |
| `--ink-2` | `#cdc9ee` | body copy |
| `--muted` | `#918dba` | secondary copy |
| `--muted-2` | `#6f6b96` | labels, meta, indices |

## Neon accents

| Token | Hex | Meaning |
|---|---|---|
| `--cyan` | `#59e6ff` | primary action, "host" / cloud, live state |
| `--violet` | `#9a6cff` | secondary accent, agents, structure |
| `--magenta` | `#ff53d6` | traffic, edge, emphasis pops |
| `--ember` | `#ff8a4c` | the torch, warmth, brand heat |
| `--ok` | `#4ce6a4` | included / verified / security |

The torch mark uses a four-stop gradient — cyan → violet → magenta → ember — so the brand runs cold to hot
in one object. Keep that order.

## Type

- Display: **Bricolage Grotesque** (600, tight `-0.02em`–`-0.035em`)
- Body: **Instrument Sans** (400/500)
- Meta, prices, indices: system mono, tabular numerals

Deliberately not Inter.

## Geometry

`--r-sm 8px` · `--r-md 14px` · `--r-lg 22px` · `--r-xl 30px`
Spacing scale `6 / 12 / 18 / 26 / 38 / 56 / 84 / 120`, container `1280px`.

## Texture

- Background: three radial washes (magenta top-right, violet top-left, cyan bottom) over a vertical
  `--deep → --void → --plum` gradient.
- Grid: fixed 64px square grid at `rgba(168,140,255,.055)`, masked with a radial so it fades out below the
  hero. This is the "railway map" texture that echoes the hero's perspective floor.
- Grain: SVG fractal-noise overlay at 5% opacity, `mix-blend-mode: overlay`.
- Glow: always soft and wide (`0 0 24–40px` at 20–35% alpha). No hard shadows.
