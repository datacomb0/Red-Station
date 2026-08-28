# REDLINE — Morse Field Station

An interactive Morse code translator designed as an 80s field-radio console. REDLINE combines live text/Morse conversion, an animated telegraph key, audio playback, and a dark-red ambient interface.
Live domain: https://red-station.netlify.app/
![REDLINE Morse Field Station](https://img.shields.io/badge/REDLINE-Morse%20Field%20Station-f04a35?style=for-the-badge)

## Features

- Live **Text → Morse** and **Morse → Text** translation
- Directional **Swap** control that changes both the interface and conversion flow
- Interactive telegraph key: tap for a dot, hold for a dash
- `Shift` keyboard control for manual keying
- Web Audio playback with configurable speed and tone frequency
- Telegraph lever animates in sync with Morse playback
- Live visual Morse signal display
- Adjustable WPM, frequency, and sidetone controls
- Built-in Morse alphabet and number reference
- Responsive, touch-friendly mobile layout

## Run locally

This is a dependency-free static site.

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

For the most reliable clipboard and audio behavior, run it through a local server:

```bash
npx serve .
```

Then open the local address shown in your terminal.

## Controls

| Control | Action |
| --- | --- |
| Text panel | Type a message to create Morse code |
| Morse panel | Type dots (`.`), dashes (`-`), spaces, and `/` between words |
| `SWAP` | Switch between Text → Morse and Morse → Text modes |
| `PLAYBACK` | Listen to the current Morse transmission |
| Telegraph key | Tap for a dot; hold for a dash |
| `Shift` | Keyboard alternative for the telegraph key |
| Speed / Tone | Adjust WPM and oscillator frequency |

## Project structure

```text
.
├── index.html   # Application markup
├── styles.css   # Visual system, responsive design, and animations
├── app.js       # Morse translation, audio, keyboard/key interactions
└── README.md
```

## Technology

Built with vanilla **HTML**, **CSS**, and **JavaScript**. Audio is generated in-browser with the Web Audio API; no backend or external API is required.

## Notes

- Standard Latin letters, numerals, and common punctuation are supported.
- Separate Morse letters with spaces and Morse words with `/`.
- Audio starts after a user action, following browser autoplay rules.

---

Built for clear signals and late-night transmissions.
