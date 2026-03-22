# css-era

> *The same passion. The same subject. Five years apart.*

`css-era` is a personal archive and living showcase of growth as a frontend developer — told through a single subject: **Peaky Blinders**.

In 2021, at the very beginning of a CSS journey, a fan page was built. Red background. Ephesis font. Broken image URLs. A `font family=` that never worked. It was imperfect, honest, and exactly what every developer's first project looks like.

In 2026, the same page was rebuilt from scratch — not to erase what came before, but to place both versions side by side and let the distance speak for itself.

This repository is that conversation.

---

## Structure

```
css-era/
├── index.html          # The showcase — side-by-side comparison with annotated diff
├── v1-original/
│   └── index.html      # The 2019 version, faithfully restored and bug-fixed
└── v2-modern/
    └── index.html      # The 2026 version — cinematic, animated, production-grade
```

---

## What's inside

### `index.html` — The Showcase
A split-screen comparison page. The left panel renders the original 2019 code with honest annotations — hoverable bug tags that surface exactly what went wrong (`font family=` instead of `font-family:`, missing semicolons, Google image search URLs used as background images). The right panel shows the modern rebuild, live, interactive, and fully functional. A code diff block at the bottom maps the exact syntax evolution. This is the page meant to be shared.

### `v1-original/` — 2019
The beginning. Red `background-color`. The Ephesis font. White text. Simple character boxes with `border: 2px solid white`. Bugs fixed silently so it actually renders, but the spirit — the boldness of a beginner who just learned what CSS *was* — kept completely intact.

### `v2-modern/` — 2026
A full cinematic rebuild. Coal and gold palette. `Cinzel Decorative` display font. Film grain overlay. Scroll-triggered reveal animations. Character cards with multi-layer hover effects: staggered line-by-line text reveals, unique atmospheric gradients per character, gold corner bracket animations, scanline texture, and in-character quotes. CSS custom properties throughout. Fully responsive.

---

## The character hover system (v2)

Each of the four character cards in the modern version has a distinct hover experience:

| Character | Hover atmosphere | Quote source |
|---|---|---|
| Thomas Shelby | Gold + deep crimson radial gradient | Series 2 |
| Polly Gray | Violet + gold radial gradient | Series 3 |
| Grace Burgess | Cool blue-silver + gold gradient | Series 1 |
| Arthur Shelby | Raw red + iron grey gradient | Throughout |

On hover: the character monogram fades back, the base name slides out, and a reveal layer animates in — name, actor, a character description, a ruled divider, and a signature quote — each line entering with a staggered `translateY` transition. Gold corner brackets slide into position. A subtle scanline texture overlays the card.

---

## The diff

```diff
- font family= "Ephesis", cursive;
+ font-family: "Cinzel Decorative", serif;

- background-image: url("google.com/imgres?…");
+ background: radial-gradient(ellipse at 50% 0%, rgba(201,168,76,0.15), transparent);

- border: 2px solid white;
+ transform + opacity + transition: all 0.45s cubic-bezier(0.25, 0.46, 0.45, 0.94);

- color: white  /* missing semicolon */
+ --gold: #c9a84c; /* CSS custom properties */
```

---

## Why this exists

Because the red background deserves respect.

Not every project needs to be polished to matter. The 2019 version was built by someone who had just discovered that you could change a webpage's background color and thought that was *incredible*. That instinct — to just build something, broken URLs and all — is exactly the instinct that leads here, five years later.

`css-era` is a reminder that expertise is just enthusiasm with time behind it.

---
## Web Page

<p align="center"> <img width="1918" height="912" alt="Original" src="https://github.com/user-attachments/assets/01aa56f5-3945-4a56-b967-86a719e53ac6" /> <strong>Original</strong></p>

<p align="center"> <img width="1918" height="897" alt="New" src="https://github.com/user-attachments/assets/9de13ad6-8d40-49a6-a114-56a5ae31696b" /> <strong>New</strong></p>

<p align="center"> <img width="1918" height="907" alt="Comparison" src="https://github.com/user-attachments/assets/60451ee6-43d3-4a3c-8a08-2e1088a63896" /> <strong>Comparison</strong></p>

## Part of NEXUS

This project is part of **NEXUS** — a personal portfolio and development system documenting the full arc of a frontend journey, from first lines to production-grade interfaces.

---

*Built with care. Started with a red background.*
