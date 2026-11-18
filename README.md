# Toddler Sensory Playground

An interactive, full-screen sensory playground designed specifically for toddlers. Every tap, click, drag, or keyboard press creates joyful 60fps animations and harmonious musical notes—with zero dead zones and no harsh sounds.

## Live App URL

- https://toddler-playground.ai.studio/

## Features

- **Zero Dead Zones:** Clicking, tapping, dragging, or mashing any key triggers playful animations and sound.
- **60fps HTML5 Canvas Physics:** Renders floating ambient bubbles, expanding color ripples, star/heart/bubble particle bursts, oversized alphabet/number badges, and bouncing animal & toy emojis.
- **Harmonious Web Audio Synthesizer:** Synthesizes soft marimba/xylophone notes tuned to a C Major Pentatonic scale (`C4`–`C6`), cheerful bubble pops, and sparkle chimes on pointer drag—so any random combination of keys sounds pleasant.
- **Tactile Sensory Dock:** Six oversized, colorful bottom buttons (Duck, Star, Balloon, Rocket, Rainbow, Puppy) mapped to musical notes.
- **Toddler-Safe UX:** Disables scrolling, text selection, and accidental browser navigation shortcuts (`Space`, `Tab`, `Arrow` keys, etc.).
- **Parent Hold-to-Mute Control:** Discreet top-right sound toggle requires holding for ~1.1 seconds so toddlers cannot accidentally mute the app.

## Project Structure

- `public/index.html` — Complete frontend application (HTML5 Canvas, Web Audio API synthesizer, Tailwind CSS layout)
- `public/favicon.ico` — App favicon
- `server.js` — Express static server serving `public/` on port `3000`
- `package.json` — Node.js scripts and `express` dependency
- `firebase.json` — Static hosting configuration for Firebase Hosting

## Running Locally

```bash
npm install
npm run dev
```

Then open `http://localhost:3000` in your browser.

## Deploying to Free Firebase Hosting (Spark Plan)

```bash
npm install -g firebase-tools
firebase login
firebase use --add
firebase deploy --only hosting
```