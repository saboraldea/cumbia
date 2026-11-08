# Cumbia Club — FM1 groovebox prototype

An interactive, browser-based prototype for an eight-part cumbia groovebox concept inspired by the M-VAVE FM1. It includes a four-bar, 64-step sequencer; instant cumbia patterns; Euclidean rhythm generation; browser-synthesized Latin-inspired percussion, bass, piano, and brass; and optional Web MIDI output.

## Run it

Open `index.html` in a modern browser. For MIDI, serve the folder over HTTPS or localhost and use a browser with Web MIDI support (for example, Chromium). Press **Instant Cumbia** or choose a pattern, then press play. The audio is synthesized in the browser with Web Audio; MIDI output is optional.

## What works

- Nine playable instrument lanes: kick, conga, güiro, cowbell, clave, shaker, bass, piano, and brass.
- 64 steps per pattern (four bars of 16), tempo and swing controls, and three starter grooves.
- Euclidean hit generation with rotation, applied to any track.
- Click-to-toggle percussion steps. Melodic steps cycle through note pitches when clicked repeatedly.
- Web Audio playback and optional MIDI note output to a connected device.
- Tropical visual theme with palm, beach, sun, and taco accents.

## FM1 firmware integration

This repository currently contains a browser prototype, **not flashable M-VAVE FM1 firmware**. An FM1-native port needs the FM1 Open SDK/toolchain, hardware/API details, audio and display interfaces, and a tested device. The browser build is a usable interaction and sequencing reference; the audio is FM-inspired synthesis rather than the FM1's native sound engine. Do not flash these web files to the device.

A native port should map the sequencer transport to the FM1 clock and audio engine, map the nine lanes onto available synthesis voices and MIDI notes, and replace the web visual theme with controls supported by the device display.
