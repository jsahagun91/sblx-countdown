# Super Bowl Countdown

A single-page countdown experience for Super Bowl kickoff with a video backdrop, centered branding, and responsive layout.

## Features
- Background video with a red/cyan distortion overlay
- Kanit font timer with fixed-width digits to avoid layout shifting
- Side-by-side logos that scale for desktop and mobile
- Mobile-friendly, full-viewport layout

## Assets
All required assets are already included in `assets/`:
- `assets/ggb.mp4`
- `assets/PEP_TITAN_Logo_Globe_FullColor_RGB_NoBG.webp`
- `assets/Super_Bowl_LX_Logo.svg.webp`

## Run Locally
Open the file directly in your browser:
- `index.html`

If you prefer a local server, you can use any static server (optional).

## Update the Countdown Target
The countdown target is set in `index.html` using a UTC timestamp:
```js
const targetDate = new Date(Date.UTC(2026, 1, 8, 23, 30, 0));
```
Adjust the year, month (0-based), day, and time as needed.

## Customize
Common edits in `index.html`:
- Video overlay intensity: `.video-bg` filter and `.scrim` background
- Logo sizing: `.logos img` width/height clamp values
- Timer scale: `.time-value` font-size clamp

## Notes
- The timer uses tabular numerals for consistent spacing.
- All styling and behavior live in `index.html` for easy updates.
