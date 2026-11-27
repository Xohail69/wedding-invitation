# Nikah Invitation — Rizba Parveen weds Dr. Javed Ahmad

An animated, self-contained HTML invitation card (9:16, mobile-first), live at
**https://xohail69.github.io/wedding-invitation/**

- `index.html` — the whole invitation: inline CSS, inline SVG art, the music,
  and a small script that sequences the nine scenes. No build step; the only
  external request is the Google Fonts stylesheet.
- `.nojekyll` — tells GitHub Pages to serve the files as-is.

## Music

Tapping **Play invitation** starts `music.mp3` (configured via `MUSIC_SRC` in
`index.html`). It loops, fades in and out with the card, and the note button in
the bottom-right corner mutes and unmutes it.

To switch back to the built-in Web Audio API celesta score (D – Bm – G – A) or
use a different audio file, update the `MUSIC_SRC` line in `index.html`:

```js
const MUSIC_SRC = 'music.mp3';   // '' = use the generated score
```

## Viewing locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```
