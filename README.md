# The No Button

A big red button that counts your nos. It's a playful way to practice
saying no: every time you turn something down, press the button.

## Features

- A big red emergency-stop style button with sound, vibration and a little
  "NO!" burst on every press
- A different slogan around the button every time you open the app
  ("Protect your peace", "Your time, your rules", "Say no without guilt",
  "Boundaries are healthy")
- Today's count, shown as a number and as tally marks in groups of five
- An encouraging line after each press, plus milestone messages
  (1, 5, 10, 25, 50, 100, 250, 500 nos)
- An adjustable daily goal with a progress bar
- Stats for this week, all time and your day streak
- Undo for accidental presses, and a sound toggle
- Light and dark mode
- Installable on your home screen and works offline

## Privacy

Everything stays on your device. Your count lives in the browser's
`localStorage`; there is no server, no account and no tracking.
Clearing your browser data resets the count.

## Run locally

It's plain HTML, CSS and JavaScript with no build step. The service worker
needs to be served over HTTP, so use any static server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

The workflow in `.github/workflows/pages.yml` publishes the app to GitHub
Pages on every push to `main`. Turn it on once under
**Settings → Pages → Build and deployment → Source: GitHub Actions**.

After changing any app file, bump `CACHE` in `sw.js` so installed copies
pick up the update.

## Install on your phone

- **iPhone (Safari):** Share → Add to Home Screen
- **Android (Chrome):** menu → Install app / Add to Home screen
