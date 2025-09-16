# app-loading-simulator

Simple static page that simulates an app “loading” for a configurable duration, then shows a loaded state. Designed for GitHub Pages hosting.

Usage
- Host the repo with GitHub Pages (or open `index.html` directly).
- Pass the delay in milliseconds via the `duration` query param.

Examples
- Local file: `index.html?duration=3000` (3 seconds)
- GitHub Pages: `https://<user>.github.io/app-loading-simulator/?duration=5000`

Details
- Param: `duration` (ms). Missing/invalid values default to `0` (instant load).
- Max duration is capped at 10 minutes to prevent mistakes.
- The loading screen shows a spinner; after the delay it switches to a static “Application Loaded” view and displays the simulated delay.
