# Voice Food Log

Tap the mic, say what you ate, get a calorie estimate. Entries are stored on-device
(localStorage) by day.

- **Frontend:** `index.html` — served via GitHub Pages (HTTPS, required for
  microphone access on iOS Safari). Speech is captured with the Web Speech API.
- **Backend:** a Cloudflare Worker (deployed separately) that estimates calories
  with the Anthropic API. Set its URL in the app's Settings screen.

## Phone setup

1. Open the GitHub Pages URL in Safari.
2. Share → **Add to Home Screen**.
3. Open the app → ⚙︎ Settings → paste the Worker URL → Save.
