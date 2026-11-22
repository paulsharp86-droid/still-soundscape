# STILL PWA 0.4 — installable offline prototype

This is the first installable Progressive Web App shell for STILL. It includes an offline cache, home-screen manifest/icon, the native Web Audio prototype, four tone voices, pink noise, and a rudimentary delayed-response interaction idea.

## Current limits
- This package does **not yet contain a SoundFont (SF2/SF3) or SpessaSynth playback library**. Those require a built/bundled library and a redistributable bank; this is a testable PWA shell and audio interaction prototype.
- Native oscillator voices are placeholder timbres, not samples.
- For offline installability, host the folder over HTTPS (GitHub Pages is an easy option). Service workers do not install from a plain `file://` folder.

## Quick Android install
1. Host this folder over HTTPS, e.g. GitHub Pages.
2. Open the URL in Chrome on Android.
3. Use Chrome menu (⋮) → **Install app** or **Add to Home screen**.
4. Launch STILL from the home screen. It should cache the shell for offline opening after the first visit.

## Audio use
Press Begin Soundscape once. Browser audio requires a user gesture. Start with noise at 0% and the instrument faders up while testing. Adjust Density for activity.

## Next engineering milestone
Bundle `spessasynth_lib` into the app build, copy its AudioWorklet processor alongside the bundled JavaScript, include a properly licensed compact SF2 bank, load it locally at runtime, and map the four instrument channels to presets. Then replace the oscillator placeholders while retaining the PWA caching and UI.
