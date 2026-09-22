# Hover-Card-effect

A sleek UI project showcasing interactive 3D hover cards built with pure HTML and CSS — no JavaScript, no build step.

When a card is hovered, tapped or focused with the keyboard, the cover tilts back in 3D, the title lifts forward and the character pops out of the frame.

## Features

- Pure HTML + CSS (perspective, `translate3d`, gradient overlays)
- Works with mouse hover, touch (tap to activate) and keyboard (`Tab` to a card)
- Responsive: cards wrap into a single column on narrow screens
- Respects `prefers-reduced-motion`
- Optimised images (~550 KB total)

## Project structure

```
.
├── index.html      # Markup for the cards
├── style.css       # Layout, 3D transforms and transitions
└── Images/         # Cover, title and character art for each card
```

## Running locally

Open `index.html` directly in a browser, or serve the folder:

```bash
npx serve .
# or
python -m http.server 5500
```

## Customising

- Card size: change `--card-height` in `:root` in `style.css` (width follows at a 2:3 ratio).
- Animation speed: change `--duration`.
- Add a card: copy a `.card` block in `index.html` and point it at a new cover (2:3 JPG), title (transparent PNG) and character (transparent WebP).

## Credits

Hover effect inspired by [@coding.stella](https://www.instagram.com/coding.stella/). The card artwork is not original to this repository — check its source and licence before reusing it.
