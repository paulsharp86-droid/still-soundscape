# STILL Beta 0.7

Upload the contents of this folder into the root of the GitHub Pages repository, replacing the existing files. Keep a copy of Beta 0.6 before replacing anything.

## Beta 0.7 changes
- Replaced random chord selection with weighted, functional chord progressions and short-term progression memory.
- Added restrained chord colour (sevenths, add9 and sixths) and closer voice-leading between chord voicings.
- Added a continuously sustained, slowly evolving chord bed that is independent of melody density.
- Reworked melody generation around short directional phrases.
- Melody notes are selected against the current harmony; a non-chord tone cannot be followed by another non-chord tone.
- Density now controls note skipping, event spacing and note duration. At 100%, notes are never skipped and durations overlap the event spacing by design.
- Preserved the existing interface, instrument choices, tonal gravity, presets, settings storage, pink noise and PWA structure.
- Updated the service-worker cache version to `still-beta-07` so installed copies can refresh.

## Notes
This remains a self-contained Web Audio synthesizer prototype. It does not yet use SoundFont samples. Musical balance, timbres and progression weights should be assessed by listening on the target phone and adjusted from there.
